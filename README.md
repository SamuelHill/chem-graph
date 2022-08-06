# Background

N/Z charts are pretty neat. Finding the data needed to make the chart isn't to challenging, but it is
evidently enough of an issue that some chemists wrote an [opinion piece][1] about a need for a central
repository of isotopes (they really want all the relevant findings in one place but thats more or less
what I want here too). As well, even [IUPAC][4] is getting involved in peaking interest in isotopes,
and subsequently adding more data to the already packed periodic table with their little aplet. The
table is so packed that 4 different layouts are available on [ptable][3] to sort through the different
relevant info such as the isotopes, the electrons, or just general stats. Plenty of places exist that
[have some data on isotopes][2] or other general info, but most are outdated or incomplete. Due to
these factors (it being hard to find a place with all the data) I'll just use the [same source][6] that
wikipedia uses for its [isotope stability list][5] as it has a good interface for accessing the 
underlying data and seems to be as close to the repository that I mentioned at the start.

With a little effort, the above data could be scraped and re-graphed. To add a third axis to these N/Z
graphs we need to choose both what that third axis should be and how to tie that data into the already
semi-scattered N/Z data. The options I have thought of for a 3rd axis are; number of electrons, 
[ionization energy][10], and the [orbital shell][8]. The first two of these would be much easier to use as
they each have an associated unit for the axis that makes sense - num electrons is as it says and
ionization energy could be eV. To use orbital shells on an axis I would have to order the orbitals and
I'm not sure by what metric as [orbitals are complex shapes][11] that are themselves defined by three
parameters. Just too keep all the axes in units of numbers of a thing, I'll try the number of electrons
on the 3rd axis. To get known ions I'll use the [oxidation states][7] which wikipedia has the best list
for as it thoroughly combines the main source and plenty of ammended footnotes. Now that I know the
axis I will be using, I have to figure out how the two graphs will merge. Do I only put the oxidation
states we know about on the stable isotopes or on all the isotopes? We can only get some isotopes to exist
for such short periods of time we still don't know the electron config so is there something about...
How to filter these views to see layers within the mass of isotopes and ions? What layers matter? What
will a layer even be for such an oddly curved structure... What do you color code with? Stability should
be the same regardless of ionization... Hopefully we can find some answers by just trying it out and making
different models.

N/Z charts are charts of [nuclides][9] - with one axis (protons) being essentially the periodic table drawn
out in a line (or a list of the elements) and the associated row of nuclides are the isotopes. On the nuetron
axis you aren't really getting anything that we would normally graph (nuetrons with stable proton configs?)
but we are seeing all the isotones in these columns. N/Z charts are a graph of the two necleons found in
atomic nuclei and from that view rounding out the graph to include the other common component of an atom,
the electron, makes sense. Although, from a subatomic particle view this graph is odd as it is two baryons
graphed against a lepton, but since subatomic particles can't view this graph and - again - this is what
atoms are made of, it makes some sense to round it out. Overall though my reasoning for this stems from an
admiration of N/Z charts and an incessant voice in the back of my head saying make it 3D or what about
electrons. This is largely just me making up something that doesn't exist (probably because it isn't useful to
anyone) and trying to answer any questions that pop up from it - i.e. research. Maybe this is misguided -
I'm no chemist or physist - but graphics are fun and if nothing else I'll learn something from this.


[1]:  https://www.pnas.org/content/114/12/2997 "Need - central repo for isotopes"
[2]:  http://nucleardata.nuclear.lu.se/toi/ "Nuclear Data Search"
[3]:  https://ptable.com/#Isotopes "ptable isotopes"
[4]:  https://applets.kcvs.ca/IPTEI/IPTEI.html "IUPAC isotopes"
[5]:  https://en.wikipedia.org/wiki/List_of_elements_by_stability_of_isotopes "wiki isotope stability"
[6]:  https://www.nndc.bnl.gov/nudat2/ "wiki nuclide source"
[7]:  https://en.wikipedia.org/wiki/Oxidation_state#List_of_oxidation_states_of_the_elements "wiki oxidation"
[8]:  https://en.wikipedia.org/wiki/Electron_shell#List_of_elements_with_electrons_per_shell "wiki electron shells"
[9]:  https://en.wikipedia.org/wiki/Nuclide#Nuclides_vs_isotopes "wiki nuclides"
[10]: https://en.wikipedia.org/wiki/Ionization_energy "wiki ionization"
[11]: https://en.wikipedia.org/wiki/Atomic_orbital "wiki orbitals"
