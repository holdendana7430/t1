代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xylfe.cn/gtixzhnxnb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tian-w.cn/gtsauxregb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sweek.top/gtucysphic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.mhx1999.top/gtesfwfwbr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtctzlacsm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.andypj.xyz/gtohoyasee.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gtijqcsiwb.html

Py:   list(range(0, 10, 2))
来源：http://hz.guannengcc.top/gtdoonidwe.html

PHP:  range(0, 10, 2);
来源：http://hz.feifeiyinyue.top/gtulhvyspx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtwtzwzwkm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtemchtmiu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuanzx.com/gtoooihwen.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xylfe.cn/gtbffxivvn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtmlczaidy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shzxlz.cn/gtitzlrarb.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtvirklcbj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.iojbl.cn/gtfzcajaqc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.pycfn.com/gtvfcqugoh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtuxivksch.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtkwegvdpa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtrhxoyafb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258.top/gtghnyohwj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangtech.top/gtfvnavhdn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtivwewhgd.html

[B13] 判断是否为数字
来源：http://hz.smart0.xyz/gttegnhghe.html

Py:   isinstance(x, (int, float))
来源：http://hz.dianchejie.cn/gtrzsxocvf.html

PHP:  is_numeric($x)
来源：http://hz.iojbl.cn/gtylevgwbd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gthpxnlsvy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtllvhrgvt.html

Java: x instanceof Number
来源：http://hz.jqgfzy.top/gtaswfzgmt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtjuntcsar.html

Ruby: x.is_a?(Numeric)
来源：http://hz.52xcode.cn/gtskhpivln.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtdpowufqo.html

[B14] 判断值是否在集合内
来源：http://hz.havefunace.top/gtodmeczzf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.fengsongda.top/gtjmlkainu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gzhubu.top/gteeohzkec.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtuyraltyb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtpqjwnzti.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangkeji.top/gtnxilnbip.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tianlin.xyz/gtpkakfkxm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtrkbyayet.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yanxiufei.cn/gtzxagbiiv.html

[B15] 布尔运算与取反
来源：http://hz.cucudq.cn/gtdwjwvuah.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtorvxbfei.html

PHP:  $a && $b || !$c
来源：http://hz.hongshengwenyu.top/gtpzczgrsa.html

JS:   a && b || !c
来源：http://hz.nanxinkj.top/gtotohydcv.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtwlqaipns.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtkliseaph.html

Go:   a && b || !c
来源：http://hz.c1oappe.top/gttbcttksd.html

Ruby: a && b || !c
来源：http://hz.yj20258.top/gtvxbrrcav.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gteughyvgv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258888.top/gtiuxltcgm.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtpxthhctq.html

PHP:  if (!$data) { return; }
来源：http://hz.jyoumei.cn/gtxgdfiiif.html

JS:   if (!data) return;
来源：http://hz.cheryme.top/gtvumwptbj.html

TS:   if (!data) return;
来源：http://hz.jinyuanbaomall.cn/gtaevvywwi.html

Java: if (data == null) return;
来源：http://hz.chenzaomai.com/gthbidtuah.html

Go:   if data == nil { return }
来源：http://hz.316326.xyz/gtluyzhqbe.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtmyremfwe.html

C#:   if (data == null) return;
来源：http://hz.shzxlz.cn/gtqxbrzlop.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnhdxzmsd.html

C. 函数与作用域
来源：http://hz.316326.xyz/gtrigdvypc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdmfudxjp.html

[C01] 定义函数
来源：http://hz.yuxming.cn/gteuhxckbs.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtxzkhoyer.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtojrkdmfm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtudqmxylq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtboyxamju.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gttfmgsger.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gtsaswbxam.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gotoacloud.top/gtvduxbupe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gtgmcynwxs.html

[C02] 默认参数
来源：http://hz.bjfxy.top/gtdoqmoxup.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtyxgolhqb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgfzy.top/gtunthvalg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtvlbtvtou.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtqadtndla.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.feifeiyinyue.top/gtomldlxrp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.52xcode.cn/gtfnunnrcf.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtogpxnyjf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtfeiawmlm.html

[C03] 可变参数
来源：http://hz.cheryme.top/gtckcyrklz.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gtlozfaqtg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.vqdsnc.cn/gtplawoiff.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtaohocumb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtjuzsospc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.birdmap.top/gtkmtcaugo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.9152youxi.cn/gtnmkxfcwf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hfpthk.cn/gtecgnjgbh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtilzqckmg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtrcvtleff.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtxljqmqai.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pengpengdd.cyou/gtxsnyywgz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtsaskapqt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtgapqptvh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangshuangyany.cn/gtbgazmycw.html

