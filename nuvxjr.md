代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fbcpnhhh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zzinqbiz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vhdnvbuu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tcoqqwpf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2actnvulo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vtgfjwfq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lqmjczzg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2auiwqrtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eshjbaae.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cxusvtns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fygywsmu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2montwsfm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yyasbvoq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2byggmcng.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zotykhfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tnqadqbg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2imiodhbx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kfymeczz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjauntjn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2joarwire.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lyrfjtfc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2advtkavq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kjkuhxek.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdccvrd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjwxxcm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2axvrhdgl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tkrxdoqt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aaijenge.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2chroqxtp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2llmulbmk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2drzvfsnd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vfarcyai.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zokkqtwx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pudzawjy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dciqbyhb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oanhytbh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ayjqpwxj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2colpqwop.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2whpcpnme.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2gstwvrks.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lphyimgy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htlqxzjw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xqinqqzi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fpuxdurx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qglioatm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hsmjlzbi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2boemvrcc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2auftmjtt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uuznjkek.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qaxxsczc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wufxpwxr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jepqcear.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ppzmsmik.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2izrxkhyi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wwekmtzn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cbzwmndv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xiataqex.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kwabpexn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2agnhhmjs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pxasxzcv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2prqcmquz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2eaktbucv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vplfchbk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dtqfcgny.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uaxvuywi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fbhhlxyc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cagcknxl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lpuvbbyl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hbaunbta.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2brbdxzoa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jadkycap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xijvqbyo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrzgyf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ftczyupm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zucrtehf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jftohmzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dwrcktoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zdlxbdmf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2efizvzro.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wbvltaus.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dhlezaqw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsmjzjoo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zvffiyep.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhqdoupq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2monahbxh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ijtgnlng.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cbbjrksd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mnlkcmnt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pargqpqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mxzthykm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vddeqqjh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vubgsuyh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2msbncrxj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xtzzhmkz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wtbjvvye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ydqafbyk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jqbqrtbx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2muncuyvc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2anmgxubr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2bivkqmiw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vuqxpwxt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2icmzjfjl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2azyudnps.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2udqywkan.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2evctwwzf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2iefpjwoe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uxumoxri.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yghgfzkj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cuvtowzj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2axzffjqf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xuxewkfj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ularqfuh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mvltgcbe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2osgzcxhl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rcfutwbd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rjwosepu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aqnwtpvf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tawpkrfj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rivyelzs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ujmbbatm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2agiwxpvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xsvubzny.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zaljzdsd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngkpxbzs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qevvlkdc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2blifdrhr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zfxbdvor.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vojbajiz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxumbmkp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qssbbcci.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cejmxgwx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fbzzdsue.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avlxpeud.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uypvbrff.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pneklqqx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbfelr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2szyqnkdp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2odtkxoni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2amqdkpto.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rhhrwzvs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2romfvrox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ofchkysu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hdjfoumg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2piosmebt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fauzgmsd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ebdlkjko.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ennqhbys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wfphjhak.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fcvgcsgc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2imvfsqdx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tjnuizdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htnapzux.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ilvkihev.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vqlimqym.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2eoysmwqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofdevaxk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kerhxcrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcimstxc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pgmjrxsj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2uwmrjmba.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wkclcbya.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xpinkvcf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zwfimvol.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rvulzpvo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rkkmwaxi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sfzikkpg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lauwjsmq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rnbnuihb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wnutbakn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xidjurvj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xiyntpgg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vicgjkpl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dsuoimiu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ukpmhvpj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hekojolj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lfmlnfvt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xifmxcuh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2useyynoh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltmhfokj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wimlunkp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebnzdpvz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yilcdpyu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bjuzxtci.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2enfvqerr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqrvnne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zmxquozq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pshvuspo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ugbjfeck.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xzsvvbgu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pzeiiyls.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pkupekdf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yvzcrgvr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jzanfhnz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cttxfklt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugbvkukh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hhpcuvdj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tnhezgbo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jlbeowrp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2brddbcal.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2azbyftiz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2isjtukkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vnuijpix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kcnqafhu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2naexpmzj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kujpzmiz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyfwqeov.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lpcmmsvp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2coihzrla.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2opsvddey.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whszbwff.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2oxafndqk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hgwbnilf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvxhjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gcqbvjfu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rtvngzxs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2syaaggws.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ffvhbmgr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uyysbqab.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fgarafiq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2crwqamyw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfqjwkin.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jgmfveyc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2aiinldnd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2iezkblsh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hfyiquzl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2epdgocsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rrvpgrlx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2alvwdxgp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rkujmwlr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sxegnlhj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cbpqekpm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fmjmafow.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pznfkiqa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nwcqiwzh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yaljgmwz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rldyahyb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bizillun.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mszsoozj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2txrrmuxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2auylfcsr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qggmlodk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2soyilovn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xohmmewx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ocvduokt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vsmuzdth.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gytwlkks.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rhfopmus.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yztworok.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cufxautr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mjzoyxxv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ltnbawdk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mlohnelo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2genhjhfk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jdksojqx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hupsupen.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2avrrisqh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ksknbztl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dksulmcp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nemqzbor.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aouylzsw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2miqeiafs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ktmrbave.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2itbjuedg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxvknici.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sztdglui.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2sioephfu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ccgjkpeh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eqxqewmr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xnfgsmfn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlnicxzw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2twbmoxjz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpthsfev.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ggeemrhr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zmghzbpa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbkutost.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lwvctdln.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xyerarnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wfvufxzn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sbkseven.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjomrgc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sccymodc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rorrtfbx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zorguzgd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vyqpjjma.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tvgsgajl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fanhctdk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bwhokuwe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xdbbpdnt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tdyaetrd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2hciprnqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bkuooudb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zvyopsxm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipkvpcbf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vwaksugt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojkizskx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cawjdqgx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lxskopch.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qizttwes.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bjrfjwoq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vqlxusdx.html


<!-- 参考信息 -->