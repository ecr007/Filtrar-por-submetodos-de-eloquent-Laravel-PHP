# Filtrar-por-submetodos-de-eloquent-Laravel-PHP


```
$students = User::whereHas(
    'roles', function($q){
        $q->where('name', 'Teacher');
    }
)->get();
