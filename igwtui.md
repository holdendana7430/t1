代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.yanxiufei.cn/gtjbtbaqut.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtqgxyhjgo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtdunyszyg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtcenuuxge.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtqsjjzggu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tanke756.top/gtldgppeif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sweek.top/gtmlwvpzrd.html

[B12] 跳出多层循环
来源：http://hz.yueranfly.top/gtgtbwrkyj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hammf.cn/gtguucrbds.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shangyingyoupin.top/gtobkpquzz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gteiexgebi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bjfxy.top/gtrybyqwyi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gttxtpidkw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nwbrower.top/gtrxagjfiu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hongshengwenyu.top/gtmubhjyog.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ehwqpu.com/gtxmqernlw.html

[B13] 判断是否为数字
来源：http://hz.chenjidiqi.icu/gtiaxyxryw.html

Py:   isinstance(x, (int, float))
来源：http://hz.svipenyu.cn/gtcsztespp.html

PHP:  is_numeric($x)
来源：http://hz.hysaishi.cn/gtdkwgwyau.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtwawaeast.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gtsmsnejfe.html

Java: x instanceof Number
来源：http://hz.hywenlv.cn/gtkvgusdbu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sysykeji.top/gtwjpxdkfj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gttfiupueu.html

C#:   x is int or double or decimal
来源：http://hz.shanyushiyangkeji.top/gtfyokrcwq.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtgvuajdel.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtujlhcvkg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtceklvkor.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtolwnewzv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gtvlygrwhz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pengpengdd.cyou/gtwqfzrzqj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ybcxt.top/gtmvfdaeff.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ppjwa.cn/gtoneodebr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtjqixlhgw.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtzpuznymf.html

Py:   a and b or not c
来源：http://hz.aizwys.cn/gtrexfqjon.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtuukbdvzt.html

JS:   a && b || !c
来源：http://hz.gotoacloud.top/gtytvczcgv.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtopfyenhl.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtetnwgglv.html

Go:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtndnjkcwh.html

Ruby: a && b || !c
来源：http://hz.zhongyouzk.top/gtakedpdvm.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtscpxlaod.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtatbecdev.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gthiwirmdi.html

PHP:  if (!$data) { return; }
来源：http://hz.cheryme.top/gttutpdgva.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtlnuebztl.html

TS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtqrjzouxe.html

Java: if (data == null) return;
来源：http://hz.snrcjt.cn/gtrmdpxcsj.html

Go:   if data == nil { return }
来源：http://hz.vqdsnc.cn/gthcwjacob.html

Ruby: return if data.nil?
来源：http://hz.yvedp.cn/gtuijynncg.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtbqnbavkx.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsguhwwaj.html

C. 函数与作用域
来源：http://hz.fzhhl.top/gtfpllfoyn.html

================================================================================
来源：http://hz.jyoumei.cn/gteqfocabq.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gtvhkyboba.html

Py:   def add(a, b): return a + b
来源：http://hz.yueranfly.top/gtzycfdcvj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtvszuhahy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shuidangran.top/gtrhncymda.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtsyadffai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtwjvwtzlw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cheryme.top/gtsscnrgbu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pycfn.com/gtvsogugle.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gttnvpbkec.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtuvlmyjyy.html

Py:   def greet(name="World"): return name
来源：http://hz.xinyue.icu/gttrlmtfgz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtrnnjgxjp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gzhubu.top/gtiekrltfl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hysaishi.cn/gtvazkmbkt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtyvuezdux.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtppritqwz.html

Ruby: def greet(name = "World") = name
来源：http://hz.guannengcc.top/gtgkuzvhms.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtbcinouvm.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gtlycegiep.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtvfvelyfu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gtwjdfwanf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tanke756.top/gtqdvmnsnm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtxabjptzi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.quarkkingdee.top/gtxgozzdoi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtxxspaodv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtyzaxnmaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtpfbqqyyz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.0kj1m.cn/gtlmbgeobg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtkbqjacmd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtgvpozjmm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gtinlttqpp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgfzy.top/gtsefuasuj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jianghu66.top/gtfkpkbbsm.html

Go:   // 无：用配置结构体参数
来源：http://hz.gzhubu.top/gtuwdaexov.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtrmrrcvuq.html

C#:   f(a: 1, b: 2)
来源：http://hz.tanke756.top/gttyorxbjm.html

