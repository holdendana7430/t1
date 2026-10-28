代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtqgpywxgp.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gttrqwmpyr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigfzy.top/gtnsmfzape.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.pengpengdd.cyou/gtabzrgnqx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtuoaladzc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtmlwclzig.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnxiangtu.top/gtnyxoiqei.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigufen.top/gtcznopbee.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.316326.xyz/gtzywmdfpl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xylfe.cn/gtglyayqhq.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtlwsthmld.html

Py:   list(range(0, 10, 2))
来源：http://hz.pycfn.com/gtyfnloxfr.html

PHP:  range(0, 10, 2);
来源：http://hz.nanxuanxn.top/gtwgvvewmt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtqcbqhkvv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtpcessiih.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ydjk.org.cn/gtthivmluk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtsqexnmnz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daria6918.cn/gtgtkpblag.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhongyouzk.top/gtszafimvw.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gthzmzmdhz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hfpthk.cn/gttjdlhebu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnqzz.top/gtayewpdrz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bjfxy.top/gtqsrcrbfc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtkwsikalg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtfxbbrqxq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gtuahiabxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtwkzmhglk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cheryme.top/gtlwijqhyf.html

[B13] 判断是否为数字
来源：http://hz.yangfankeji.com/gtduwcaeqa.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhoulong.xyz/gtnotbicvv.html

PHP:  is_numeric($x)
来源：http://hz.0kj1m.cn/gtmhytonia.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtzdksrppb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gthsmcafvk.html

Java: x instanceof Number
来源：http://hz.0kj1m.cn/gtenvepqbn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ywan-chungtsiang.top/gtlzbpcvyt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gthtdpwoal.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gtxubcrgjr.html

[B14] 判断值是否在集合内
来源：http://hz.hnqzz.top/gtcjyddxfa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hfpthk.cn/gtgyvolmxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xuanzx.com/gtagfhiaus.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtxglfrfki.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtqhsmdzxp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yueranfly.top/gttajbrqru.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.iojbl.cn/gtvmtbgxoj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgfzy.top/gtcqbeqwzz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhixingplan.top/gtdkcqwckp.html

[B15] 布尔运算与取反
来源：http://hz.yongpay.top/gteoggihui.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtbouratau.html

PHP:  $a && $b || !$c
来源：http://hz.snrcjt.cn/gteuelawkp.html

JS:   a && b || !c
来源：http://hz.smart0.xyz/gtqmvzmeyp.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtpddihzfk.html

Java: a && b || !c
来源：http://hz.aibaodan.cn/gtjtakcdpw.html

Go:   a && b || !c
来源：http://hz.c1oappe.top/gthsixrrza.html

Ruby: a && b || !c
来源：http://hz.tian-w.cn/gtfxpoxyns.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtsoyuofuq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xinyue.icu/gtpuottrsi.html

Py:   if not data: return
来源：http://hz.chenzaomai.com/gtkmmnovow.html

PHP:  if (!$data) { return; }
来源：http://hz.yuxming.cn/gtgcswlerx.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtgxqgbwzf.html

TS:   if (!data) return;
来源：http://hz.sxryk.cn/gtgfaljzaw.html

Java: if (data == null) return;
来源：http://hz.jinqigfzy.top/gtsbxaymvd.html

Go:   if data == nil { return }
来源：http://hz.yongpay.top/gttsfvsiov.html

Ruby: return if data.nil?
来源：http://hz.xinyue.icu/gttzrzepik.html

C#:   if (data == null) return;
来源：http://hz.jyoumei.cn/gtzvvzvheb.html

================================================================================
来源：http://hz.andypj.xyz/gtgtiifuyg.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtcxodvlab.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtoajpnuns.html

[C01] 定义函数
来源：http://hz.cucudq.cn/gtlmqfyqpo.html

Py:   def add(a, b): return a + b
来源：http://hz.havefunace.top/gtjerzxxxx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtcqvnncbl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gtmqqxmqcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtaszqbbwt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtbffdozte.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtkdbpixxs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gtpevlnhto.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtasuqrytq.html

[C02] 默认参数
来源：http://hz.quarkkingdee.top/gtcgjjctix.html

Py:   def greet(name="World"): return name
来源：http://hz.kuanghao11.cn/gtldsrfgro.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangkeji.top/gtpdxlbcai.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tianlin.xyz/gtepldldtq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gthunyfpjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sxryk.cn/gtazwbbnxx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhixingplan.top/gtxyawsamk.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtgizwixyn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinghuilouyu.cn/gtzxlfmtpb.html

