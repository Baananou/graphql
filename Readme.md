# Récupérer toutes les tâches :

query {
tasks {
id
title
description
duration
completed
  }
}


# Ajouter une nouvelle tâche :

mutation {
addTask(title: "Nouvelle tâche", description: "Description de la nouvelle tâche", duration: 60, completed: false) {
id
title
description
duration
completed
}
}


# Marquer une tâche comme terminée :

mutation {
completeTask(id: "1") {
id
title
description
duration
completed
}
}