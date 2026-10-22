代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzuqvjpz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2frpgyxsj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yunbhqqn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdudspd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lfeycjev.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxsaaifv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ltxcctjc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2liefnlbn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ziyeetwc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qigpavar.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwhozstb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fdglaxcz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kvkjbbuq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bovhltmc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uaruplhz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mjmkwhxs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iacillzm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ooieegjx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pxojghxq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wtdnkvwx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqquaz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cabzdigd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gsrxmowt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2krwssrno.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zaoxuqjv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uizhtaea.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wdicbkfp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2sswrkoqt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uxpmxgns.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxwzdc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vpxcablo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swsmwgiq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bzkzfctr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yospieuz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cspwksgh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zmdabeis.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2snuwcamr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oijkmmbz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dsxewaho.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2doqxlxmt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yanwnhtu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hyvicnqh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pxxbavba.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2atrtfqca.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2knejbtay.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2oyywismg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtsnjpq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qrvrwzhe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eosavboj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ebcaykix.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2odbgvauf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fmdrzfvp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bajvvjjf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qmjromue.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2brxnhblx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xqkzhigj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2npjtpotp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2acspftew.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nfpeycpk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jtbxxpqj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xxeomhlf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uaphaxau.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nkvtkuyd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fdiwfpob.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qlryzzsm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2knpkhzxs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fotvadfn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ksfzjwwn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2krgcongz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tewbzsxx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dukgqsmj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zszmodwa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vlrqnqvi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xmwkslal.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lpzdsrgb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gtcaqbjc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ouglfotv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lktmnfcj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zpbkeuhr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2lbbcmbuv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wmjybyzf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ksohtysi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyavdnne.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2biuyobgi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zyefxmah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2boaubesz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aykvwncb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rsbntjit.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2afdmorsi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2viivqtwv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lzjilkkw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ycwwuvcy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ijynxucl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ckbysnbq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2adcpoirs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bqujjkpu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uiollxgs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lgrtwhdx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rcwjsyto.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cfpjiojr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2upmgogkn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2sglctoxq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2aytvxnyv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ypcpyjxs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ccohovdy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tjkydbjl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vnyhbnjh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2siswtanb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lkszdvfh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mdegjbaa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qtexwtxk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rcqrfygx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qozlpmts.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hlpqnnok.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2krihfgmp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jjwdcscj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lefspmgw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2luvfykmw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olfuzjuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsmuitbv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2scczzaym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eotwyccr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ifttqxzi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ddspdzxe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qqthnvib.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vpkwekaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ptphytcg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2aapedtno.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pajguxgv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aznfbhml.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2igyuwuit.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vfaauffo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ymenroar.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jifdrlvv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wadwcdjp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgbkboui.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yemenzvi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gxexsvdv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tngrwvdv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dpsmlrhc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rreonric.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kovzbwxl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgvbgjvs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ouoobnyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2grarhamk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cubautmm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vabjjfby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gwpurpgv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uailwdzk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jtphhabe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vorgxtls.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eenykghw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2thzadiax.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2khltmuiy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzbhnjlj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxkncphs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwxpfwau.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdpeyunx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dpvlnqqf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vnxxnmbx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ztvzjixf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uwbarbcd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfoyfrzg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2arfejerp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bsatgcso.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2clxiienr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bsqvgrfe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hljtkyfn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2owbhozuu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pxdlcnsz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywrvagge.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gulequsj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qsfpbpys.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibvcyhyt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nuqtayfl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xzfctpgp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zbhdzbyz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tprqiymd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ghshzuhe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cusjonwn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dyzeaqgz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2avxyqqax.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kxannvgu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vgjiiaef.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nbaaywkj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hulrqkrv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctuyirsg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rlciyptp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lsnwtyqu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2uxbfzney.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2sgrcsrsm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xuyxkxqg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xqyzqdmx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tszwiwow.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2keythkwt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bzsbujrw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mzadcgrv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2oupioxnc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ygiginbh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2joxctcnn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wzntdrxb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jnxhbbdl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2keuawikn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wlsodyye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usmzcnfn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vwyifgwo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2obmzhlfa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gfepzzxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2knvmlxlt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fhdkkenw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tfkyrljj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nheruehn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vapvmhdu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ghttcobg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2etxlwhbn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fkjxebby.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2seebvxmo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxsiduds.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdewtrs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uqumdght.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2urhzdkgp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2eelpboje.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2imrcldre.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbievpkp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ntejlzgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pqosjvit.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qkxwnhyx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecmswxvb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aevphgch.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fwcnnqwv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hyecsgxw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2euaknrwq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2urcsqtoh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ucgniqxc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aalnxzar.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2khynqttu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tzealazv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2slevaskb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifnfcgxs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ocwabito.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iqrrmgkh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2agyotqco.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ebglaaty.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpzaewam.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eglbrrmg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kkvzcles.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fqckpwur.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2glldpetk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wkguwbrd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zdgjoymu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqnvapoz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sjltftxf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qeoguwjf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xiiamptx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tkheiimu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2zizjusfu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gegawpzz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ylomscnz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkungblu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wisetrww.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfmmjzcv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lozerpss.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2labjsnqk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xpbqtney.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qfibmxue.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2valmrbgf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qinqxtus.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tjibvlqe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cpfjfwyo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tjaicwny.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lrfcisnx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ztuqykns.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bwnstorf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wfpcqqit.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nrfxlcgc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jiuqwift.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rsmvdoqx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2klfjkpxd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dtyeorzz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2emaiwdps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfulgypk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wdwxlktq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2znufybwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kscgogrg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qpgypows.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dblmrlgv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2apmmktvx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pqubdyzw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2coodlsaq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2coabfyeu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jqrjwtnr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxcswb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ibfzcxey.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xchyqggx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxmxyuek.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwcwoqlb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wgynpkjw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fauszvsq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2blebcjqv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tjaerqnu.html


<!-- 参考信息 -->