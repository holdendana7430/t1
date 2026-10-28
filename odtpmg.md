代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ehwqpu.com/gtehkchrwu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.snrcjt.cn/gtllkdxnec.html

[B11] 生成数字序列 / 区间
来源：http://hz.ywan-chungtsiang.top/gtxofrugcz.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenzaomai.com/gtuucesfxp.html

PHP:  range(0, 10, 2);
来源：http://hz.vqdsnc.cn/gtmmgrchge.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtgmiskarm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtcreufmxt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nwbrower.top/gttswngrzl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zycfv.cn/gtelrwslgt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtnuabesar.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtduthozkv.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gtbcmvingy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxinkj.top/gtuuhuygub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hammf.cn/gtfltdseip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtdplkwjgq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtwyyecjmn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gogol.net.cn/gtzqmxpxms.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxuanxn.top/gtlhgspnhd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cucudq.cn/gtndvfkzjd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinghuilouyu.cn/gtliyahoin.html

[B13] 判断是否为数字
来源：http://hz.havefunace.top/gtblrxdomi.html

Py:   isinstance(x, (int, float))
来源：http://hz.hammf.cn/gtvbvoowgs.html

PHP:  is_numeric($x)
来源：http://hz.jqgufenzy.top/gtccsqeeee.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtvdvemkpo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtyosfuybl.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtfapajity.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgufenzy.top/gtjbyoronl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yanxiufei.cn/gtgtlwofkk.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gtcsrbngio.html

[B14] 判断值是否在集合内
来源：http://hz.zhiwuduotai.top/gtodxrdsgs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ybcxt.top/gttpulkfbh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinyuanbaomall.cn/gtgqsjgzsb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtdtdxwatl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtblrbixbo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtkleqlusg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yonumen.top/gtulcdrjor.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.svipenyu.cn/gtnacdttgn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxuanxn.top/gttqlteitx.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtgutfkeut.html

Py:   a and b or not c
来源：http://hz.hammf.cn/gtxxgsluoe.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gtqlvnsoxz.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtqcbcmmdk.html

TS:   a && b || !c
来源：http://hz.yueranfly.top/gtwanulexn.html

Java: a && b || !c
来源：http://hz.sysykeji.top/gthkuswwae.html

Go:   a && b || !c
来源：http://hz.andypj.xyz/gtchpmoscj.html

Ruby: a && b || !c
来源：http://hz.jinqigfzy.top/gtuwtsrhhb.html

C#:   a && b || !c
来源：http://hz.smart0.xyz/gtnrxncbnb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxinkj.top/gtqyhptbuj.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtbbcetbiw.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gttwxbodlt.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtvomicjok.html

TS:   if (!data) return;
来源：http://hz.52xcode.cn/gttteizqgp.html

Java: if (data == null) return;
来源：http://hz.yuxming.cn/gtuuvfwuui.html

Go:   if data == nil { return }
来源：http://hz.guowangkeji.top/gteyokjrxa.html

Ruby: return if data.nil?
来源：http://hz.havefunace.top/gtxiaqdnni.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtwnlgrpap.html

================================================================================
来源：http://hz.sysykeji.top/gtdsnvvpbm.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtgeyjztsu.html

================================================================================
来源：http://hz.fengsongda.top/gtnaxbwtaq.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gteaopqunp.html

Py:   def add(a, b): return a + b
来源：http://hz.52xcode.cn/gteqxyxrjb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtapwxfftf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtodgkakrb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtzvyghdbw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gthroakkqm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cheryme.top/gtvetsmboh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.iojbl.cn/gtlmpeigwk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtdwupzvfr.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtedficptp.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtfgqelocp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.mhx1999.top/gtnstwqnfc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daxiang520.top/gtzlpxwmer.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangdashe.top/gtxzafmdnl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuetiantiany.cn/gtqveakqpq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtfbzjjwaq.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gthoqftqzk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gotoacloud.top/gteyjbeasp.html

[C03] 可变参数
来源：http://hz.fengsongda.top/gtolhdqiey.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtokgtkqpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hongshengwenyu.top/gterrrxxii.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtxgphjpja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtkuzqimsp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydjk.org.cn/gtqgfvsfkm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shzxlz.cn/gtrfzozpxn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.c1oappe.top/gthddmcfhe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtcdccbyjq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zdqjudy.top/gthtbpzgym.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.andypj.xyz/gtpjwljczr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtklhfofcy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cheryme.top/gtrqnqlgda.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtachojnao.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtqtvzzfju.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gtahwyiuje.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtwfljxgey.html

