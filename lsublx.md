代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtlcemdwyf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.bjfxy.top/gtlvcvkyqi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xuetiantiany.cn/gtfmpgjtrd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenzaomai.com/gtqeobxojd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guannengcc.top/gtpzpggliq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daxiang520.top/gtugqgeben.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtpziyxsyo.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtlncieqic.html

PHP:  range(0, 10, 2);
来源：http://hz.xingfuxueyuan.xyz/gtyueinkvb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtbibqfmyv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtdfppxjgu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtwdnatkcs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gttzinlpnz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhaomingkeji.xyz/gtvoivwiaj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hongshengwenyu.top/gtfvqucgqt.html

[B12] 跳出多层循环
来源：http://hz.aizwys.cn/gtehzkbdxm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.guannengcc.top/gtcbssbozl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dashuyun.cn/gtfkgavhco.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtrpykudyq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gttgsrnwoi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtpwnmooyu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangdashe.top/gthliwuans.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yueranfly.top/gtnfuzcbdf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtfalrkolf.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gttdtooecb.html

Py:   isinstance(x, (int, float))
来源：http://hz.xylfe.cn/gtincsckml.html

PHP:  is_numeric($x)
来源：http://hz.dianchejie.cn/gtkhybpgya.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtqiyhtfnp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtlcuptwke.html

Java: x instanceof Number
来源：http://hz.xziqi.cn/gtaeahzpbc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gtxxlkcdvz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yangfankeji.com/gtwjcwzvvl.html

C#:   x is int or double or decimal
来源：http://hz.sysykeji.top/gtzmpdxipe.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtbevajipg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtanavibfe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.snrcjt.cn/gtcpogwock.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtpisiekzn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hywenlv.cn/gtyakjbnbr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guannengcc.top/gtrlicblue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yongpay.top/gtxowuorwx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnxiangtu.top/gtqefwnmls.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangshuangyany.cn/gtviilvgpc.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gtugtsiyhq.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtrjgmpqxq.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtxqubdwvj.html

JS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtxrkzixku.html

TS:   a && b || !c
来源：http://hz.zycfv.cn/gtxwzdrmoi.html

Java: a && b || !c
来源：http://hz.sysykeji.top/gtighmwqha.html

Go:   a && b || !c
来源：http://hz.cashguo.top/gtafhjonux.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtzmmmhtcx.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtprgrktgn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtwngivxfp.html

Py:   if not data: return
来源：http://hz.yuxming.cn/gthokuspyp.html

PHP:  if (!$data) { return; }
来源：http://hz.52xcode.cn/gtxwefqfyv.html

JS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtkxqpvesp.html

TS:   if (!data) return;
来源：http://hz.tanke756.top/gtiogtqdvj.html

Java: if (data == null) return;
来源：http://hz.ybcxt.top/gtrgeheldp.html

Go:   if data == nil { return }
来源：http://hz.aizwys.cn/gtbgxgfvmv.html

Ruby: return if data.nil?
来源：http://hz.hysaishi.cn/gtzoatrtwu.html

C#:   if (data == null) return;
来源：http://hz.jqgufenzy.top/gtxxgrwwhv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtoklzaegy.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtsulwfpjh.html

================================================================================
来源：http://hz.xylfe.cn/gtjiovkgev.html

[C01] 定义函数
来源：http://hz.yongpay.top/gtjsnslwpn.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gtkodpkvae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtyyafymwd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.smart0.xyz/gtjcwcdcpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtcdttfhwc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtopjpvptj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cdnleiting.top/gtsftrszyx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ywan-chungtsiang.top/gtpcgjlali.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gthginzsdb.html

[C02] 默认参数
来源：http://hz.hnqzz.top/gtoxbjrztr.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gternrulkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhoulong.xyz/gtilikcoid.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtixsplehz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gtqmorhukh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.feifeiyinyue.top/gtuudfsvan.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxuanxn.top/gtwcywrhao.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtealjzxhw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhoulong.xyz/gtlvhsaxgh.html

[C03] 可变参数
来源：http://hz.gotoacloud.top/gtrbwephod.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtiatmbttb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtgjmqvbie.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtbslwlpeg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gttncbhcjc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhijiandao.cn/gtcnrobijy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtiosfpasv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtoqjllpaq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxuanxn.top/gtqpcsacbv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gtmnwkqept.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtxnmitxik.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtbjxclcoa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.haohaochexian.top/gtfzlcoxrx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinyuanbaomall.cn/gtdincmxuu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtmgklrgfa.html

