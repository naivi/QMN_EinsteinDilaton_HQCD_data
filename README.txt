README for data files associated with:
"Transport coefficients and quasinormal modes in Einstein-dilaton holographic QCD"

Each .dat file corresponds to a figure in the paper:

figure1_temperature_zh.dat
- Columns: zh, T(zh)
- Use: ListPlot[Name]

figure2_speed_of_sound_T.dat
- Columns: T, cs^2
- Use: ListPlot[Name]

figure3_im_qnm_tensor_sector.dat
figure4_re_qnm_tensor_sector.dat
figure5_im_qnm_vector_sector.dat
figure6_re_qnm_vector_sector.dat
- Columns: mode number, Im(w) or Re(w)
- Use: ListPlot[Table[{Name[[i, col1]], Name[[i, col2]]}, {i, 1, Length[Name]}]]

figure7_hydro_mode_vector.dat
figure7_hydro_mode_analytic.dat
- Columns: q, w
- Use: ListPlot[Table[{Name[[i, col1]], Name[[i, col2]]}, {i, 1, Length[Name]}]]

figure8_bulk_viscosity_cphi.dat
figure8_bulk_viscosity_eo.dat
- Columns: T, zeta/s
- Use: ListPlot[Name]

figure9_bulk_viscosity_jetscape.dat
- Columns: T, zeta/s
- Use: ListPlot[Table[{Name[[i, col1]], Name[[i, col2]]}, {i, 1, Length[Name]}]]



figure10_speed_lattice_c004.dat
figure10_speed_lattice_c022.dat
- Columns: T, cs^2 (lattice comparison)
- Use: ListPlot[Name]

Files can be imported using:
da = Import["path/to/file.dat", "Table"]

For plots requiring columns:
ListPlot[Table[{da[[i, col1]], da[[i, col2]]}, {i, 1, Length[da]}]]

For direct plots:
ListPlot[da]

These data files allow verification and reproduction of the figures presented in the article.

Contact: n.villarreal@ufabc.edu.br
