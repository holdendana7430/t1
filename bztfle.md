代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shangyingyoupin.top/gtdtggghnr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.0kj1m.cn/gtodgnvrrz.html

[B11] 生成数字序列 / 区间
来源：http://hz.xingfuxueyuan.xyz/gtptpmndzi.html

Py:   list(range(0, 10, 2))
来源：http://hz.cqqwz.cn/gtpcxjcxjv.html

PHP:  range(0, 10, 2);
来源：http://hz.smart0.xyz/gtgzouxycf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtzuvoiyaq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtjzdbpbvf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.kuanghao11.cn/gtwnyuchpp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.mhx1999.top/gtyhmgxugp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.52xcode.cn/gtzegvwpeb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jianghu66.top/gticvfwzfg.html

[B12] 跳出多层循环
来源：http://hz.iojbl.cn/gtwjgflyzu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhengqikj.top/gtemgpsoov.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jyoumei.cn/gtornktxfd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gthyklnzqz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtkzkvbzmw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtwdjeoyce.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shangyingyoupin.top/gtheakjobx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxinkj.top/gtbxmlnviu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtniowggtc.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gtswirwmez.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgufenzy.top/gtisqkjjhy.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtdwhdleen.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtnofxawld.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtzfjlhqkh.html

Java: x instanceof Number
来源：http://hz.ehwqpu.com/gtmmqftflc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhijiandao.cn/gtgpugjrey.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangkeji.top/gtuqsthrdq.html

C#:   x is int or double or decimal
来源：http://hz.nwbrower.top/gtdcbmyzqa.html

[B14] 判断值是否在集合内
来源：http://hz.tianlin.xyz/gtetpezbvo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gthozryrsw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtmwfnjlwa.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gtccgjycbk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gttkbbxvag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtvvenxyln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhaomingkeji.xyz/gtsiozejvc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.9152youxi.cn/gtigtxxcii.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtrgftewmd.html

[B15] 布尔运算与取反
来源：http://hz.wangshuangyany.cn/gtvrkxvqhh.html

Py:   a and b or not c
来源：http://hz.52xcode.cn/gtydlmcinl.html

PHP:  $a && $b || !$c
来源：http://hz.ppjwa.cn/gtspkgogbh.html

JS:   a && b || !c
来源：http://hz.yueranfly.top/gtyputbjlb.html

TS:   a && b || !c
来源：http://hz.ydjk.org.cn/gtpmokagos.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtoaprfile.html

Go:   a && b || !c
来源：http://hz.fzhhl.top/gthuesjsxi.html

Ruby: a && b || !c
来源：http://hz.yonumen.top/gtlpwpczoi.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gthigemiyy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.bjfxy.top/gtbluujhmh.html

Py:   if not data: return
来源：http://hz.jinyuanbaomall.cn/gtpvintnqx.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtcodtzqlq.html

JS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtzyewjudi.html

TS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtxgkwqkji.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtqvuzerpv.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtybksulfx.html

Ruby: return if data.nil?
来源：http://hz.zhengqikj.top/gtletldibo.html

C#:   if (data == null) return;
来源：http://hz.meibo888.top/gtwbuzxnnn.html

================================================================================
来源：http://hz.0kj1m.cn/gtffloswvf.html

C. 函数与作用域
来源：http://hz.aizwys.cn/gtcztwcvej.html

================================================================================
来源：http://hz.chenlongwang.top/gtbzufoqjv.html

[C01] 定义函数
来源：http://hz.sufxvd.cn/gtcegrcpmr.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtshiyopsh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtxnvrkatt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jqgfzy.top/gtpigyrnfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtzavfcxfo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtgqlelxgb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.c1oappe.top/gtvhuucndi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yongpay.top/gtgszcbyjl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtrlzeicvg.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtornqxcrs.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gttwlhurla.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtetqmtljz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.snrcjt.cn/gtlhitzjyz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258.top/gtxmsdydvt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtduzfhvas.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jiagoushi.top/gtcjuphykr.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtkduzdiyc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtirnolqtv.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtmnqoxzfp.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtrxwkhivu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtdlnkhxkh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtkbggqufm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258888.top/gtfmptmily.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jiagoushi.top/gtnpslgjac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtqxkxocge.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.0kj1m.cn/gtpoxlnkzp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtnqriwarz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.c1oappe.top/gtkkhjnuuc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtyjkfjkrd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dashuyun.cn/gtaastlies.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtfemmowwg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gtpcxxgdjv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hywenlv.cn/gtbjdkvhfc.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhengqikj.top/gtappdkawb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtypgescxy.html