Go:   // 无：用配置结构体参数
来源：http://hz.smart0.xyz/gthxjjtadh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtxnbhtvgt.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtsjonjdpl.html

[C05] 返回多个值
来源：http://hz.zycfv.cn/gtpexcdwnp.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtilmqwtle.html

PHP:  return [$a, $b];
来源：http://hz.jlsjyb.cn/gttjltgkpf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.svipenyu.cn/gtwqihptgs.html

TS:   return { a, b };
来源：http://hz.shangyingyoupin.top/gtjiiszszh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.daxiang520.top/gtmxsgecbs.html

Go:   return a, b
来源：http://hz.guowangkeji.top/gtwxjszwbx.html

Ruby: return a, b
来源：http://hz.tanke756.top/gtvilorooh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtwdpkdrug.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtcxzakvdb.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtveidcowd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.quarkkingdee.top/gtjgxvspqa.html

JS:   const square = x => x * x;
来源：http://hz.yuxming.cn/gtrnzumful.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gtxkdkssob.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtovwmzqyh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yvedp.cn/gtwlagsplx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinyuanbaomall.cn/gtgvbqekjb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yongpay.top/gtmppsayoo.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gtbbkgzjmv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtguxrrcqq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gteqimmbqd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuanzx.com/gtozleygfw.html

TS:   arr.map(String)
来源：http://hz.zhongyouzk.top/gtpzolxdrj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.feifeiyinyue.top/gtvcxsecsb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sysykeji.top/gttesctxtk.html

Ruby: arr.map(&:upcase)
来源：http://hz.hongshengwenyu.top/gtexctypkt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtymjhvugl.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gtfemfitrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gtwxchmksb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hywenlv.cn/gtwbcxsufj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtrqkzcpty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gthkboljrg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nwbrower.top/gtlsaoaubl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtamrkagxz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtgshbtvbw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtcnhetgft.html

[C09] 递归
来源：http://hz.nwbrower.top/gtpyrsrqds.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtqyxnqnbx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ivvv.top/gtgfrjkpmg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cqqwz.cn/gtugnxkgyt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtsqqtsvtq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yongpay.top/gtcwaicowk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinghuilouyu.cn/gtwkyylmjn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtpgaxdvmj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.c1oappe.top/gtvvlkxbso.html

[C10] 变量作用域
来源：http://hz.yongpay.top/gtsmcanczp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtbpcjokof.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.birdmap.top/gtlgfcplvf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gttjkrllrc.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtszzitnso.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtmmyxrpoz.html

Go:   花括号块级作用域
来源：http://hz.cheryme.top/gtpqqtoppg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sxryk.cn/gtsksdimua.html

C#:   块级作用域
来源：http://hz.hywenlv.cn/gtecevluyo.html

[C11] 模块导入与导出
来源：http://hz.hywenlv.cn/gtenyblfbx.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtmndelafv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtvdadyxhu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yonumen.top/gtgzhblzby.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gtyonjbink.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtisqvbaxv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtnxpwkjri.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtcbomsgbj.html

C#:   using System.Text;
来源：http://hz.daria6918.cn/gtfxncebdo.html

[C12] 立即执行函数 IIFE
来源：http://hz.birdmap.top/gtxurcfypy.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtncmbblru.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtmtwptiqa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtlzseilye.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtteyahmmm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtqbwknubw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhoulong.xyz/gtvlceletu.html

Ruby: -> { puts "run" }.call
来源：http://hz.zdqjudy.top/gtgdgsngcc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guannengcc.top/gtycfwppvt.html

[C13] 类型声明 / 类型注解
来源：http://hz.c1oappe.top/gtutdrroxo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtstvqbzfz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtjezlwpvj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtkrleuslc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtrteampke.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gttijvjtbj.html

Go:   func add(a, b int) int
来源：http://hz.pycfn.com/gtmlzozdbp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.haohaochexian.top/gthsiszpwn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cashguo.top/gtfssywqeg.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtesdhlxyg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtfklzxlcn.html

PHP:  // 无泛型
来源：http://hz.cdnleiting.top/gtjsfjtlna.html

JS:   // 无泛型
来源：http://hz.dianchejie.cn/gtzscjrzwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.smart0.xyz/gtcuejkhbf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtshcgtjap.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtafuinhlg.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtpzvlndgc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtfqgxbzzk.html

