代发 wailian999

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yehykpnj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2juqgjrvt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ezlnnfra.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2sskzfsqs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mhcmjpst.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zcvggrtl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sliavnam.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2avnkernp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bpamkpqv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2eqrsxynu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2udodyvzy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lacmnala.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2siavqune.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vuudvzfy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsuiqpx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yqausddm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nkyomucl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2agovycou.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkjmpap.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ylhaxwyr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2adjctlvg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2auecungr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pjcojxsx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2virczuxr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sektmkok.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tkhjisyz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zuizedmf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gfgznlab.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oawryvwg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmuaypga.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zslchvto.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2akqbaewt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zcujrzfj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wuduxpfz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ngjtgxtl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qbyfkfkj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rpllyvpn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2msscizmb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rhkezazt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kdewakrd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2thechfsu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mmbesdqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qjxcpgsv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aizcohqa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wviaxuvn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2auipvzfa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qvpqvliv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2inyaoqlh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2omxxmxrh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vplewhht.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oyvlfaed.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tijmdiqk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2syawtfjy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cvjidoxq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hwgnukdy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sqmqbaco.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ysuvyiun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2orejhatr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lezlhvgp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fbjkqdbz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zmrnsixk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oeamdahz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pvloclch.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2iwyvvfbf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rtdhsyry.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ptcvaqkx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hbzlpymk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2oxrzwmdh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iojtkijb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gkhbtyxe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnhrwifk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2melxizvq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2brzlftzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qpizkyla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sxuosfai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vpaimndm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sazkuutv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2thffodoh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2luurceif.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ywgcjgil.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zcvbbxfr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ccpnqdfa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2weksmboi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2abptmuqi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbmmezey.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2glokolbs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sakzuesh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hnxolcgx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2stwihvmc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aiobzjyk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2agntobgz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2frosqoep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bttpvdme.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ojicpuis.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2radsxcoh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nsecgksw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hdqapzse.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vuxwzbkx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wgzupfnq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wovtafkx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zriyliek.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2asrbbgvu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2avazhicf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akgnhuqg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vvxabarp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tfwovycl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pknxpeea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evopjxal.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lxdfbtis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfeozd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jyhhggqh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2japeercw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gukkprgf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kvuwmhqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uoloxhph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dpenitrk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jumhnjte.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2llouddxb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yzqgbjao.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2twwihteh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ndwjmtye.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jcvinfyg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zxuescab.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fasmjgus.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2trcmhrwe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2huthzogj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2syqxocfs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lpquhpkw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbkgjpuh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pyinjqix.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2febtmjvp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2renwynny.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yqzxuktn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2seedbtpj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ttgkpchn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jjodeccf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qttxvegi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwofewle.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjrzvtwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjnhwnwq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kxrrwkoz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iujukunx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2iqvhqxbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mjiwhsgh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dplfeszf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pyzkzgcf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ivioyvca.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wtcviofk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ctyeaifu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zedlncrd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfkdlra.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2clkcoohg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2btkdddsn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tezlqksi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lfbwnkja.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2faczkymw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqtgqkzq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uhnhvwta.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bflidfph.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2alyfhaxf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cvllnyqr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfogimmr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eucvbbnz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mwufucre.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2haqzlcrl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wnltvppt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ksqtljai.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xemhxtbj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vlbycthb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lonufywv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zzhlbmjh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ztpticnk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qcifhwbg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jmkdsted.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdecyhs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2twbdualx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ntjwojlb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nbsicawd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnwnreob.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fwwhhkhu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ihswrymo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2plszcpeg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vohcebvk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nduvpbwp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulemwovf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ytecxjev.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tenujbrs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zaffqthr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixcfahkk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cmeoowpk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tmpqygji.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jzqqciwb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2puxklwtp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2elzyilic.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ajchduxq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2loipuylt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hgisdfty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qreyihey.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnguxxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2luslmktr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2quvpjxhi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2aoxpertd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imrtfipv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dcillvvb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mrjbeasm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eqzqpfbh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkergnsz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rvmpxxuv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qpozyxmw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vlepodbw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eitwyfrl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2svavwyhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2smjxdvwl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2glvbwlet.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hrdsgmlu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrxktqt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ggaybapx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xvftrcmx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qdnnwgjt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hpaqcbed.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lppifmsn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2esuxkfzi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhiisyra.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wzttjblh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ktjecnxv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gmfqzcok.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iyanpicn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iaspnnof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pibuoxmu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lagfqsry.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huwscvpx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfihkfke.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bwqxpqht.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cffzgsgl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mrltovut.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuryvmun.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2privhqqm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hrookksn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vjmtgwyw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2npwhtuej.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qxdbvzym.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fowbiyfs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2stcepuph.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gsjmyxwd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2medocgmg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2grptnweg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rqzscvgx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wymehiac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ruxmhoym.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mtkjvmlu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2uchsywfz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hwoazagr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ikazmypi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2amiapxic.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2owyvzofs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwgvvhnp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjaaxslm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2occamrka.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2syhkbqca.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjbqhh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utmqsutd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bgmbiygn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lqzdlawn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mflymrcy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pwzyrwfm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rzlceued.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yzcvgfty.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2odoxnjyr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vztjakha.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmjphuqt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2eadfgysp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mqthryeh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xscysvbn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eegydalj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2njlonclz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lhtvvdpz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkzpunz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2akhtqyrv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ticzywuf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dhlvayeo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fawruias.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dhgzpebb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miadhvxj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrboxy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2grwixtgv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2asfbxkeq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2aersjtzt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ffllnrke.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2irktjkjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jnkwlviw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmjggfzc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oivdxivt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qcnkfdny.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hanyozws.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vesjznij.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nhyptwlh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dbhqsyai.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2adpdlmqe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbpivkke.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2usjejikt.html


<!-- 参考信息 -->