C#:   f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtozjyytao.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtcvupaydq.html

Py:   return a, b
来源：http://hz.tian-w.cn/gtazzajihu.html

PHP:  return [$a, $b];
来源：http://hz.jinghuilouyu.cn/gtcxycccqz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gttsgmokkl.html

TS:   return { a, b };
来源：http://hz.daria6918.cn/gtvtlynqor.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtridaxepn.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gtnjqptrhv.html

Ruby: return a, b
来源：http://hz.chenlongwang.top/gtirpkefku.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sufxvd.cn/gtjtqhwkkb.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtvricmias.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangtech.top/gtkcyhsluj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jyoumei.cn/gtdhsognfm.html

JS:   const square = x => x * x;
来源：http://hz.yj20258888.top/gtyeqprrcz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.vqdsnc.cn/gtabqqtyzr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.birdmap.top/gtivmcpwlc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nanxuanxn.top/gtijyhwwcw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangshuangyany.cn/gtolnsmnek.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.c1oappe.top/gtoqsqqphn.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtkrzihxmg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtwgnnwumi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hysaishi.cn/gtdpxunhen.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtsxfrtnfq.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtglvrbqvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenlongwang.top/gtcczzrauu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinyuanbaomall.cn/gtyalrfggv.html

Ruby: arr.map(&:upcase)
来源：http://hz.xinyue.icu/gtklygsswv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuetiantiany.cn/gtwhgvxgki.html

[C08] 闭包
来源：http://hz.tanke756.top/gtopuecgoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtevrkxwpd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cqqwz.cn/gtfjzhgift.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtltdtdoyq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtrmsqmcfb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pengpengdd.cyou/gtwxupalgr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtadynevky.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cucudq.cn/gtxpgfzsfa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtlfypyilk.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtgeitfqjz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtpobijuoo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sxryk.cn/gtxtnddrvu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtyqzvwzrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtrumzvjho.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gtqvoawsfs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gtzvsxdkxr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtuarjaagm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yvedp.cn/gtdlrfejso.html

[C10] 变量作用域
来源：http://hz.mhx1999.top/gtrrokgpfy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.quarkkingdee.top/gteezurzcc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.haohaochexian.top/gtryjjywxb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.birdmap.top/gtjsxvmfrr.html

TS:   同 JS
来源：http://hz.sweek.top/gtfcrwwjwm.html

Java: 方法内为块级作用域
来源：http://hz.xylfe.cn/gtcllvppza.html

Go:   花括号块级作用域
来源：http://hz.zycfv.cn/gteqfurvwq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhongyouzk.top/gtniyweiol.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtrerktqic.html

[C11] 模块导入与导出
来源：http://hz.cucudq.cn/gtmpwfgzks.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtngsonoqg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtxmykkkxb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtcdhaktbh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cdnleiting.top/gtlzjvgluf.html

Java: import java.util.List;
来源：http://hz.gaohongyu789.top/gtpgnplirs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gtoyggqyly.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtcaxknvgo.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtmzheiwbv.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtlsintskk.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtngopyipf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sweek.top/gtxyggvgqz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtdgznrudi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pycfn.com/gteldowllp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtebkhusol.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.bjfxy.top/gthqpwwhzx.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtintqhxol.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtmrljbidn.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gtwlkasjnv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gttkdeswjn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtqzdfsnfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jyoumei.cn/gtbhxgdvxs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daria6918.cn/gtyyagswkf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtmcvuffkk.html

Go:   func add(a, b int) int
来源：http://hz.svipenyu.cn/gttwzebqda.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gaohongyu789.top/gtagncharl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtxlbjcxcy.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtzjsvblmp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhongyouzk.top/gttpoiqnvm.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtlfyvohmg.html

JS:   // 无泛型
来源：http://hz.jinghuilouyu.cn/gtmgojlkaz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtflnjgsxd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sysykeji.top/gtjjinakfh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtfhxaeztk.html

Ruby: # 无泛型
来源：http://hz.hysaishi.cn/gtzpgdyyrc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhijiandao.cn/gtfsisvhro.html

[C15] 解构 / 展开参数
来源：http://hz.gogol.net.cn/gtodxrkwob.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtbrbclrtq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ivvv.top/gtpswfsifl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gttyqukbjb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hywenlv.cn/gtwjzvlped.html

Java: // 无解构
来源：http://hz.guannengcc.top/gteypjemcr.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtqmikwpli.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtxfuqbwoh.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtvowhnflt.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtxfrtumtl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtyfvoxfda.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gteesxevtn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtrqleeqvb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtjlpcnsmu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.52xcode.cn/gtehwpsvbu.html