[C15] 解构 / 展开参数
来源：http://hz.nanxuanxn.top/gtqovayeqi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtuaiopera.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtijenbhkj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtsblgwruh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtibwmmkgx.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtpuzyonbd.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtwsclvzih.html

Ruby: a, b = pair
来源：http://hz.pycfn.com/gtyzwxsumk.html

C#:   var (a, b) = pair;
来源：http://hz.mhx1999.top/gtjwijzmtw.html

[C16] 函数 / 方法重载
来源：http://hz.hnxiangtu.top/gtopafuwzv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gtwlxxbani.html

PHP:  // 无重载
来源：http://hz.yanxiufei.cn/gtcthgyykf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.snrcjt.cn/gtmxpsubaf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtkuvbdbep.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtdlsukjjd.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtiffsrwyg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtjpyryftx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtsboqksti.html

================================================================================
来源：http://hz.ivvv.top/gtgizxkpax.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gtafxdsdto.html

================================================================================
来源：http://hz.yj20258.top/gtqfzptkdy.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtidfmtcos.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtjbpncaqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtxxirwwkw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gtiawwxmgj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtzbzknbye.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtqkstdrqb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydjk.org.cn/gtomerfvxc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtxjhjcill.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gotoacloud.top/gtfkvjudts.html

[D02] 追加元素到末尾
来源：http://hz.xinyue.icu/gtnzdsmksb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gtcwyisyoz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tian-w.cn/gtteagxfiy.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtjdcpqyaf.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtsryuuzxs.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtbsftzyvc.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtpzdyjoxz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtiigzduas.html

C#:   list.Add(4);
来源：http://hz.daria6918.cn/gtjouqxjnj.html

[D03] 在指定位置插入元素
来源：http://hz.cqqwz.cn/gtivrzbuyf.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtqilebgwc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtwsarhsyw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtyhkepbmv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtkpxwkibu.html

Java: list.add(0, 0);
来源：http://hz.jyoumei.cn/gtqhakekay.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtzltndcec.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtqttcpxav.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtyqxhwfls.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gttrraehhr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sxryk.cn/gtlzptiplh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtciarepvm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhaomingkeji.xyz/gtesnwzyek.html

TS:   arr.splice(0, 1);
来源：http://hz.cqqwz.cn/gtuskduyoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gttfqaaqog.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtnzbbiatw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gtxxkcucyv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtngndsdoc.html

[D05] 访问与修改元素
来源：http://hz.ydzc1.top/gtmlkttaik.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtdargngds.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gtreghsiai.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tianlin.xyz/gtiyixcwep.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fzhhl.top/gtlhleygmc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtahhbpwrs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtyhamwmvc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtmdixhxvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtgkeficfv.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtwkuznkwi.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtvggbuwnx.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtkdfoeknp.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtgyfnegqx.html

TS:   arr.length
来源：http://hz.aizwys.cn/gtbjscxkib.html

Java: list.size();
来源：http://hz.nanxuanxn.top/gtpkqtbzlo.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtdaqpovfl.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtodaxksga.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtwimfrasc.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtogbrdope.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtjbkyswre.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtnkaoeyjo.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtbzszijva.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtszdchydu.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gtcfnwlidi.html

Go:   arr[1:4]
来源：http://hz.c1oappe.top/gtnihheskw.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtipjfdecd.html

C#:   list.GetRange(1, 3);
来源：http://hz.fzhhl.top/gtkiswchbb.html

[D08] 合并两个数组
来源：http://hz.smart0.xyz/gtzgsrnrvb.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gttnalletn.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtszfgekvr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtitzpuqxt.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtgmjieofj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtdwlugsch.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtctoqpxrs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtbceomvyh.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtgkmgtvqq.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtbrhmhoym.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gtabwjglwm.html

PHP:  sort($arr);
来源：http://hz.cheryme.top/gtcjvptswl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gtkcdcciki.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtygfsdnuf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuxming.cn/gtauwthtcn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtnwvsmrcd.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtnotqwoyd.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtpkskcunu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gthadxfhsv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.kuanghao11.cn/gtcwefintn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtonadlxjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtzaibhtaw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gtugdltrik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtiwofnjwa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.9152youxi.cn/gtzqjrrwho.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtdftlbrzv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sysykeji.top/gtfgjsjpud.html


<!-- 参考信息 -->