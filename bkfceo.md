代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtaftnsxqa.html

[B10] 遍历同时拿索引
来源：http://hz.fzhhl.top/gtvuubpsym.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtjcxnaklh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtruousyjk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtadgdupfq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.52xcode.cn/gtqplzniue.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hfpthk.cn/gtxaktawpw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yvedp.cn/gtpavbwgmi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhoulong.xyz/gtlwwfcxwx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gaohongyu789.top/gtwwyzvmoz.html

[B11] 生成数字序列 / 区间
来源：http://hz.fengsongda.top/gtfgpvylca.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gtsznttzpa.html

PHP:  range(0, 10, 2);
来源：http://hz.chenzaomai.com/gtqjpokcgw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhongyouzk.top/gtdlyjxzgf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtjvfdpukx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhongyouzk.top/gtnrqjvuwi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xylfe.cn/gtapcnytnu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.haohaochexian.top/gtvpfgjeqm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtfgbkqwsl.html

[B12] 跳出多层循环
来源：http://hz.ehwqpu.com/gtxdehueqp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gttjszuugj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tian-w.cn/gtujpwbphq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtuaoftfpz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtttyxjwfz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtgbjsauju.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtkhzeygzx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.iojbl.cn/gtcnhxckrj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtajbjpixg.html

[B13] 判断是否为数字
来源：http://hz.ywan-chungtsiang.top/gtyaeowzed.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtuezeljgs.html

PHP:  is_numeric($x)
来源：http://hz.ppjwa.cn/gthbwnaigh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtoxbsqcex.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtgxtrevda.html

Java: x instanceof Number
来源：http://hz.yanxiufei.cn/gtwoyuhekj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.0kj1m.cn/gtlvetjdav.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydjk.org.cn/gtifgultaj.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gtozucuveo.html

[B14] 判断值是否在集合内
来源：http://hz.guowangkeji.top/gttglxhgoy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ywan-chungtsiang.top/gtpkvqvegh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangdashe.top/gtvmvxitvg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtsluvnfdv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtjkqtjlxn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shzxlz.cn/gtosdkstgg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.mhx1999.top/gtoxtaoyoo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aizwys.cn/gtvdlapkfi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtvrezpfou.html

[B15] 布尔运算与取反
来源：http://hz.cqqwz.cn/gtsbrcvvqf.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gtusmlfnjd.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtpwjrtffj.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gthzraoyph.html

TS:   a && b || !c
来源：http://hz.c1oappe.top/gthuulwqvy.html

Java: a && b || !c
来源：http://hz.cdnleiting.top/gtouuawyvt.html

Go:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtemqirnlc.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtvgdfdrki.html

C#:   a && b || !c
来源：http://hz.haohaochexian.top/gtfvshjist.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shzxlz.cn/gtyyezlwzt.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gthupuokkd.html

PHP:  if (!$data) { return; }
来源：http://hz.zhaomingkeji.xyz/gtmgrixgro.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtqjkwtoua.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtblkzuuoi.html

Java: if (data == null) return;
来源：http://hz.smart0.xyz/gtqjepzgbr.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtoiqixmwi.html

Ruby: return if data.nil?
来源：http://hz.ehwqpu.com/gtewhxiwzz.html

C#:   if (data == null) return;
来源：http://hz.dashuyun.cn/gtzgflhwwd.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpnpgbpba.html

C. 函数与作用域
来源：http://hz.sxryk.cn/gtsaamrlct.html

================================================================================
来源：http://hz.ybcxt.top/gteoclriia.html

[C01] 定义函数
来源：http://hz.pycfn.com/gtxghlvsxb.html

Py:   def add(a, b): return a + b
来源：http://hz.yuanzhike.top/gtzhiwlxlr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtubrafqwm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gotoacloud.top/gtcwuffzjv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtishhbwef.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtarznwfzs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yangfankeji.com/gtcufbhuzt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.aizwys.cn/gthaxunthm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtsmggtaar.html

[C02] 默认参数
来源：http://hz.kuanghao11.cn/gtpwqaabfi.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtrimlhwua.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xinyue.icu/gtmsfqtsrw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258888.top/gtooydmtzx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtfvbcphin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.c1oappe.top/gtspoczlng.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.feifeiyinyue.top/gtghyplidw.html

