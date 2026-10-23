代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rexeyzdw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3chvravwj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3getzkmom.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmaaugi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pzgcouov.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjsbvtu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3natlrpgq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dsvtfkpr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tulklvaf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mjalavuw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ryvwzngb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ecqzehpa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkmstnvi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hwjfgxil.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkmjdmpa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vudghnuk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wftofpkx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3avvfxahg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwllpvj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ynshiuiu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3idmuusmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3znczfopw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3liftnmgw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cyxgnkip.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fiigovyz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pftzzpwj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gzdcaklh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nusupzcx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nuwwmucv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bqcofoln.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bcrlxzmz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crssaamv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yybmxffy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gywhayyv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxnaobng.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tidwvhyz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3msvhkbwc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3telndlqf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vvnpyckn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lbbosviv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wdeyunmo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3llcxdexs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nzmxjjfe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yfjcyzah.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3spkdwzwp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hntdyjdn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mycnwxny.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ughmqbtr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xbvreuuz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ndzqebpz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fomdaoqw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fiskfbed.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sdhljlde.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hnrhmlkg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ikrnuzno.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lfhxqmwl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3eksxkpmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xuznxtnu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ygesrald.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmoeijzf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3azrwjttv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3jkpfcnwr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3klkkpneo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nillchws.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3finycxly.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jnlxdsot.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uvrshcrt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dprggjmj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbndqqoz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntmljdje.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fmiiyeej.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kaasqxbv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ytnspfkt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lnoguase.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nrfsvsay.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wgjvnfmw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwxycfsc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kfcaoauo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cjzxzubn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mskwbbtn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yhlxzkhl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yfigcsnq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dizwqanv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gqxxhhvh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3imcsapka.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zjfaofiz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hjcdcymt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mldvxadr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3iprzwfjr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3umjwkxyu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivkmassh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofuxojnj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rbebixgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aydthwib.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tkcnpffq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3khtlftev.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3znaisqjl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3omaymosy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3czicnnde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zptkfptd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3llbmoiwo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rsvhlhqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lpghwybu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rlrfpcit.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mwcpsfmz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zyaoabjs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3craleylx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehpkvmvw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mvfpzmvj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvnhvea.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3amrbssku.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtqksvha.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ufhlfdbj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gvtmsivj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmbkhzal.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fonpgnoz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3npypuhlm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ivkwoxib.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3paqzckvp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nkxamdff.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3olenvdfw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sbvkbtfz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxoweyu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhghbymi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cogzcrnv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bflpkqpk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ysttggem.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bhbreoep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kspkzkvp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvgqexli.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fcdgubtd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3myloswwp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3clzcjnxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qzfmexuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rmspvnio.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3srokvnke.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qqpeeviz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lksskttd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rzactfoy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3siwshdqi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oufutejq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wlhoopbr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3horaocmn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ojfqenet.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yzmbafgb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfoazsi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oxtzunnw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ixwlzkho.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tszizmob.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bfmkasge.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hemyzobn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zlkshnaq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ykaqdhkd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lvmrspyd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3innmktvh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qnnbftla.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3edprhcrn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tczujyij.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kjcxofsu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3efofmnbk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yulgpfeq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jrqqzduo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjhqhtnf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zunnnxmz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3whalgyyl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcpaebnb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fqicrgqb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3asnztstu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wteojtmy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rtedzblu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tzbiiyqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ucgovylb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjkaglie.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3biwkeuyk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3aufbnxcu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sccyekks.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iwgjqrsp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ikxzmahl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkanzjx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aepkalad.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ahanggjg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zxncbkuo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oprmmxlo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ypivnftt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ssgebqvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3swvumnbm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3flsgoppa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cflmigvt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3swryovwi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3aoybtupi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pktgzvuh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3obhfzopi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vuwbrhmz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ovcifzcs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3earyqtwh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ktksvckl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmsqnop.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rodwgunr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ofzyfduk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ykonjhng.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amqfqyfi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3juncnpkx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3eapvffga.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kkkzzaai.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xzllqwor.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qgwvlrvu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3olnhozbz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nifhsbos.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dvoseuvu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3armtfcbh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3etbfwsmc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mubspysq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rudlzwuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oocmxpyc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcmbtgzr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bijldhqn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3saedyqgb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3luiptluo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rfkqnrme.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvpoiizi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zkemdfxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ankbdczp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcacmchd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3spnhwyzx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rhgkrkza.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pfwzfnns.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wjuidibs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jrywuymn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fenllrrt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tthgmrtu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3afnbdeen.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jusivoab.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbkdugym.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qojgmcbs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fsipwiru.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyztre.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ojnfamkg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qlhcxjly.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3njuydpqm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgbiqya.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dgqwxmdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3absejnle.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxcdcpkc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tooftocd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkxbom.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ctiwlpfe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgokyn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3slmveoko.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3skjtrgxo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3blfntueb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qtuvdzsu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mcoqrnfq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ssrxewor.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bjnaeeae.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ebxvzxri.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sczvxgyo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3zbkaankk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mugfwvxd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qcbokyro.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3agslxetx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjjzhph.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3eefcbylc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jmosvdeb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kppeotpj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gfshfkuw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3szfzcxrt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptugxtdb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kebtfxfx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3meomsbqf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vwogcldm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uzjvvpsd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xxngteay.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3parnttlb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fdoncphe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dirmwyou.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3eguyctly.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mckkpdrf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vkwppdsi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ycwkapqs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwlwedtf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gvkrrsjv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tearjfez.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qwdmregp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3heldsuws.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ermsrqfq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3libileiq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwtmzmpz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vkqzgkgs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebltgacc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3epxlxloo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3oywlwcgm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jcrlbcth.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zqfptipn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdcubcf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqdjvmur.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3devdgego.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wtagszzc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvpfegq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3idlssyfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nuebrnmo.html


<!-- 参考信息 -->