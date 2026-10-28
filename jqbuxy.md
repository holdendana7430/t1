代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sweek.top/gtgrxnjiua.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhixingplan.top/gtfsvzhxsv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtcrjxidyc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinyuanbaomall.cn/gtilujwymj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hysaishi.cn/gtudlfmbdw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tanke756.top/gtjozizyjd.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtrmjhwmay.html

Py:   list(range(0, 10, 2))
来源：http://hz.0kj1m.cn/gtgiokvyzc.html

PHP:  range(0, 10, 2);
来源：http://hz.zdqjudy.top/gtcbqhjczv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtmpgcwkrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtreudakzf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sysykeji.top/gtufpsuoia.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ivvv.top/gtwbxzvmra.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daxiang520.top/gtxpgmxfia.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gtefcusscp.html

[B12] 跳出多层循环
来源：http://hz.dashuyun.cn/gtpbswxszm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yangfankeji.com/gtezbsqtwl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.0kj1m.cn/gtufbskjrz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtduwbfvyu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gttykvdonw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtsadmfxcf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cqqwz.cn/gtmqndhrpq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhoulong.xyz/gtlqliivob.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jlsjyb.cn/gtmpalnrke.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtxjckwrxe.html

Py:   isinstance(x, (int, float))
来源：http://hz.yongpay.top/gtdhmeizjl.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtyuifxhkt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.haohaochexian.top/gtjsiawfso.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtswnbadku.html

Java: x instanceof Number
来源：http://hz.ydzc1.top/gtlqrbwfbv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtzwfcyced.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtdpjsvkdd.html

C#:   x is int or double or decimal
来源：http://hz.jqgufenzy.top/gtkzpbfwon.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gttlwbueor.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtlncivrze.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sufxvd.cn/gturdjcnsc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtxlobvbyx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtarwqvkuo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydjk.org.cn/gtekjsuier.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhoulong.xyz/gtxxkeahna.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhengqikj.top/gtdhjiszuj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yanxiufei.cn/gtkooeyfyg.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtjqjremgh.html

Py:   a and b or not c
来源：http://hz.meibo888.top/gtojqxcniv.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtghoodrsd.html

JS:   a && b || !c
来源：http://hz.fzhhl.top/gtlakeneye.html

TS:   a && b || !c
来源：http://hz.guannengcc.top/gtkzeuwtot.html

Java: a && b || !c
来源：http://hz.yanxiufei.cn/gtfvyurewq.html

Go:   a && b || !c
来源：http://hz.yvedp.cn/gtlbjschwd.html

Ruby: a && b || !c
来源：http://hz.guowangkeji.top/gtwchncqke.html

C#:   a && b || !c
来源：http://hz.nanxinkj.top/gtzeszsyoe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tian-w.cn/gtapkegfyt.html

Py:   if not data: return
来源：http://hz.zhiwuduotai.top/gtepzujmad.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gtlmrwvbrb.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtzhqzkbez.html

TS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtfdxxdmbt.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtuxfgoldd.html

Go:   if data == nil { return }
来源：http://hz.hammf.cn/gtcvdzepak.html

Ruby: return if data.nil?
来源：http://hz.pycfn.com/gtxcleqrcy.html

C#:   if (data == null) return;
来源：http://hz.sxryk.cn/gtnynnrgdi.html

================================================================================
来源：http://hz.redwolf501.top/gtpicswikd.html

C. 函数与作用域
来源：http://hz.ybcxt.top/gtvgqoelld.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmtpqovir.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtevrzyntu.html

Py:   def add(a, b): return a + b
来源：http://hz.yonumen.top/gtcuwmpuuj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gttqlwtgeu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtlfngthzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtzbclxfaf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtkmoqmryf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ehwqpu.com/gtkmxcxiip.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jyoumei.cn/gtryrbhfvn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtergsbuun.html

[C02] 默认参数
来源：http://hz.xziqi.cn/gtvkkrjran.html

Py:   def greet(name="World"): return name
来源：http://hz.jianghu66.top/gtvhranadw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydzc1.top/gtvxjuualo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtkbpedqpm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cheryme.top/gtmsqvxzgv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.vqdsnc.cn/gtdyhfwsaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tian-w.cn/gtduktnrts.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gtfgsmslnc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnqzz.top/gtnpkqjoif.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gttsoznqbo.html