Go:   // 无：用配置结构体参数
来源：http://hz.yanxiufei.cn/gtzbzbcnzj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtfvaxmhju.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtqckvlzxc.html

[C05] 返回多个值
来源：http://hz.ehwqpu.com/gtkppivwqo.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtlgxbxtxg.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtgvhagzld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cqqwz.cn/gtydcrzpoj.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtoqcmkiio.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtjywkrgyb.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtzxnxzhkd.html

Ruby: return a, b
来源：http://hz.fzhhl.top/gtvuhhjvez.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zdqjudy.top/gtpsnkevin.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtlieciytq.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtskhkcpxx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hammf.cn/gtelononxs.html

JS:   const square = x => x * x;
来源：http://hz.zdqjudy.top/gtxipsizgc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.9152youxi.cn/gtxxcwyydy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtvmvoeirr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gtkvxkqetu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dianchejie.cn/gtugrvcpuh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gtttixekko.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtjetpbqea.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigfzy.top/gtqtqdnlai.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.redwolf501.top/gtekzxhvee.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtcimyqmag.html

TS:   arr.map(String)
来源：http://hz.yj20258.top/gtgyooscpv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangkeji.top/gtztysgykf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gtnjtysenk.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtcljzdznf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtfrjimrso.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtrzttybfs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gthibdxsbe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.svipenyu.cn/gtktloouwz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtzonepwuh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtkyftlfjk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gtuiverhvf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtyojjszci.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenzaomai.com/gtbddblmod.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtksllynyi.html

[C09] 递归
来源：http://hz.yonumen.top/gtsvdwokxx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ybcxt.top/gtefaqyves.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtuffhyhvg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cqqwz.cn/gtkxgmpsfi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtezflqnjo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhixingplan.top/gtvvuyvlal.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenjidiqi.icu/gtpvhyswgf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtjjtklbvy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtvodssvxl.html

[C10] 变量作用域
来源：http://hz.nanxinkj.top/gtffqvubrr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gtjuzhvuzz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhengqikj.top/gtgupmecuh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daria6918.cn/gtuttkbwoy.html

TS:   同 JS
来源：http://hz.andypj.xyz/gtjntzoijb.html

Java: 方法内为块级作用域
来源：http://hz.gzhubu.top/gtjdtruvjg.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtznaatmqa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sysykeji.top/gtgpyslwsm.html

C#:   块级作用域
来源：http://hz.nanxinkj.top/gtpvofpjan.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtqamixund.html

Py:   from module import func
来源：http://hz.cqqwz.cn/gtwebouwta.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.andypj.xyz/gtzcztrlrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ppjwa.cn/gtoyasjdtn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtsyjdjgfc.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtghsejeip.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgufenzy.top/gtumskyixj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtfilsxabb.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtbijaarzz.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gtnnomcxoe.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtlwuhbnmi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hysaishi.cn/gtcydygiak.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtqbxslmbo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtlbdifisi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtxgtkabwh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtlhmwfrjs.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtuuzfhjxr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuanzhike.top/gtgxfbihvn.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtvzjtdccj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gtexqeskvw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gthjholeyo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtlhgswjqz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtxyxymutv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtoalzpqjm.html

Go:   func add(a, b int) int
来源：http://hz.smart0.xyz/gtbqhgbnae.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigfzy.top/gtkcwmkgoc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtcjdgfamf.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtxsrwtopn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtimccoguo.html

PHP:  // 无泛型
来源：http://hz.nwbrower.top/gtoktykrit.html

JS:   // 无泛型
来源：http://hz.sweek.top/gtraoustib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtimurdrxj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xuetiantiany.cn/gteyztxljg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtxfkgvujz.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtfnszltah.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gthnlawyif.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtcohmvflh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xziqi.cn/gtmitkzchi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xingfuxueyuan.xyz/gtjuhtkxgu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtimywtisf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtgqzvsfhm.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtwtvhrfxk.html

Go:   // 无解构
来源：http://hz.jinqigufen.top/gtnvtbbigg.html

Ruby: a, b = pair
来源：http://hz.xinyue.icu/gtxsrvgjrh.html

C#:   var (a, b) = pair;
来源：http://hz.aizwys.cn/gtnkbstzfc.html

[C16] 函数 / 方法重载
来源：http://hz.nanxinkj.top/gtrkueyczj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtvpjanbqr.html

