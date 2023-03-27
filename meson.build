project('LDtkloader', 'cpp', version: '1.2.2')

incdir = include_directories('builddir/include')

conf_data = configuration_data()
conf_data.set('PROJECT_VERSION', '1.2.2')
configure_file(input : 'src/Version.hpp.in',
  output : 'Version.hpp',
  configuration : conf_data,
)
#configuration_inc = include_directories('.')

executable('LDtkloader',
 'src/DataTypes.cpp'
,'src/Entity.cpp'
,'src/EntityDef.cpp'
,'src/Enum.cpp'
,'src/FieldsContainer.cpp'
,'src/Layer.cpp'
,'src/LayerDef.cpp'
,'src/Level.cpp'
,'src/Project.cpp'
,'src/TagsContainer.cpp'
,'src/Tile.cpp'
,'src/Tileset.cpp'
,'src/Utils.cpp'
,'src/World.cpp'
,'include/LDtkLoader/DataTypes.hpp'
,'include/LDtkLoader/Entity.hpp'
,'include/LDtkLoader/Enum.hpp'
,'include/LDtkLoader/Field.hpp'
,'include/LDtkLoader/Layer.hpp'
,'include/LDtkLoader/Level.hpp'
,'include/LDtkLoader/Project.hpp'
,'include/LDtkLoader/Tile.hpp'
,'include/LDtkLoader/Tileset.hpp'
,'include/LDtkLoader/Utils.hpp'
,'include/LDtkLoader/World.hpp'
,'include/LDtkLoader/containers/FieldsContainer.hpp'
,'include/LDtkLoader/containers/TagsContainer.hpp'
,'include/LDtkLoader/defs/EntityDef.hpp'
,'include/LDtkLoader/defs/FieldDef.hpp'
,'include/LDtkLoader/defs/LayerDef.hpp'
,'include/LDtkLoader/thirdparty/json_fwd.hpp'
,'include/LDtkLoader/thirdparty/optional.hpp'
#,'include/src/json.hpp'
#,'build/include/LDtkLoader/generated/Version.hpp'
#, include_directories : configuration_inc

, include_directories : incdir
)

