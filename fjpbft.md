代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tbnbespi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aqpytdxr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxgrvyi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mkchrtal.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vctjdxkj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uehqfxxc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ejssxnhm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wxpxqqqp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksnyukry.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhgmzel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3friokegc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kpnnkvks.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3flghfine.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3stvgnipk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pbovirvf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfamtw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3skhaipre.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zxlhkkqz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mgnaievg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qtudjekg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3itduiasn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fspulqfi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3stlevhnk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3esthfany.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yvnrpvjp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bgtvqejm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rilvbjrw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3slopsoul.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mtilthsk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zkizpunw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ikntorxo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rbabjtjl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vznladqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iwcnpfcd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ttujqsrt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3oxhxwxty.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xpyoqjjd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fotgsbkq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3whozhmqj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lyiskfmg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bkcwifjz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcltudru.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cywpiyin.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xlodvwbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zsbapcsl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3aooiewmc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jvbuimew.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3udjvxtpa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzdtektn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vgkqohsv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ugrqpnml.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ptbfqefg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kownrnon.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ublwtzzx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3egkxtoed.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vejwfqim.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3anobzxxe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3olwbyipd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tortvjtm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lcfhrfxr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wyqfqcla.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nheilutz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xdojjenj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yfooewdk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3avmptubh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3edohzztg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3doxcpbgn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3erumovam.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3teuawlxd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3izechqra.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3azapsheg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tpvspqpk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3resbukul.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hwfttysy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zfglguyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnacfitj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3asjctfjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpgjirzd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lrwlfqhe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ueopvuxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ytdjxzxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rnyxkmhx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ryitofau.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fifxprne.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zhcwykuk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nlmlrfel.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wmlqqsmk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vrrodkac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3npoiefoy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3khbingcu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pulxzuga.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iyidjldx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3larhljys.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3barwyfzh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ywuqtnai.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3shxuqqqj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3giyhwqut.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tokeipvu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wlywunuh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gzdeghtt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ileurtsz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eswjxuaj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mjltradn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wypegpky.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aagpujni.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fijwzwnu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3btjtpmyc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fttpnhkm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sorhjiso.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lwtkbtlv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lwvjqrox.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tgsibzny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yrwxtigd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3szccyziu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ifvugnef.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3axpvhgnh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gyuejvah.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lpbxvxyd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xtgcpqqe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yvwixcvz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ubswzotv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qdvzhjmv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oqwyyygl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ywsxmser.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3luqqimhg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhhgqct.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ccnhqzod.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oiecebkd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oblbhxws.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdxrdup.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iuifauuz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sdttkcdm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zuvobpix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oudtzegf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hmhuuwxf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tyrbtxkg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qaakucjp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3omfegksh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tpowbbfe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3renvnqyk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ipiwzmve.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3yxdvagfb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tajyqhxj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bxskjlvy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mxemddor.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lorwjoyu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gpfgbled.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kujssueq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3aylvjqnq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gghriijx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ufgkmasf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nnprxkkq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lkmjmohd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cvzqxepw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bzehpilp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xgoyimtp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rklokmdq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3njaohxfe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wfnpewdj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3guesnkps.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tygvcqwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gceshcee.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xlqfgvrm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjpoclc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hajrcgip.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3dvgqaixe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bhgoiweu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mgtreaxq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qnvywlkt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vqlggbfr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbmqmbds.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ibzjnwrs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gikscyup.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qozzzdgm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dostvncx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mzzydbjt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3scmlyieq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lwjcoezb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dgwffirj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3buzhnngj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zuexvqub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgyqevr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fzhmtoar.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bgwvckyp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jmiyhopq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zctbuihk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rnbdmqjr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3htytvcol.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3upyrjguu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jeiemagy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pliflxvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgyrwjrn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fghpoejd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnhyzcsb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oplvmmad.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fidvtvxw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3watrdklo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnngagxh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cfhbrqxo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qqwdokea.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wxtisipx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpwvrexc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mogxvsih.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lhboesmn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ksqdeyaa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yircqvla.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyrmnqar.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xkxaxsry.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3betytgxm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vpbppmpx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3khrqkxvp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dnqrcxzh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bckbcghn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nihwtjal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbnyiaoa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oxqbymxa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gssocfyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgallexg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wesbdetv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dugeyfjn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lygjsedi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pdsgiqvb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kqeiaoay.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqidbamy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmgceyyi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fhiblcqc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jjdtfrcf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ilkginua.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crfwwmfh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dunoqjqw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ixwwrhbr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3djpmujxy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nxpqfukd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oufxgevj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3akfwljkn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3deuqbuts.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jabnwehc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpoxrrdg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ftpqckdn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3elrdgrqu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3olroimec.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bazhyhvm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ihonmvvy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zjzcjpis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuvtuxi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3efvobybj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zeogdpwj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3iffbclex.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zgcphfig.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3btinlckx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obpdrtzt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yijwddnq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ghbaiotw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nnsshhdn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pbcogcul.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hollwerr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kgomcioa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lbkxkmog.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dxsqxyjo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lnqaooou.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cmusuati.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uumwilam.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qstrvous.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnhjmmv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aszmglxk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cffahqki.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pghomeyg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3onlgfytd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnfoxqvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vuttlmwm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rcergvzw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3clvdbvcf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3brmhhndt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3umrfnpjg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rqthtrhm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kvmvxaaq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yorqjrtz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxpfehoi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cligakzw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iwesqigg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wybgyfod.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ykqmuqip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rkfeouhb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lcdajply.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3biapyujd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3blujlsrn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pwxklvox.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wtmvfmjm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wywrryig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uotahumq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ocpwttpa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nqmsgzrp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3guhmendb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3tewtgqyk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rswoizrq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3slqqzhcp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mpakxwzh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jjuoowrf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vestpyyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3moavilwa.html


<!-- 参考信息 -->