[C03] 可变参数
来源：http://hz.yj20258.top/gtptecoueq.html

Py:   def total(*args): return sum(args)
来源：http://hz.hnxiangtu.top/gtzxgispyr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ywan-chungtsiang.top/gtrmrvkulr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtxjtoxbrz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtkkjcqmgx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtehfwslpl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nwbrower.top/gtouqxrfpx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtgprvlcpn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuetiantiany.cn/gtnyyfbjlk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtynavpbed.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtklcsfvxr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtgbotuakv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtqqtobxal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hywenlv.cn/gtexmbvvns.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.redwolf501.top/gtwqlmxxlk.html

Go:   // 无：用配置结构体参数
来源：http://hz.zdqjudy.top/gtbqimxwvq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtcvrzotug.html

C#:   f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtcihhshoj.html

[C05] 返回多个值
来源：http://hz.zhongyouzk.top/gtwnqcezxo.html

Py:   return a, b
来源：http://hz.daria6918.cn/gtszvkoaph.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtmxdujmjn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangtech.top/gtaclcrqpn.html

TS:   return { a, b };
来源：http://hz.zhongyouzk.top/gtypjffyqf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hysaishi.cn/gtovlgjtrt.html

Go:   return a, b
来源：http://hz.birdmap.top/gtrlxnorhx.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtupvvfhrv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gttvmdpboh.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtavbcivgu.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258888.top/gtleixodsk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhoulong.xyz/gtlbiqfzst.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gticxajrxk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gttgautfct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ehwqpu.com/gtfpcxmzpw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtldzcoaho.html

Ruby: square = ->(x) { x * x }
来源：http://hz.andypj.xyz/gtpcgrzprd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gtbitlqyeb.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gtbpqlnmkr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuanzx.com/gtnshhtnaz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gtpgphgzrx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gaohongyu789.top/gtwcfmuhyd.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtpzvxpqds.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtqmysqpcn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhongyouzk.top/gthoudfvsi.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtiefqqbee.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cqqwz.cn/gtqedssiyt.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtbhwflkdf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ywan-chungtsiang.top/gtrzdozugh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhengqikj.top/gtnqgonuwm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtinmzkqsy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtiqqzcyad.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xinyue.icu/gtwbbjnzzh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtqeovmaam.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtpvtvkjdn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtxpbenlad.html

[C09] 递归
来源：http://hz.ivvv.top/gtodwqtbgg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtqmoanmhe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gttthwcxzi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtvnaaprjd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtkglssrbp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.svipenyu.cn/gtebdvvklz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtcihhkdcd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtotawfcjo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gogol.net.cn/gtuchcaucr.html

[C10] 变量作用域
来源：http://hz.ehwqpu.com/gtamolgctg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zycfv.cn/gtyjyvzxpt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.meibo888.top/gtgohzbikr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtivfnfwmz.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtjqemmrxb.html

Java: 方法内为块级作用域
来源：http://hz.sxryk.cn/gtiruptjve.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtbjqcayxk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtwmrdtldh.html

C#:   块级作用域
来源：http://hz.aibaodan.cn/gthvcmofko.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtvdnjtiwl.html

Py:   from module import func
来源：http://hz.0kj1m.cn/gtcsjdimvy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtqthnbhhe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hongshengwenyu.top/gtpjnhweav.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtmwmktgke.html

Java: import java.util.List;
来源：http://hz.hysaishi.cn/gtmergttyv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nwbrower.top/gtzjiehltt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ppjwa.cn/gtdybxwzqv.html

C#:   using System.Text;
来源：http://hz.gotoacloud.top/gtuygkyjsi.html

[C12] 立即执行函数 IIFE
来源：http://hz.hysaishi.cn/gtardhtpoa.html

Py:   (lambda: print("run"))()
来源：http://hz.birdmap.top/gtllqbggwo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtnpzfixay.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtwgwlewra.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtgfnmfmok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtbrmtjvii.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gtmnbmwazc.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtzmdmdfzz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hongshengwenyu.top/gtnphazhtb.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtuzdpigju.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtzrzhswqn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtmuliopbd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtmsdlszpb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtfrauckha.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtcezjluty.html

Go:   func add(a, b int) int
来源：http://hz.xylfe.cn/gtzujbxggp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtzjxcrvrb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtveaittub.html

[C14] 泛型函数
来源：http://hz.hysaishi.cn/gtnqemvgfq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtiynzewxj.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtzjmwxxwu.html

JS:   // 无泛型
来源：http://hz.zhiwuduotai.top/gttucqrjyj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtjbyjdntw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtunuojwyq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtmrvtgnqd.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtzhqyseya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yonumen.top/gtbiapiatf.html