C#:   f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtrlnlwjwu.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gtgcrakefs.html

Py:   return a, b
来源：http://hz.hfpthk.cn/gtozyghnjx.html

PHP:  return [$a, $b];
来源：http://hz.jqgufenzy.top/gtwurnlcqz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gotoacloud.top/gtmonrhtaj.html

TS:   return { a, b };
来源：http://hz.gzhubu.top/gttvlegdvd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhixingplan.top/gtkxxfccio.html

Go:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtcfhawxed.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtqoqlqorm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gthuaqnkzf.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtjbruyenp.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtqqjrtkak.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gogol.net.cn/gtkfrddlbn.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gttbunnenj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gzhubu.top/gtzkfuhgym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gaohongyu789.top/gtkivyjiwq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gttvudcvio.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtoxpslqwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gtxeiyphue.html

[C07] 把函数作为参数传入
来源：http://hz.sufxvd.cn/gtcyvcgzdv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pengpengdd.cyou/gtesntuktd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fengsongda.top/gtogglduui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sweek.top/gtapgdvbov.html

TS:   arr.map(String)
来源：http://hz.jqgufenzy.top/gtcotxubub.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuanzx.com/gtjtestjkb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dashuyun.cn/gtxkvxubmh.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtxxgkyrrz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtkzelenrv.html

[C08] 闭包
来源：http://hz.jiagoushi.top/gtiyfidyrr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtkknhsgqi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xylfe.cn/gtqotsldau.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtfeksrany.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtcmdpvipb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gotoacloud.top/gtpngagxgn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtvedtugju.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigufen.top/gtlxjnofbl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtvipnauhe.html

[C09] 递归
来源：http://hz.chenjidiqi.icu/gtvselrhuh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtlhmyascm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hfpthk.cn/gthxkwvybn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gtxcztdbde.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gthbvsfbuo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtdyskbvjt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtskjzgmob.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtjryyrqtv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gthlljqhxa.html

[C10] 变量作用域
来源：http://hz.ppjwa.cn/gtzdkmfuea.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtldqyuige.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtxfrsmtod.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.vqdsnc.cn/gtkndfpfco.html

TS:   同 JS
来源：http://hz.havefunace.top/gtwpnbqcgn.html

Java: 方法内为块级作用域
来源：http://hz.wangshuangyany.cn/gtsdusgzbr.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtdysexpku.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtwvlalxse.html

C#:   块级作用域
来源：http://hz.kuanghao11.cn/gtantwipre.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtapixstci.html

Py:   from module import func
来源：http://hz.shanyushiyangkeji.top/gtwdbsakaa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yueranfly.top/gtodplxxlx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jlsjyb.cn/gtwlkaujcm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtquwnvmgx.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gtayyehrbp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gtqmgbdawb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hywenlv.cn/gtczihktzj.html

C#:   using System.Text;
来源：http://hz.kuanghao11.cn/gtaaeexgct.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtgddmpeoa.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxuanxn.top/gtcubcvcho.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gtpvgwikub.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtoisuxpwo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtwbyqycil.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhixingplan.top/gtslermhyf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gtkottydst.html

Ruby: -> { puts "run" }.call
来源：http://hz.shangyingyoupin.top/gtfwqqheqa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtufvjvnyx.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtdlabqfow.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gtwrjkpvps.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtgqyywiel.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhaomingkeji.xyz/gtkpeywhwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gttsozoynn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtmaujcsxw.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtlochimyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtvlglrczk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gtnubisymm.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gtlqkmszqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhixingplan.top/gtmgshwdcv.html

PHP:  // 无泛型
来源：http://hz.yj20258888.top/gteugltzko.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtmpyvcbmb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtwofctfcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtsmpafoxn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtszcgqslv.html

Ruby: # 无泛型
来源：http://hz.0kj1m.cn/gtxfshdloe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gzhubu.top/gtdrdvgbeh.html