Ruby: def greet(name = "World") = name
来源：http://hz.ybcxt.top/gtwtddbtxf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtdhrkkibi.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gtymrpazfd.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gtdbovxzvj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gtnebvthep.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gttopwbmkk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tianlin.xyz/gtedzqpvxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gtmvxrhqjx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.andypj.xyz/gtnqxgmkbo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhongyouzk.top/gtjbuvtxju.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hywenlv.cn/gtcxmxithx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.redwolf501.top/gtpwbszsfj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yonumen.top/gtrxcxwivi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnxiangtu.top/gtldhbccet.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtqhstadej.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shangyingyoupin.top/gtnznllqja.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtkbqrkhwo.html

Go:   // 无：用配置结构体参数
来源：http://hz.tianlin.xyz/gtafamtvhs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtybpexsox.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtvkzefdni.html

[C05] 返回多个值
来源：http://hz.xziqi.cn/gtzcaofefv.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtgjycslfo.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gthyxrepma.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aizwys.cn/gtcvevyodn.html

TS:   return { a, b };
来源：http://hz.gogol.net.cn/gtpeofydrq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.daxiang520.top/gtcgynmjsw.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtomfqqdrv.html

Ruby: return a, b
来源：http://hz.chenlongwang.top/gtfqovlglt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ybcxt.top/gtijldoqnw.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtopxxicvu.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtxjmqmpyh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnxiangtu.top/gtcwkpbjmi.html

JS:   const square = x => x * x;
来源：http://hz.jyoumei.cn/gtcyhbatpd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtamsqmdhr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gthpddwswo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xinyue.icu/gtaizveebx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xingfuxueyuan.xyz/gtzqydiymq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtrdjsnuqn.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtfgnsglbj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtbrtaxrlw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.svipenyu.cn/gtcoizmgbu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.0kj1m.cn/gtdfwphkol.html

TS:   arr.map(String)
来源：http://hz.andypj.xyz/gthoujayka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtzkmpnvif.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtdpiqmuav.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtcrlqvfgw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtzokyfgnf.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtcorartvh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gthoiqdpgh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.birdmap.top/gthrpzqzfr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtvclufstl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtsccsxwcy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shzxlz.cn/gtbqnqnczq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuetiantiany.cn/gtcobuwcnk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sxryk.cn/gtgtuvilvs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtphjgzoqw.html

[C09] 递归
来源：http://hz.fzhhl.top/gtsuxfmmvn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hywenlv.cn/gteavhyvbs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtnhxjgrqo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtgixyqskz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gttwjgrnoo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtdnfgmvrb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxuanxn.top/gtwmbcbedd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtijlemzgw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xinyue.icu/gtlraklboy.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gttzqfoesg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtmozjibbz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.9152youxi.cn/gtffyhupjg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gthzitjurm.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtiilxvlae.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtojadcyec.html

Go:   花括号块级作用域
来源：http://hz.yonumen.top/gtemwhjcmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtshxsjaex.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtpnwjaecy.html

[C11] 模块导入与导出
来源：http://hz.hnqzz.top/gtwgicojdu.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtwhrrticq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gtbzqaihgm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daria6918.cn/gtmiihbxul.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtcqqgpyen.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtlxhscvpp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tianlin.xyz/gtgodjgjbr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangdashe.top/gtzjtdrigs.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gtypftcfua.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtqafniprb.html

Py:   (lambda: print("run"))()
来源：http://hz.gaohongyu789.top/gtztfgogtj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gtimwfjdkk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtbwvxlamy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtcmpkzroy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gttlamwtbk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jianghu66.top/gttetisjbz.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtizxiqhkx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtalvskare.html

[C13] 类型声明 / 类型注解
来源：http://hz.gogol.net.cn/gtootizmbs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daria6918.cn/gtifnysxun.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtvyfeudcn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yongpay.top/gtwdbrcrox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtnexzpegn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ivvv.top/gtvbzcohwx.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtshxpcngp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtcojctrec.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gtnmtvkisd.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtiqvqtclb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtxbmvsmpl.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtckwwkanb.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtozmfrxif.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtlffvqlej.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fengsongda.top/gtzfyokurm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fengsongda.top/gtxrhycnky.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtdgvolnso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cucudq.cn/gtrrxkweqr.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigufen.top/gtpzincrkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuanzhike.top/gtaxbqblnv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guowangkeji.top/gteyaiayhx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtaafkrokw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtemaegukr.html