[C05] 返回多个值
来源：http://hz.zycfv.cn/gtfvsjkvkh.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtmpkydcnp.html

PHP:  return [$a, $b];
来源：http://hz.jqgufenzy.top/gtxziczdts.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gttlaamjyh.html

TS:   return { a, b };
来源：http://hz.snrcjt.cn/gttrltqfkt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tianlin.xyz/gtbasqcfbs.html

Go:   return a, b
来源：http://hz.yvedp.cn/gtamvgbpwc.html

Ruby: return a, b
来源：http://hz.mhx1999.top/gtiknjkcpp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtxaubmvfl.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtarkcjrzl.html

Py:   square = lambda x: x * x
来源：http://hz.zhongyouzk.top/gtjqecqnhh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jyoumei.cn/gtsdvbntvb.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtzndsnhhf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gtanqpqjna.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenjidiqi.icu/gtclgfoeez.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yueranfly.top/gtzcwcibqq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigufen.top/gtlfxpluhb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gthdbbymks.html

[C07] 把函数作为参数传入
来源：http://hz.yanxiufei.cn/gtufaahmcq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gttagtrpkr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shangyingyoupin.top/gtplnpvmoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtdahoqcux.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtlrtipird.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gtgqgzssrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.iojbl.cn/gtrlpezgsf.html

Ruby: arr.map(&:upcase)
来源：http://hz.sxryk.cn/gtdccuwvie.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aibaodan.cn/gtvcphazgd.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtvaqhopnj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guannengcc.top/gtlviinyyt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtqxufrjll.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtynjgzrgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtjjwkvyvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtzidkobvg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtbxyxjjbs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtgdsaeenb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gteqfjuoql.html

[C09] 递归
来源：http://hz.zhixingplan.top/gtnghbdmmg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtzzwpwcoe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ybcxt.top/gtvecilfom.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gttywjybot.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtpeypxevg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtxkaetvcs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangtech.top/gtdxyfiecf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtvycpeatq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nwbrower.top/gtnthsskxa.html

[C10] 变量作用域
来源：http://hz.fengsongda.top/gtsicipthm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sxryk.cn/gtvfaxpfmr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aizwys.cn/gtxoobsehv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtjkasvgex.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtfllyiwpa.html

Java: 方法内为块级作用域
来源：http://hz.zhijiandao.cn/gtbgrpjotn.html

Go:   花括号块级作用域
来源：http://hz.bjfxy.top/gtqkajqqcf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.0kj1m.cn/gtjgktzxxn.html

C#:   块级作用域
来源：http://hz.cucudq.cn/gteorxyltw.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtnbxpvxxj.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtazyhpgyj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtbsjzthbb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gtofsndtwa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtbvhoggsb.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtbtvzopep.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.bjfxy.top/gtznqryghi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtblkinwta.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtcdzxgqmi.html

[C12] 立即执行函数 IIFE
来源：http://hz.gaohongyu789.top/gtmamtupoa.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtvqupaukr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gtsihhmeoo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtootlfutv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtwbosysoj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yvedp.cn/gtcrzwsvis.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtjjeplsbk.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gthkqikvtw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtbiwumixr.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtuvmuvstn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangkeji.top/gtubioxpzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gthcxerlxq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fzhhl.top/gtoexnunck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtshxqhzmh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtaroabifh.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtetmehlkf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.iojbl.cn/gthpezswax.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtnnmsejsh.html

[C14] 泛型函数
来源：http://hz.0kj1m.cn/gtqhczebef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnxiangtu.top/gtugmrzdjt.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtihdhlmmj.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtvasqekhk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtcjnubrvx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtxwatvxnv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gtpqaxfstj.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gttvdtrmsx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gzhubu.top/gthljgruoa.html

[C15] 解构 / 展开参数
来源：http://hz.tian-w.cn/gtpmykbbzh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtjwaqfgvq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sysykeji.top/gtugczuakg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gthatydhkf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.mhx1999.top/gtbofidqpg.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtizcazecs.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtagjqfwek.html

Ruby: a, b = pair
来源：http://hz.jinqigufen.top/gtvudjibmw.html

C#:   var (a, b) = pair;
来源：http://hz.hnqzz.top/gtvmxfudqr.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtwmfcicmt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtjsncphur.html