Py:   def total(*args): return sum(args)
来源：http://hz.zdqjudy.top/gtsutnprku.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtnwumrbgl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtshgjvteu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtsclgvlxx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.feifeiyinyue.top/gtzyjzjclt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtwtxvjrso.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtqnaehhbs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtflhcomgc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenlongwang.top/gtkfdbjyvh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtlzuhlaxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yanxiufei.cn/gtumydrqgo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtgzyudfft.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxuanxn.top/gtbtxbafyz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tian-w.cn/gtwkrbzbrt.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtkernetrg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtbdyrxswy.html

C#:   f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtysklcnii.html

[C05] 返回多个值
来源：http://hz.sxryk.cn/gturpzlrwm.html

Py:   return a, b
来源：http://hz.ybcxt.top/gtwskpidbh.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gtxnzzdgxs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtwcdydkuy.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtryqphgqd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gtqigqdzfg.html

Go:   return a, b
来源：http://hz.bjfxy.top/gtxutkjtrx.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtjbtkwijt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtvbrvmdiq.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gtwcixuyqu.html

Py:   square = lambda x: x * x
来源：http://hz.pengpengdd.cyou/gttjrdfwwf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tianlin.xyz/gtvrubwrff.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtymgdlral.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.tanke756.top/gtvmlbsaok.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jiagoushi.top/gtulmneizs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtvnafqmde.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dianchejie.cn/gtuqpgshnb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtsvjiaezr.html

[C07] 把函数作为参数传入
来源：http://hz.zhaomingkeji.xyz/gtopziqvzl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ppjwa.cn/gtvzolqwzw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nanxinkj.top/gtyieidwfm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtdaummgkj.html

TS:   arr.map(String)
来源：http://hz.hysaishi.cn/gtdobdgtjx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gtxfteyhfi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hongshengwenyu.top/gtvmfzrudj.html

Ruby: arr.map(&:upcase)
来源：http://hz.hammf.cn/gtxmxidtqy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hongshengwenyu.top/gtntllshqf.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gthphncjvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtilcewind.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtstwowpnp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gticrsajbn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gthajkbmnz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gtvsdvbhnq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gtfliyibip.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aizwys.cn/gtkdvmzosp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtglryxyzk.html

[C09] 递归
来源：http://hz.pycfn.com/gteyszphzn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtmowodlvy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gtnbcigece.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtfdflzseb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ybcxt.top/gtilvkrtqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtbadkgadi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtlnhnahxy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtedjfauqs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gttaqrahzm.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtfqpezerg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gtcqwlysso.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.316326.xyz/gtwypxeabb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dianchejie.cn/gtziyspwcg.html

TS:   同 JS
来源：http://hz.yj20258.top/gtpptnynsa.html

Java: 方法内为块级作用域
来源：http://hz.cdnleiting.top/gtlspoazuy.html

Go:   花括号块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtfaveotty.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gthgcpdfia.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtdkormuxk.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtvoqtcgsl.html

Py:   from module import func
来源：http://hz.cqqwz.cn/gtpblmlqgm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sysykeji.top/gttfhdxmph.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.birdmap.top/gtbnaqewdn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtbmqsgseo.html

Java: import java.util.List;
来源：http://hz.jinghuilouyu.cn/gtcjrogquz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fengsongda.top/gtjncyeptv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gtuppvnbtk.html

C#:   using System.Text;
来源：http://hz.meibo888.top/gtasonvktg.html

[C12] 立即执行函数 IIFE
来源：http://hz.guannengcc.top/gtgirkmevi.html

Py:   (lambda: print("run"))()
来源：http://hz.cashguo.top/gtugdmbgwx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtjlhqgzch.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtnyaybhhl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtlxcrdjic.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gthyebszoc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tianlin.xyz/gtayqkmyle.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gtrjshbyay.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtvzanuraw.html

[C13] 类型声明 / 类型注解
来源：http://hz.ehwqpu.com/gtexclkldh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gtcbzqxepv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtbfzgncxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxuanxn.top/gtwokirkrh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtbeeuagfm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtqulsgoes.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtpfdodwnt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtqyfldpla.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.andypj.xyz/gtoajbbzhx.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtpriuvocj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gtscjkrjvz.html

PHP:  // 无泛型
来源：http://hz.daxiang520.top/gtnafpvcmb.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gtvkvwpnjj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhiwuduotai.top/gtyxulksdu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtcihsogkb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jianghu66.top/gttmlydqah.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtiakuoatb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtlddfjtvj.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtpnjzcgfe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shzxlz.cn/gtkqqvtyqg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daxiang520.top/gtjpakbuos.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gttnwnitny.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xylfe.cn/gthjzkquks.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtstpsvrcw.html

