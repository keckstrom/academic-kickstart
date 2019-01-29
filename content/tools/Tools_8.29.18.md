#### Tools 

##### Compiled lists of resources

- [Comparative genomics in bacteria](https://www.omicsonline.org/microbial-comparative-genomics-an-overview-of-tools-and-insights-into-the-genus-corynebacterium-2155-9597.1000167.php?aid=11588)
- 



##### Graphics and Visualization

###### Differential Gene Expression

- [Morpheus](https://software.broadinstitute.org/morpheus/?ref=labworm)



###### Venn Diagrams/Comparisons

- [Venny](http://bioinfogp.cnb.csic.es/tools/venny/?ref=labworm)



###### Genome Comparisons: Circular plots & multiple loci 

- [myCircos](http://mycircos.iric.ca/?ref=labworm), may be limited to human or mouse (double check)
- [easyfig](http://mjsull.github.io/Easyfig/?ref=labworm) should be good for the Steno CF isolates
- [CoGe](https://genomevolution.org/coge/?ref=labworm) 
- [VISTA](https://img.jgi.doe.gov/cgi-bin/w/main.cgi?section=Vista&page=vista)
- [CGDV](https://cgdv-upload.persistent.co.in/cgdv/) requires BLAST or some other comparative output to be run first
- [CGview](http://wishart.biology.ualberta.ca/cgview/) can be used for other types of genomic viz as well



###### Heatmaps

- [Gitools](http://www.gitools.org/home)
- 



###### General Visuzliation Environments

- [PAST](http://folk.uio.no/ohammer/past/?ref=labworm)
- [Gephi](https://gephi.org/?ref=labworm)
- [fluff](https://fluff.readthedocs.io/en/latest/usage.html#rna-seq-profiles) python based package, focuses on heatmaps, bandplots, expression profiles, etc.
- Tableau -> check again for a University license? may be installed on iMac
- 





###### Generic figures/pathways

- [bioRender](https://biorender.io/?ref=labworm)
- 



##### Genome Assembly & Assessment

###### Post-assembly Analytics

- QUAST
- [Assemblytics](http://assemblytics.com/?ref=labworm)
- PATRIC, including recent [protocols](https://link.springer.com/protocol/10.1007%2F978-1-4939-7463-4_4#Fig4) paper



##### Annotation

###### Functional Annotation

- GOfeat
- [Manatee](http://manatee.sourceforge.net/)
- [PGAP](https://github.com/ncbi/pgap) now available as stand alone local tool (requires lots of dependencies though, may be best utlized via the VACC)



##### Alignments & Variant Detection

- [Roary](https://github.com/sanger-pathogens/Roary/blob/master/README.md)

  - potential workaround if ubuntu won't update:

    - convert genbank files to gff3 format required: On NCBI's website, GFF3 files only contain annotation and not the nucleotide sequence so cannot be used. You need to download the GenBank files plus nucleotide sequence and convert them. When downloading, click on the *show sequence* option, *Update View* then *Send* to a *File* of type *GenBank*. You can then use the Bio::Perl script *bp_genbank2gff3.pl* to convert to GFF3. Just be aware that mixing different gene prediction methods and annotation pipelines can give noisier results.

      Alternatively you can use [ncbi-genome-download](https://github.com/kblin/ncbi-genome-download) to pull down the FASTA files and convert them to GFF3 with Prokka.

    - Roary using virtual box (windows) or through [Galaxy](https://toolshed.g2.bx.psu.edu/repository?repository_id=143d84eeaab68c4b) toolshed, or [EU ](https://usegalaxy.eu/?tool_id=toolshed.g2.bx.psu.edu%2Frepos%2Fiuc%2Froary%2Froary%2F3.10.2&version=3.10.2&__identifer=4p2fd655g33) of public galaxy

       - ​	other galaxy info that might be useful about adding things from the Toolshed:
          - https://biostar.usegalaxy.org/p/28949/
          - https://biostar.usegalaxy.org/p/28925/
      - other gbk to gff3 convertors
        - https://www.hiv.lanl.gov/content/sequence/FORMAT_CONVERSION/form.html
        - https://www.biostars.org/p/134589/
        - https://github.com/mscook/to-gff


      ###### Insertion sequences
      [ISmapper from the Holt Lab](https://github.com/jhawkey/IS_mapper)


​      

      ###### Tools for read manipulation/quality control
    
      [seqtk](https://github.com/lh3/seqtk)
    
    ###### Phylogenetic tree construction
    
    - alignment
      - [MAFFT]
      - [MUSCLE]
    - tree construction
      - [RAxML]
      - 
    - visualization
      - [iTol](https://itol.embl.de/)
      - 
    - general
      - [Holt lab resources](https://holtlab.net/2015/10/03/plotting-trees-data/)
      - [SRST2](https://github.com/katholt/srst2) get MSLT ST info from WGS short reads, [explanation](https://holtlab.net/2014/12/27/behind-the-paper-srst2-for-short-read-sequence-typing-of-bacterial-pathogens/) from Holt lab website
      - 

- [Exelis lab](http://www.exelixis-lab.org/software.html) several good software choices

- [RAxML-NG we server](https://raxml-ng.vital-it.ch/#/)

  - phylogenetic tree

- [REALPHY web server](https://realphy.unibas.ch/fcgi/realphy)

- [MAFFT](https://mafft.cbrc.jp/alignment/software/) 

  - alignment tool, can handle large numbers of sequences for comparison, widely used

  - webservers available at [EBI](https://www.ebi.ac.uk/Tools/msa/mafft/), [MPI](https://toolkit.tuebingen.mpg.de/#/tools/mafft) with [PHYml](https://toolkit.tuebingen.mpg.de/#/tools/phyml) available for the viz of aligned file, [TREX](http://www.trex.uqam.ca/index.php?action=mafft) with every step of tree building process, [CIPRES](https://www.phylo.org/portal2/tools.action), 

    

      

- [MEGA6](https://www.megasoftware.net/)

- PHYLIP







###### Web-based tools

[phyd3](https://phyd3.bits.vib.be/index.html)

[DTU online tools](http://www.cbs.dtu.dk/services/software.php)

[microscope](https://www.genoscope.cns.fr/agc/microscope/about/services.php?wwwpkgdb=0fdc5afcbe29eb84137d5976237f6314)

[Gview](https://www.gview.ca/wiki/GViewQuickStart/GViewWebStart) java applet for circular genome viz, looks limited to singular genome, not comparative

[GrapeTree](https://enterobase.readthedocs.io/en/latest/grapetree/grapetree-about.html) interactive tree viz program, similar to PhyloViz; available as stand-alone or integrated in EnteroBase. Looks great for adding additional data/plots onto tree formatted data

[CiVi](http://civi.cmbi.ru.nl/) circular genome viz with the ability to layer on multiple tracks, appears to be restricted to published data?

[CGDV](https://cgdv.persistent.co.in/example_cuffdiff.html) makes circos plots from a variety of inputs/data types -> look into for RNA seq coverage maps potentially?

[eggNOG & eggNOG mapper](http://eggnogdb.embl.de/#/app/emapper) requires protein sequences, but then provides functional annotation of large datasets



###### Visualizations

- Stand alone tools

[Circleator](http://jonathancrabtree.github.io/Circleator/)

- R packages

[FigTree](http://tree.bio.ed.ac.uk/software/figtree/)

MEGAX

[BioCircos](http://jonathancrabtree.github.io/Circleator/)

[OmniCircos](http://www.bioconductor.org/packages/devel/bioc/html/OmicCircos.html)

[ggbio](http://www.bioconductor.org/packages/release/bioc/vignettes/ggbio/inst/doc/ggbio.pdf)

[ggtree](https://bioconductor.org/packages/devel/bioc/vignettes/ggtree/inst/doc/ggtree.html)







###### Conversion tools

[genbank to sequin](https://chlorobox.mpimp-golm.mpg.de/GenBank2Sequin.html) may be better for submission than python script. Other tools from this group may be useful too



###### Useful R packages

[BitSeq](https://bioconductor.org/packages/release/bioc/html/BitSeq.html)





###### Resources

[omictools pathway protocols](https://omictools.com/search?q=cancer&tab=protocols&utm_source=NEWSLETTER&utm_campaign=e2381af1b3-MAILING+PROTOCOL+3&utm_medium=email&utm_term=0_53e9df1916-e2381af1b3-230269757&page=1)