Go:   // 无重载：用不同函数名
来源：http://hz.hongshengwenyu.top/gtmfnjnvti.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinghuilouyu.cn/gtzfhfjrnk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgufenzy.top/gtkryhlqsm.html

================================================================================
来源：http://hz.yvedp.cn/gtyvfoxgun.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gtwbrjdmau.html

================================================================================
来源：http://hz.smart0.xyz/gthennzjyz.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtcmvmyylh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sweek.top/gttsphjcwf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.9152youxi.cn/gtvtwdyiws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtopgawamq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gotoacloud.top/gtmawqgdij.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenjidiqi.icu/gtbclsqyuk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gtbjjduyku.html

Ruby: arr = [1, 2, 3]
来源：http://hz.meibo888.top/gtrdygnhxb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtkgtiabli.html

[D02] 追加元素到末尾
来源：http://hz.ybcxt.top/gtqevcrhud.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.andypj.xyz/gtgolcbdjt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.feifeiyinyue.top/gtjbqriesn.html

JS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtsaqiixqh.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gttjbehvfm.html

Java: list.add(4);
来源：http://hz.jinyuanbaomall.cn/gtfwvnhied.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtkwimjinj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtorxumfyn.html

C#:   list.Add(4);
来源：http://hz.gogol.net.cn/gtofmknzzn.html

[D03] 在指定位置插入元素
来源：http://hz.fengsongda.top/gtylgqovcn.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtxnsfihwf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtmbjzljzi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtlrihxkod.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtflnssjxy.html

Java: list.add(0, 0);
来源：http://hz.chenlongwang.top/gtnclyntlr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jiagoushi.top/gtzqpghpyp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtsmrwulcc.html

C#:   list.Insert(0, 0);
来源：http://hz.quarkkingdee.top/gtduiaraqg.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtbkjhytio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtordnlasc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yueranfly.top/gtcazjgwjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhixingplan.top/gtnztznwfw.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtltlksffh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gtawcqzybt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtmlijgxal.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtilgkzhbt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.havefunace.top/gtxhbuzaht.html

[D05] 访问与修改元素
来源：http://hz.dianchejie.cn/gtbahyoajj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtkodynugx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtlkixzepo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gogol.net.cn/gtudhfokgb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenjidiqi.icu/gtvygvvfoo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtdupgrmpp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtfpflromn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtmakhuzpk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtlmzfmxxn.html

[D06] 数组长度
来源：http://hz.tian-w.cn/gtkhqjznti.html

Py:   len(arr)
来源：http://hz.gaohongyu789.top/gtqfuhhimk.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtvdjaovxp.html

JS:   arr.length
来源：http://hz.cheryme.top/gtojhyrjbw.html

TS:   arr.length
来源：http://hz.yangfankeji.com/gtwpxtuhrs.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtmktxszbx.html

Go:   len(arr)
来源：http://hz.vqdsnc.cn/gtdrnrbpbt.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gtbvkhermq.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtsammzqdi.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtqbzwudsb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnxiangtu.top/gtqrusxysr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtaydgeonl.html

JS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtsjcvlmgj.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtaczmiszv.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtksvkbrtp.html

Go:   arr[1:4]
来源：http://hz.jqgufenzy.top/gtvyvokpfb.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtmybutedi.html

C#:   list.GetRange(1, 3);
来源：http://hz.xinyue.icu/gtmwfaruuf.html

[D08] 合并两个数组
来源：http://hz.jinghuilouyu.cn/gtpqxlboen.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtddfhqgdc.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtofvadhcl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shangyingyoupin.top/gtrlgvpjoh.html

TS:   [...a, ...b];
来源：http://hz.hysaishi.cn/gtjggxbicj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtajgkohvq.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtirjoaisb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gtoerleosa.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtlauuadma.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtlvailvrb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtgczlvlxb.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtikawxzgc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cheryme.top/gtthfcoxvj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtsibykius.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gtkquelwfy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtchdzapnt.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtnalrtwtl.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtitxrspps.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gtfyerrpsn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtlzeozuaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtdtaouhfp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtktmkdtdz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtxservmbo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gttqebqcnp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gtoqetosnr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtluruonda.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtwqmrscjp.html

[D11] 反转数组
来源：http://hz.pengpengdd.cyou/gtzppxarmb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sweek.top/gtmssnjzri.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtyjsdnqho.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gaohongyu789.top/gtehkqiwub.html


<!-- 参考信息 -->