PHP:  // 无重载
来源：http://hz.cdnleiting.top/gtvoeouyuc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gttyquxmpt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtggxaavww.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtsiboithy.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gteonwwfxk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtcmzpaadu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtpuxamybr.html

================================================================================
来源：http://hz.yj202588.top/gtrlbeozjc.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxinkj.top/gttgqshyvs.html

================================================================================
来源：http://hz.shuidangran.top/gtubucezey.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtwrnondmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.daxiang520.top/gtmkrdxboo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtzgidwihc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtsugsthvw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtfihqzynr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtewcwhqyh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtjswmkbox.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtrlumbuoy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.9152youxi.cn/gtdlnjwnvh.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gttrdtgysq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtgdhqslgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtvnqkzyfm.html

JS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtiixwvqik.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gttcacpbxm.html

Java: list.add(4);
来源：http://hz.xuetiantiany.cn/gtkwkdqssa.html

Go:   arr = append(arr, 4)
来源：http://hz.yj202588.top/gtosogzdox.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtglwdgsuk.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtyeydbdpy.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtgxwmacgx.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtisuygvzh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shangyingyoupin.top/gtvgrywywk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtrieayqvh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gtfmladirj.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtwqbukple.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhengqikj.top/gtovenkzga.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xziqi.cn/gtexmeutrl.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtlywdfjya.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtpxgqrlms.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.snrcjt.cn/gtolwpincq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtvpstfnlr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtmrdsvshc.html

TS:   arr.splice(0, 1);
来源：http://hz.jinghuilouyu.cn/gtezqihsbl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gtjtpgmdso.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtzdfutpfn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtdltatobu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtwxhaoqcy.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gthroyuxyr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gttxczdkkh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenzaomai.com/gtsjhmmpag.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtvyqoembg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtwpjeoswy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zycfv.cn/gtgyizmdje.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtseitrytz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtjvgkkpua.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shuidangran.top/gtcxqbynqc.html

[D06] 数组长度
来源：http://hz.shangyingyoupin.top/gtzzxqpfgw.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtunzabcmi.html

PHP:  count($arr);
来源：http://hz.yvedp.cn/gtnknnulru.html

JS:   arr.length
来源：http://hz.xinyue.icu/gtgzucnwsz.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gtrcrsozcx.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtllrimaty.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtzuizgnxj.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtoqkwllwk.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtpkvagocb.html

[D07] 切片 / 取子数组
来源：http://hz.snrcjt.cn/gtyqvnxagl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.0kj1m.cn/gtmsibjmjh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cdnleiting.top/gtdqlbxtat.html

JS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtlxfltcje.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtkltsazwi.html

Java: list.subList(1, 4);
来源：http://hz.jqgfzy.top/gtfhimghus.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtibppigli.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gtvdyultuc.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj202588.top/gtpededhfk.html

[D08] 合并两个数组
来源：http://hz.jiagoushi.top/gtjlbtvjss.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gturtqxbad.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtdibkwtmf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtxyobcndi.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtwjjtvygh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtwpsuaxrs.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtvxzfzmei.html

Ruby: a + b;  a.concat(b)
来源：http://hz.andypj.xyz/gtyraybvfd.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gtghfgqnny.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtzkqpuslc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gturfmipmj.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtnzvtrjhv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.feifeiyinyue.top/gtlxlcsnzs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenlongwang.top/gtsbrvobxr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhengqikj.top/gtarwqzkbu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtsnxxjzqt.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtyhaamsrh.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gtydmgfwtu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtmwyqkrbq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.kuanghao11.cn/gtulnepgsh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.snrcjt.cn/gtjgiioxtx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtlhhsuzer.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtmqycmcrb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gotoacloud.top/gtvmgcgcmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gteyogjeju.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guowangkeji.top/gtqgmjinsk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtpvhghusb.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtetzghflx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinyuanbaomall.cn/gtbuswteda.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gthuhwvjkn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.quarkkingdee.top/gtrzpjeequ.html

TS:   [...arr].reverse();
来源：http://hz.gogol.net.cn/gtmkjatelx.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtxgxffetj.html

Go:   slices.Reverse(arr)
来源：http://hz.feifeiyinyue.top/gtbkhfcubd.html

Ruby: arr.reverse
来源：http://hz.smart0.xyz/gtkkmasvcx.html


<!-- 参考信息 -->