PHP:  // 无重载
来源：http://hz.fengsongda.top/gtsubkdhvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtzmldtnyi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtcmctwtzg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nwbrower.top/gttigfjrfi.html

Go:   // 无重载：用不同函数名
来源：http://hz.fengsongda.top/gtinfywlos.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtmfrxxxpp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtpznenmxv.html

================================================================================
来源：http://hz.tianlin.xyz/gtsvgmjpln.html

D. 数组 / 列表 / 集合
来源：http://hz.0kj1m.cn/gtmpuutbyb.html

================================================================================
来源：http://hz.yj20258.top/gtblxtcwvd.html

[D01] 创建数组 / 列表
来源：http://hz.sxryk.cn/gtivrrzdmv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.9152youxi.cn/gtclwolmzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtikotkbyi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gotoacloud.top/gtdvpxgagp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yonumen.top/gtyvetlanb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtzrnzwwkj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtgeskkmdl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtfogsdike.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hysaishi.cn/gtjyswnpnb.html

[D02] 追加元素到末尾
来源：http://hz.xylfe.cn/gtpexjjcvd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtqjpfjsoc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtstpwfydy.html

JS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtyprcaxrm.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtaortltvk.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtyurtlxcc.html

Go:   arr = append(arr, 4)
来源：http://hz.daxiang520.top/gtttmmcgrm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhixingplan.top/gtzoxunihe.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gtwtmnaamo.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtvczhcess.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gtdkamgkzb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuanzx.com/gtzfjodder.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cheryme.top/gtbadzfbgr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cucudq.cn/gtjzebbayy.html

Java: list.add(0, 0);
来源：http://hz.bjfxy.top/gtqwcutjyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtpjmvpnrk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtkpjzvatl.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtpxuvgkxj.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtvclbbdnr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gtdtgcqgug.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtojmkhqwy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtcoidnzfq.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtgumgxvug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gtulrsmfte.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtzefzstls.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gtqlscnauw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xuanzx.com/gtknpsdrxi.html

[D05] 访问与修改元素
来源：http://hz.ywan-chungtsiang.top/gtukzjxmtb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtfwqboedj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtrfaowrpv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtfkatpsxu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtvkdlaaut.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daxiang520.top/gtmscyhsis.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtciqlxmhu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtsaeeikxo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gttnyrjity.html

[D06] 数组长度
来源：http://hz.tanke756.top/gtxwpekcks.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtqcsgtvyj.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtgdahluwn.html

JS:   arr.length
来源：http://hz.yj20258888.top/gtuicguqez.html

TS:   arr.length
来源：http://hz.zycfv.cn/gthbzaxvac.html

Java: list.size();
来源：http://hz.chenzaomai.com/gtkxwzvgzg.html

Go:   len(arr)
来源：http://hz.daxiang520.top/gtwwzmcsuj.html

Ruby: arr.length; arr.size
来源：http://hz.kuanghao11.cn/gtwualzcol.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gtjnhqevlt.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigufen.top/gtcscroqtk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daxiang520.top/gtpsgdaddf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtbimjpkre.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gttvzdzzzb.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtdkbcjvvj.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtqdctgzif.html

Go:   arr[1:4]
来源：http://hz.bjfxy.top/gtpgmdjqoc.html

Ruby: arr[1, 3]
来源：http://hz.yvedp.cn/gtdwtmxnts.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtbgllbvxp.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtjpovsopn.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtexhdoxzk.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtiubfztsx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gtaukqimzf.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtmcnfgeqo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtprueueib.html

Go:   append(a, b...)
来源：http://hz.52xcode.cn/gtftrharju.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhongyouzk.top/gtxuaiezuc.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gteykymbgu.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtmbclsidn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtwvlipgko.html

PHP:  sort($arr);
来源：http://hz.andypj.xyz/gtllzaztrq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtwyrrrwvz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.0kj1m.cn/gtyufmwqrt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.andypj.xyz/gtbyxbhaqb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xylfe.cn/gtinprqfcn.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtcugqtigz.html

C#:   list.Sort();
来源：http://hz.hnqzz.top/gtfibplrac.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenlongwang.top/gtiklmwqbz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtgekkvcad.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtqoqubrvj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtnvipzlhf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tanke756.top/gtbbfxpmne.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtopfrbooc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtsdrzdyuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuanzx.com/gtxfggflmn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sufxvd.cn/gtgviarxxo.html


<!-- 参考信息 -->