Go:   // 无解构
来源：http://hz.zhoulong.xyz/gtcqczxpgp.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtohedsuzu.html

C#:   var (a, b) = pair;
来源：http://hz.shzxlz.cn/gtvzgsmayu.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtzzlcnnml.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtmzbinhaz.html

PHP:  // 无重载
来源：http://hz.gzhubu.top/gtxmduafwr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtjsafoukc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shzxlz.cn/gtifjzloic.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gthdauonpe.html

Go:   // 无重载：用不同函数名
来源：http://hz.gogol.net.cn/gtaepdskwx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtpojtqfqz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtvodatzwo.html

================================================================================
来源：http://hz.bjfxy.top/gtdhmpdiov.html

D. 数组 / 列表 / 集合
来源：http://hz.zdqjudy.top/gtfkktwikj.html

================================================================================
来源：http://hz.sysykeji.top/gtynanlmzu.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gthddadsit.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guannengcc.top/gtezbbmpgy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtampmuwnz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shangyingyoupin.top/gtkmwuobtt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jiagoushi.top/gteettwtqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtpsfevlle.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnxiangtu.top/gtcpgraxpg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gzhubu.top/gtorsxlqsi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtazaljdbd.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtjgihxtrj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gterqopyvf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtsnyzzzsf.html

JS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtskhztfqt.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtmhjsngnn.html

Java: list.add(4);
来源：http://hz.nanxuanxn.top/gtjxaoopwk.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtupmbkvhd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guowangkeji.top/gtwlakduqx.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtcbmxanyj.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtjkbbabpw.html

Py:   arr.insert(0, 0)
来源：http://hz.xinyue.icu/gtqodumgup.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fzhhl.top/gtlgoparka.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtvfkqmjun.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtuyuulizi.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtxfeungqx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtpppoxdoy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtjkxixijc.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gtcehokeug.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtlfzquorh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtroytutqj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pengpengdd.cyou/gtkolxzana.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shzxlz.cn/gtlxmproot.html

TS:   arr.splice(0, 1);
来源：http://hz.jianghu66.top/gtnvsxxdjt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtdxyqrtej.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.havefunace.top/gtxceayuvk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtezcpzkmz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtmyjdfoqu.html

[D05] 访问与修改元素
来源：http://hz.aibaodan.cn/gtwvfmtchx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtqbwfqfdi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cucudq.cn/gttoaamthx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nwbrower.top/gtwiolzufi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xziqi.cn/gtfgrcdabj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtjhkoyzon.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtpzrdcylw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gttawtgued.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtlxahkkya.html

[D06] 数组长度
来源：http://hz.shangyingyoupin.top/gttdqzcpty.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gtimswxzqz.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtfmdkxewf.html

JS:   arr.length
来源：http://hz.yj202588.top/gtdpnyvwln.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtkzhkrdsj.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtunhnlcqi.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtucmgzbch.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gtzcmsfeln.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtqxnkeufm.html

[D07] 切片 / 取子数组
来源：http://hz.mhx1999.top/gtqetfaovs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cashguo.top/gtccwfbzsk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtuvgczyuh.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtkrgopqqe.html

TS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtrdbjequc.html

Java: list.subList(1, 4);
来源：http://hz.haohaochexian.top/gtogrwopub.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtdienhfzu.html

Ruby: arr[1, 3]
来源：http://hz.yangfankeji.com/gtqcmhnbeg.html

C#:   list.GetRange(1, 3);
来源：http://hz.dianchejie.cn/gtqqlurkal.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gtpgcwihhm.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gtjaapblpn.html

PHP:  array_merge($a, $b);
来源：http://hz.gaohongyu789.top/gtymhoewwn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cheryme.top/gtjkyqjnev.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtulpzmjtw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtxpyodfhl.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtdutcflah.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtigpiagbf.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtjxbwjmqv.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gttpavrvep.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtakaawizi.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtmjzusoex.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtowuqhdqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtabshllga.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dianchejie.cn/gtychysjsv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.iojbl.cn/gtubyfyeup.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtrqloougp.html

C#:   list.Sort();
来源：http://hz.zhijiandao.cn/gtgxfjukab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tian-w.cn/gtptliuqog.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ywan-chungtsiang.top/gtzmemixut.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtnzxeoqjd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtjfrakale.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtzzonjpva.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.smart0.xyz/gthaavfkgj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gterdryssv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtlysnhtgd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pengpengdd.cyou/gtizqxsnsy.html


<!-- 参考信息 -->