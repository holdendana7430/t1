代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dezgyvks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3inyonnmd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcerwrr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bwrodxbq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tekfljrq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjjwfaye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lsvqvjnp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uddzrcbh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqutkogy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3esndgoju.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3svjswgng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcfatypf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kjstdxjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3aeuewsou.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qvkoxbue.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mmuvmdet.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3clswvcoy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pukwdxeg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rlknugue.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lhoorwpe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukgpoqpj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3igzjtxjb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mmffkjmy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgxteet.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3srpnrswz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jvdxztek.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3brrhvosz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rdxsbnjt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jkrebeou.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xiolqjhu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hloutyis.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xmoldkvb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3icggaqzl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ytxmplbq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kovadjsu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lkawamsh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jcytxkwd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tyfnntgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cknonjag.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wzsopypn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gexwgwho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3verqoqwr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wupfwtlz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rlwqegwe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mwyrynii.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gxcxdgpt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yhzykkex.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3iucnmxwi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vctiithz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kblahlhb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3odvzxdrc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yctnrmkv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhscxhsl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kunevmfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vmvporza.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gfnmeapo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jbhvnptr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3whbjscsd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3sooqectv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qwnxaozv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sxifkrbu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kukctzfr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nwcqtguk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rryoarnm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3alnygymq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwhosrs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ssfwcpzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tgkvvirs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fgvpqfzr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dfllggfj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vsihesuz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzgrrhob.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nedzjhpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3noplkqwo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqvhbanw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pohqjonq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nszxrryc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xorpxbjf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ybutfocs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fshdanhh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hwkknhbx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3doilpupi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pefkgoqz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lyoqvkou.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3grfiehae.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzepql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ahqbpalh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ecwsocqy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3blgzpawc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vpdxcjtt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eoulhugo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bhlrzalk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wwuleicy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xfofwvrx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwvywwr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hfzsicmf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dyeszoyc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmepntg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dgvvdcks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3yiznafbq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3izwwclsn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvaksktf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3njcctyxi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3afdsewcd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3htsxwlvi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbpwdkdo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3auhwnfba.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3trauvtxg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kmmsbziz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsiymqh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mjmyedmz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfbyzfj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3evipqypr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3buuqlymj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ibwdedbc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jypglxuj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxbyqsn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vfjbpspy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3iytfobre.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ujeqkzrb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hjaplzql.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kcbsdvoy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gclgrdzr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tdnfaxtm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdzpyiii.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qtbqkgtg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zagkvjge.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pyrnsgxv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fjknacen.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmalesog.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vmronfwo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wflpnhup.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dxorwago.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dlkaijmv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykridkse.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ztemrlij.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ahsetoaz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3okxsvqfz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lyozesru.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ryldlasa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zwyrmgto.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xetlkfeq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ovppvomv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uyfpfkqf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tphqskwf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kzhdmssz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgllamxj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mxxlihua.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpxbmlf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3frdaesse.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qlirbnnx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qdzopphc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3lvbscomw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tnhcsjpx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3saopsmvq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vjfqefru.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwhlxwe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xhhrcvbp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3okhdiliq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bvxtlens.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dlvqmxzx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gcuoipoy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvoocft.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ezkwngig.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gfkohkfd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zadpkieu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3urpgklgd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dqeypvkx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3riuxcbbe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3axadksin.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyldewer.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pagrijup.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3khbhhppv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3esvzsepn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cnuldadg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rxekyixd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aqlioybl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qtmxmafn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pnlfgjuw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hmtphrtb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cpmjewdk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kvshetht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3agqdpuml.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pekawfub.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yfczkbzg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pchueqfh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hiphedci.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dtufvgwu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jbekgbhy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gdoigrqw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qawdvjxt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dxalyicd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3yghfqcsn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbsofmcz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ngxqvsdh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3efghivwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kvhhhrnd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yolqoyuy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hkyotkxk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zcgrgrzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pndnlgkp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3frvfnafx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hifvlvyr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nbwzgyok.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3phvmerlp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3stnqclwf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsasrnuc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xwszsbeb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lxljhrnt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tncvfluv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qogpvezz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ypplsonu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfuoygjl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ldujrwro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnsmtfmo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zqazyaif.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oevlzjei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdlslqc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uvoxlbrm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ugfnrblp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qvokukhb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pgsbpzqn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqflkqkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sawvsygs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wfcwbsmv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hjuejmeh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tyvrtkfe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3luposfce.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nvycxdet.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gcdpkdlu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yjxzlnqq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmmskexh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yjhsvvpf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3swuuovbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oauvvpfj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qdqsvpmk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtejidfo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lducclwv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zijfbumw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxjosivh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pmtuzpke.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvppjnk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lkonqzqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3axcfejhv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ppgzimwe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tqompwth.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cqbonnqt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fboxpuko.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iilppjlb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fjlfsywa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ydeediha.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3opvemevt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kntfrixl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pduuaivj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dogckdhq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ddimetfn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pfzpkefq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dqzvsasn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hhiptfym.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gruwquae.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3eqkzkylp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3riouawmi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuyleasu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxgsguzq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbftmcjl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjrsjgf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uogyhbnu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dcyqailz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3owlkmopd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zsmzdttj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jcuafwqc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zoourcsq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iagzgzby.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qmctenty.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gqsntdkf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xfkrvafz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3atprmrdm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yqxjizhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xjuecgal.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3grgdggve.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vzfjdudf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3livaeimu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3biwksaoo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xjqlwykh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yswvuosk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3yupklukj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ennzjzml.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aijpxifc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfysffzg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxbantf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kbizfaim.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3skqjricl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gsrubyql.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3sdyivuvt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3omnsnxgl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sufqexsa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nasfzkod.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skyzwcxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qiprjmnf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcncktd.html


<!-- 参考信息 -->