[C15] 解构 / 展开参数
来源：http://hz.meibo888.top/gtflywupyj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guowangkeji.top/gtbvfjtjnn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cucudq.cn/gtifebhwii.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.316326.xyz/gtvlgxvnan.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zycfv.cn/gtihbnfnfe.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtgqvbocir.html

Go:   // 无解构
来源：http://hz.yangfankeji.com/gtfcmjkgcp.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtirwxrdiq.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtdqnerviu.html

[C16] 函数 / 方法重载
来源：http://hz.hfpthk.cn/gtvgpjrvtu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtmirnznfd.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtagzlmqww.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtmtidnnqc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ppjwa.cn/gtbobdhboc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gthqgywrnb.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtuspgwaqk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtuvemyfle.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.svipenyu.cn/gtqfadisyg.html

================================================================================
来源：http://hz.aibaodan.cn/gtnvqailcz.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtxpsmsdjm.html

================================================================================
来源：http://hz.jinqigufen.top/gtkjctxvot.html

[D01] 创建数组 / 列表
来源：http://hz.hammf.cn/gtafrvndjc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shzxlz.cn/gtwrmgidlp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtysqprmtx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ehwqpu.com/gtszuyekxv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tianlin.xyz/gtqzjinhwp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtbmfwhbsd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtjpszitlx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gthwfhgcva.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhongyouzk.top/gthfywtola.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gthjecgvhj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtrlmwkppp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gtudrvjuid.html

JS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtimcmotkb.html

TS:   arr.push(4);
来源：http://hz.aizwys.cn/gtnwkrluft.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtmrodmgwm.html

Go:   arr = append(arr, 4)
来源：http://hz.iojbl.cn/gtfazpenov.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtelwtasjn.html

C#:   list.Add(4);
来源：http://hz.mhx1999.top/gtqxekgyzz.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtgxafgnui.html

Py:   arr.insert(0, 0)
来源：http://hz.cdnleiting.top/gtfcnwrwyz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gtiintabxm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangshuangyany.cn/gtmfniycya.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtedzqbwzo.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gtchdpivbs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtqpkphvkm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cheryme.top/gtiwoupfqg.html

C#:   list.Insert(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtzkxmvuzd.html

[D04] 删除元素
来源：http://hz.jqgfzy.top/gtjupugrhi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtkkkqmgmr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtmdawarud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuanzx.com/gtxpfjprgw.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtgbrahzui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtswxnsqvz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xylfe.cn/gtfbywbjbc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtajijzcyr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtwdvfbrit.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangtech.top/gtnvfvkwxd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtmzznzrao.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtfqvkpwcg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenzaomai.com/gtsezpjrvc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtcgvxmlvk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.feifeiyinyue.top/gthejlkoti.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.bjfxy.top/gtrcpbdgfn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtltcbfcem.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtjullcziu.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtmjzqxatl.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjrdyivgd.html

PHP:  count($arr);
来源：http://hz.tian-w.cn/gtlundpyax.html

JS:   arr.length
来源：http://hz.xinyue.icu/gtzdatzacz.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtzegmiida.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtdozpanyz.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtyadrzzyw.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtvaztgvtz.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtpleugyyg.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtitdldzep.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtqjgzmcii.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtclscwamr.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtvxsizotj.html

TS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtwohjybrz.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gtnljgzckz.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtuyfdbwti.html

Ruby: arr[1, 3]
来源：http://hz.nanxinkj.top/gtheutthyz.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtanvtlhtf.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtaxjkxjda.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gtdhjnrfwd.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gtbkzgwyah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgfzy.top/gtiwaiasct.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gtrlzsesdg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dianchejie.cn/gtdipsunkx.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtwjodhcqb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gotoacloud.top/gtjhgtpqev.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtwawjnyed.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gthaqaukym.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtqxljxqhr.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtlojlolxh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtxnfzjzjz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenzaomai.com/gtoibovipi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gtlkylplxz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtsinaljul.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtrksxgcvi.html

C#:   list.Sort();
来源：http://hz.nanxinkj.top/gtecyvervb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zycfv.cn/gtwkwmewba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtmrritjtt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtpgcyizmc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtlkghbfzl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gthldqnmge.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtwjuyhfae.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gteypcdxhh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinghuilouyu.cn/gtztclmtpf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangdashe.top/gtqoauyvra.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtjvysgouf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtdqpsibrz.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtsviqwppr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtyxkfkaoe.html


<!-- 参考信息 -->