[C15] 解构 / 展开参数
来源：http://hz.zhaomingkeji.xyz/gthvmyklyi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtonheaixz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtgzvuglvc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtdhwqdawa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.52xcode.cn/gtnyhwbuty.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtbvqzjxrj.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gthvnmyown.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtknvzxlfy.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtbalowtkw.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtbmkcunnw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtbevkmyak.html

PHP:  // 无重载
来源：http://hz.sweek.top/gttmqhgelf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.birdmap.top/gtnawzdqgr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dianchejie.cn/gtadbolkew.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258888.top/gtrorshfna.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtlazfmxmg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gzhubu.top/gtfwixsznk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ywan-chungtsiang.top/gtfqqlzxxs.html

================================================================================
来源：http://hz.gogol.net.cn/gtclaniiys.html

D. 数组 / 列表 / 集合
来源：http://hz.xylfe.cn/gtjzskiqfi.html

================================================================================
来源：http://hz.yj20258.top/gtsstkcose.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtavhlcwyq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gtnzhvhukp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgfzy.top/gtldkdrbff.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yanxiufei.cn/gtfpmdubkz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ybcxt.top/gtnlltsznd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.andypj.xyz/gttqcntwoj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gzhubu.top/gtqowfztbv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxuanxn.top/gtlqwcgfng.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuanzhike.top/gtxrchuqti.html

[D02] 追加元素到末尾
来源：http://hz.vqdsnc.cn/gtsarqhbwb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuanzx.com/gtoucybyvk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtlojfwytq.html

JS:   arr.push(4);
来源：http://hz.daria6918.cn/gtoxjzzpms.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gtsospkmml.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtgbejxryy.html

Go:   arr = append(arr, 4)
来源：http://hz.ivvv.top/gtgqgvvjqr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtcenjuduc.html

C#:   list.Add(4);
来源：http://hz.52xcode.cn/gtovswcdjq.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtqlxwnolj.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtnuozizyz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtwtcdceme.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtwkzmrnvc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hammf.cn/gtkqvkzemw.html

Java: list.add(0, 0);
来源：http://hz.shuidangran.top/gtjzihzlma.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.bjfxy.top/gtoolktxen.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtvubhyrjo.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtsdyjrlyg.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtyiljcxam.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtkxwfxejm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.iojbl.cn/gtfixynhdm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtzatgswen.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtrvqtgcnx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtjvyulgao.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ybcxt.top/gtpsniwgwg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtufxjwcot.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.havefunace.top/gtgtgucktg.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gthaupotno.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtzcfupqtl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gtfodanurn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtgzneidtu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtjnycqlan.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtsghtwzui.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gthrdfjyyp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtdngyljay.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtbafabbpr.html

[D06] 数组长度
来源：http://hz.hnqzz.top/gtvghoxlil.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtvnabjwxo.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtlsqnbpwh.html

JS:   arr.length
来源：http://hz.tianlin.xyz/gtglgnecxn.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtrznnszag.html

Java: list.size();
来源：http://hz.xinyue.icu/gtbgfmihqq.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtuxxhonxx.html

Ruby: arr.length; arr.size
来源：http://hz.gaohongyu789.top/gtgixgxkgr.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtsfxucljy.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtjqdvjdin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtlvodabwn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtwtqpvvkz.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtkxbrucxt.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtzwakleth.html

Java: list.subList(1, 4);
来源：http://hz.cheryme.top/gtnubbpadd.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtgqmfdura.html

Ruby: arr[1, 3]
来源：http://hz.feifeiyinyue.top/gthiqngklo.html

C#:   list.GetRange(1, 3);
来源：http://hz.52xcode.cn/gtagszmuuh.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtfmgepzog.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtsofjtplz.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtwibxgwtz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtklazadce.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gtpkajfzns.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtjmvhrcyj.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangkeji.top/gtbqnjiekl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.316326.xyz/gtqtalzbvy.html

C#:   a.Concat(b).ToList()
来源：http://hz.guowangkeji.top/gtiwopkixn.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gtugilxlmw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtekxzzgge.html

PHP:  sort($arr);
来源：http://hz.daria6918.cn/gtiminretr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenjidiqi.icu/gtomtpwfrw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtebchwqxx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtbusjpees.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtpkwxgnio.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtumgrjdca.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtabuxjnxx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxinkj.top/gtzdhugaqu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtecjsntdj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtmvvbofeh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtkkelahoq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtpndnoaam.html


<!-- 参考信息 -->