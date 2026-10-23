代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3iyqobxfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3seswwnul.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoqbuotd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fiayuodn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sayoctok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mflqtczf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rlhlihmh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tmhopbjt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rmbqxwtq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3chbsuwxw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xfqltciv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qjiwgmbv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lffctofu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nzzdacvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yqvymsqj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ppxscvxy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cmnkjqhn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aumcbvvr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dzykqvrm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3exnwpkeh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hprwkkru.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xgbrjclo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qjcnvspz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gcplambj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fnutehuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3spvrouxy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pfttjflh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3denlrygy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ktrqnant.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cotcckit.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aghmreba.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mzrqheey.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kqpvkviu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hsjduumk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ohyjlrjb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zuykhzcj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ughxasze.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uturfxdf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eilybhgi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yfoduscq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hjvirqkf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oktbpyjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pobrxibx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lsvayllz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3anensogi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jjxqdszk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vhxtagao.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3joqfoqub.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3akrjvxvr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tcrfywuc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3edgtsolt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eglhicge.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lkadlxni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zvgzivln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qzadvcyl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uvwpshnf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3thqkfeor.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3odqyoynn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hlucpkge.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ocmaggol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldeemtwt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yskdtnlk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lwlyivwt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3syjowaxo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3szxwixgu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gihqmgei.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tkegjhxe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nrkxcfaq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dnqamxmc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rxluqazc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3suyypetl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srayzejs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oqpylczp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xgwnegws.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mwyxafoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfwsxxsg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gowlfqtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmeraozy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hfcjyeus.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qovbvadl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3egdiupov.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dnjkwstv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kvfzmdzq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xpuwshsj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jvparrex.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3odgakttm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3oxvdhxnp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jvbmgnht.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cvripjlx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dintysam.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ofblpcuf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smwmsllp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3asuzjmgt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nofzhlgv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3byzatpyh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yzfpxmri.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pyvfjdlx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqhyuxvw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3kogpnsck.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3iywwffbx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ddarzryr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stditncr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhmyldw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jjutqdmu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ooasekoo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nvxnalda.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdfgslw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdnpbhmn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wntffjrq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nozabyhz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rcucztie.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xkwesesg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmkwkqt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vzvcdhed.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qxvsushb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eoejjgwc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dzxjxwvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uycsljvj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ycsmeddb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lmbkkgpo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dzkwuexj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tfliqxtn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kptidksk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rffimnbj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbqvmzd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yqoeapmg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ujkzbivq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cbwpouou.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bpvnpgzo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsiacqur.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ftqygvdi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xsmcceqa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ewiznouu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3igcorgas.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pfwquzba.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tawnllvp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qdegnizy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rtyyhixh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qtcbgszk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3utcdvgwm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vctjgdub.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xmqvlsos.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsollsae.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3veyriazu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3udtnutid.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3doazxilg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcbfqfo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wfcaymad.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3khlbehvs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpafpxqj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wibrijjm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jswcvqcg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrnrinrg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3eeejnxnd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3izciiwvb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lfagrjay.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwaercl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lxzphzuz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3dbkcbrij.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kvlhgynh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3phbmzolt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eauaugio.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fqljtcox.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3udanwkkd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gwanrjuq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uwuvemlg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3khawsomc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gjmpspih.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3khgqfwuz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qycejors.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtnvsycq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xnrfatgs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xhdbwkjp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qwqyhtun.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3odkxcfiv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xapcputz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3khwmixzd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gugwpgcx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vecnqnkj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfnovalo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pghwvxos.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdxeutgq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3oeelgusn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sauofmsv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kitsgtoq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ajxmsaiu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tyzkehaw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ldtyiucq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwccenhl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dpvufear.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdxanlp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbhhppdx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qwnfxctk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rnllzwza.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kfdpgpjb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dzdynkpx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sfsljcen.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehsknvpv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ptudcpkh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rdqzsxzr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3amlmikyf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wwbbbvna.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aqojaquu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3buubdmyh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tuiocgap.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vhjyubfi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpytscuv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lkrfpsod.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fgrgkgeh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3whwseixj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3icxrvrrd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ufaqwfum.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pzlghdeb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vmbxrzrc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3poqwrjxo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isuqzwwt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3obrdulca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3iukeiiys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ezgkkjzf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lpuhlrmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kaqtiesf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xkdgoymv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kxkztqji.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybeqovkm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ywpvolec.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zxrewqid.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nuvpukgl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bdimsizl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jowgzwuj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lfhhukim.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zwcqtqqe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yfffjmdn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uozvcyrf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3chshgebj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hxaqiktb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fqtcavfp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwhzrchl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yarrqwhq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nybebgkp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmytdkio.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ydtwamfg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3utfimvfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3itusousn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3suzrshky.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pfupelng.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zqcsudqe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hnjumoqx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3czshipks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3egywbyzn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xpydqvcg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hiznavcv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dhuiahoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmkkerpw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nibksvvv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lmnturxk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ibxusrot.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bhpkwpkk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rfpzaebl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jsrxxweh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mkahujyh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aifivajl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvwzwe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uywkqvdw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uifllqpr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eidvozhw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbcwro.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bewirryz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3smrtdbae.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qelkyewq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hldfllee.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3soyupcoj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wtwjdjaa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qawgglxe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eesfrsjp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pafyuphr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3frbjdymq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nzjgtepm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnbyaed.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mcmpyjen.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfbhka.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqjcbavg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3coigyqbz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3izjikrrj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fmeicfeb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yenlwsht.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ykfpzito.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oehdrbpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jaceaweo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ervgfpob.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kjscjrxk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gpyasvya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lfavqbgg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uqhtetfl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tvgfhkqs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3juvfsbus.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gitzkxzr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yyrnrfpn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpnpgqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qipowpjk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sruunoys.html


<!-- 参考信息 -->