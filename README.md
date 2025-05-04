# ToHeart utils

## To compile:

```
cd LVNS3
make
```

## To unpack LVNS3SCN.PAK
```
mkdir indir outdir
cd indir
../extract ../LVNS3SCN.PAK
```

## To decompile the scripts
```
for file in *.DATA *.TEXT; do
  ../decompile ${file} ../outdir/${file}
done
```

## To compile the modified scripts in `outdir/`
```
cd ../outdir/
for file in *.DATA *.TEXT; do
  ../compile ${file} ../indir/${file}
done
```

## Known issues
Unpacking of LVNS3DAT.PAK is not supported