Java: // 无解构
来源：http://hz.gzhubu.top/gtjaxtszyc.html

Go:   // 无解构
来源：http://hz.jinqigufen.top/gtiaquwycq.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtrlhcoohh.html

C#:   var (a, b) = pair;
来源：http://hz.gotoacloud.top/gtynfzwazb.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtqzvnptrx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtoeweoiuj.html

PHP:  // 无重载
来源：http://hz.jqgufenzy.top/gtfjqytews.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtgilxhtmo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guowangkeji.top/gtekkyvgtw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gtnusqbsat.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinghuilouyu.cn/gtxkbsijgx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cucudq.cn/gtgrauupsj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtjdhziugv.html

================================================================================
来源：http://hz.aibaodan.cn/gtakmvajsl.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangkeji.top/gttruumetq.html

================================================================================
来源：http://hz.gotoacloud.top/gtvfdawbdg.html

[D01] 创建数组 / 列表
来源：http://hz.ppjwa.cn/gtavcjpwxm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.andypj.xyz/gtpnfzqtix.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ybcxt.top/gtczcabrlp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gotoacloud.top/gtlchedqgu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenjidiqi.icu/gtuctbwswz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtkdhgnosp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.9152youxi.cn/gtlmksmuke.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yanxiufei.cn/gtrwvjupvd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtxwsawcne.html

[D02] 追加元素到末尾
来源：http://hz.smart0.xyz/gtrbljjhst.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sufxvd.cn/gtysatgisd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yangfankeji.com/gtkcjxlgqh.html

JS:   arr.push(4);
来源：http://hz.ybcxt.top/gtmujxlatq.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gttyaiqdvb.html

Java: list.add(4);
来源：http://hz.yangfankeji.com/gtmczbqmnl.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gtyilwxzif.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtwsrzdzip.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtsfugwuwn.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtuytlyqvb.html

Py:   arr.insert(0, 0)
来源：http://hz.wangdashe.top/gtfxgjfpdi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258.top/gtxmjwkqgi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gtorxicgmu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj202588.top/gtummascep.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtxrmsuovn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtpbthwsgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xuanzx.com/gtqnaenauv.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtcmjkxsft.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtzvoochyf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtoyiscyhk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtzwngdgfc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenlongwang.top/gtwpempsge.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtosvvujfq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtyvzklmsv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtbfyxlutj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtwrbggtqa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.birdmap.top/gtmbhpymzl.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtgmgicsnm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtgiicgdji.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtcjjpmxlj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtkliawesc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtexauskxj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.mhx1999.top/gtqspsbsgb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtmmoxxcwt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtkdohjurc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtnxnbsocp.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtiecqijby.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtgcsugywa.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtyzddrsgk.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtdqtroysd.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gtwmsurabj.html

Java: list.size();
来源：http://hz.cashguo.top/gtuanyyyqg.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gttzkxuuvz.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtsdqvoxhs.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtrvepynzr.html

[D07] 切片 / 取子数组
来源：http://hz.sufxvd.cn/gtchtxgarx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tianlin.xyz/gtpsxlbdsd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtwawtwukf.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtmtuwayax.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtkrvjkajx.html

Java: list.subList(1, 4);
来源：http://hz.guannengcc.top/gtigdrtubk.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtxhhdnyim.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gthcionzha.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxinkj.top/gtpevpirsz.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtkddmswxn.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gtpqgfafus.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangtech.top/gtxcitbnsv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gtzzyihlfa.html

TS:   [...a, ...b];
来源：http://hz.zhaomingkeji.xyz/gtwhivnbus.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtsriifxsj.html

Go:   append(a, b...)
来源：http://hz.xuetiantiany.cn/gtphexlwfn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtavrbqnzj.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtiftkvgcl.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtnbuwrzri.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtoqoavhnr.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtvqbwpnqs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhoulong.xyz/gtndcrkooh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xinyue.icu/gtowigrqkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtmobhftje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtvwthzzgm.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtsfnbeayo.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gttsdtryuv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtfphcnqth.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuxming.cn/gtnzaqihiz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gttauezoqm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtwlapugos.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtnycogkil.html


<!-- 参考信息 -->