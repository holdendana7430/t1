代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj202588.top/gtcwpzwmxu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xziqi.cn/gttwbgjigj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.daxiang520.top/gtauxwitfv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guannengcc.top/gtilxrqpcl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pengpengdd.cyou/gtnjzawjtu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hysaishi.cn/gtqhfjbttw.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtieoikbpr.html

Py:   list(range(0, 10, 2))
来源：http://hz.hysaishi.cn/gtxbshilzb.html

PHP:  range(0, 10, 2);
来源：http://hz.ybcxt.top/gtllpcelbr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aizwys.cn/gtydjaxljy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hfpthk.cn/gtfsluodvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ivvv.top/gtcllphcvs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yuanzhike.top/gtoeqkpjib.html

Ruby: (0...10).step(2).to_a
来源：http://hz.smart0.xyz/gtctjaadma.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shzxlz.cn/gtvafskxvl.html

[B12] 跳出多层循环
来源：http://hz.aibaodan.cn/gtwjpnylqc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ywan-chungtsiang.top/gtkmhvtryz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhoulong.xyz/gturobwfhp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtgjkeyvbe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtexcgwqtf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtlkoutbnk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hywenlv.cn/gtuagnkcrn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tanke756.top/gtjytcyxju.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.svipenyu.cn/gtqtattpny.html

[B13] 判断是否为数字
来源：http://hz.0kj1m.cn/gtizpliehw.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtryjsmhav.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtolrysplw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtlpjaktde.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtxmspvtvi.html

Java: x instanceof Number
来源：http://hz.nanxinkj.top/gtawimupnd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhaomingkeji.xyz/gtrbwxiwud.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gaohongyu789.top/gtdsfqxotj.html

C#:   x is int or double or decimal
来源：http://hz.vqdsnc.cn/gtslyutywq.html

[B14] 判断值是否在集合内
来源：http://hz.tanke756.top/gtzurkvcnq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cashguo.top/gtnclezjjq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gtuulcgudo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtofpgrgly.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gttxqcgxve.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtyomhdznq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yanxiufei.cn/gtsxfulqml.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhongyouzk.top/gtrzxxhctz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.kuanghao11.cn/gtcapjvgls.html

[B15] 布尔运算与取反
来源：http://hz.ybcxt.top/gtmeprqeks.html

Py:   a and b or not c
来源：http://hz.sxryk.cn/gtwpxwycni.html

PHP:  $a && $b || !$c
来源：http://hz.0kj1m.cn/gtlxdrarka.html

JS:   a && b || !c
来源：http://hz.ybcxt.top/gtuvjlpvxj.html

TS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtuyuwqnfy.html

Java: a && b || !c
来源：http://hz.wangshuangyany.cn/gtpxoetbgu.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtmmoqeohd.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtnqolgkru.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtryqpiuzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.0kj1m.cn/gtwlitfxwm.html

Py:   if not data: return
来源：http://hz.zdqjudy.top/gtmlplwobb.html

PHP:  if (!$data) { return; }
来源：http://hz.hywenlv.cn/gtihgiylzz.html

JS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtbyvrrxkm.html

TS:   if (!data) return;
来源：http://hz.hnqzz.top/gtfsqebpik.html

Java: if (data == null) return;
来源：http://hz.bjfxy.top/gtwxzwwfdr.html

Go:   if data == nil { return }
来源：http://hz.ywan-chungtsiang.top/gthmvipjpb.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtxzjmcpjw.html

C#:   if (data == null) return;
来源：http://hz.birdmap.top/gtpttngmwt.html

================================================================================
来源：http://hz.nwbrower.top/gtlpiksgre.html

C. 函数与作用域
来源：http://hz.yueranfly.top/gtcrrmjofs.html

================================================================================
来源：http://hz.sysykeji.top/gtyuajjrpm.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtjxfaijpt.html

Py:   def add(a, b): return a + b
来源：http://hz.zdqjudy.top/gtixxuvosa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtvcaivmqh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yueranfly.top/gtjlkgnucz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gthxluslne.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtgagouglf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtyvxqhszj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhengqikj.top/gtjwymvqui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtnplromfq.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtoxngkkja.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtctfhhvku.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigufen.top/gttgnggutg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.haohaochexian.top/gtjbxhneyf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtovabygev.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cdnleiting.top/gtxtomngdb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtlvyqsrvq.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydzc1.top/gtupezpspu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenzaomai.com/gtgwmvtxse.html

[C03] 可变参数
来源：http://hz.yj202588.top/gtltjbrlig.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangdashe.top/gtzlkegyzg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtowkxhtmc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtndpvmwwk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtadouylly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.52xcode.cn/gtvrckmosh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.feifeiyinyue.top/gtoljglnxm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gaohongyu789.top/gtyzuabhqg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sxryk.cn/gtxaatifki.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtfvgbniic.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tianlin.xyz/gteevifszf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtrahgoftl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtvpoxprfg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtgwxexiqa.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtiqawlxly.html

Go:   // 无：用配置结构体参数
来源：http://hz.fzhhl.top/gtscsbwnes.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtdxxssrva.html

C#:   f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtguiwuztn.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gtlalydcuw.html

Py:   return a, b
来源：http://hz.gaohongyu789.top/gtdsvkbyfa.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtuokaqvqi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yonumen.top/gtrpgbmlli.html

TS:   return { a, b };
来源：http://hz.pycfn.com/gtsynhikkc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangkeji.top/gtdusxclbx.html

Go:   return a, b
来源：http://hz.zhengqikj.top/gtysgaslgf.html

Ruby: return a, b
来源：http://hz.yueranfly.top/gtmjddqguz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuetiantiany.cn/gtiptebhpe.html

[C06] 匿名函数 / lambda
来源：http://hz.xinyue.icu/gtxpufxfor.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtzrrmesvh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.quarkkingdee.top/gtuzdgxbab.html

JS:   const square = x => x * x;
来源：http://hz.cashguo.top/gtqiihrdzp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sweek.top/gtzdusyjkx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pengpengdd.cyou/gtsdacthui.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.dianchejie.cn/gtbwggodvk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtyputghww.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hammf.cn/gteounhbjq.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtkaohgzpe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cdnleiting.top/gtulujzrin.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xylfe.cn/gtupxkpvhk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.meibo888.top/gtbqffwpdd.html

TS:   arr.map(String)
来源：http://hz.hnqzz.top/gtoqcfktcp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gaohongyu789.top/gtjoxzvpsu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hfpthk.cn/gthqitttqp.html

Ruby: arr.map(&:upcase)
来源：http://hz.pycfn.com/gteuejcexw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtursjprni.html

[C08] 闭包
来源：http://hz.birdmap.top/gtbfbegnsv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtcpjbtftw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gtntlmavic.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gttmimfird.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtmovoskgf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtmvazzfyz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtmwisirks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guannengcc.top/gtxhczcdxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtwnzluqur.html

[C09] 递归
来源：http://hz.gzhubu.top/gtofsanfcd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtmmrbmofr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.smart0.xyz/gtowvbutuv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtgkwyqamb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtmcnecdps.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guowangkeji.top/gtmihlppqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258888.top/gtpdzpukdp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.havefunace.top/gtkgrqkitp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtlglrkrus.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtoiojmjlf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtzazpnxae.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jianghu66.top/gtvhcnloyy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.snrcjt.cn/gtmgiibqpe.html

TS:   同 JS
来源：http://hz.guannengcc.top/gtmlodmzde.html

Java: 方法内为块级作用域
来源：http://hz.birdmap.top/gticxqitvb.html

Go:   花括号块级作用域
来源：http://hz.svipenyu.cn/gtxzfbysot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtpqmvcnlt.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtmtcmvqpz.html

[C11] 模块导入与导出
来源：http://hz.nanxuanxn.top/gtkbehhahg.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtdwxiteyl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj20258888.top/gtfdoecveq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daria6918.cn/gtancsvcof.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgufenzy.top/gtglllbsjo.html

Java: import java.util.List;
来源：http://hz.nwbrower.top/gtzfmmhtcj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nwbrower.top/gtrcalvcul.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangkeji.top/gtjobtaqed.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gttkvqpzby.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhaomingkeji.xyz/gtfxfeznna.html

Py:   (lambda: print("run"))()
来源：http://hz.aizwys.cn/gtxxzwiwea.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gtdrpnswbf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtuhqucavy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtwjtavbqm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxinkj.top/gtgtnpqqwk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtixuejwwy.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtkudyicag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxuanxn.top/gtopozlgdz.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtzixjsmsm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ybcxt.top/gtxsdhhhrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtqwswickb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtzxlpzxzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cucudq.cn/gtobfbjqxn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtrdawzmac.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtauehpwze.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtoxxrzfjb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtivrkwjqi.html

[C14] 泛型函数
来源：http://hz.hongshengwenyu.top/gtmxjzdsoo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnxiangtu.top/gtmbwkmuyu.html

PHP:  // 无泛型
来源：http://hz.guowangkeji.top/gtquzhzzik.html

JS:   // 无泛型
来源：http://hz.hongshengwenyu.top/gtsizmldaz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gthwaujxpj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtlbaecyvc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yangfankeji.com/gtzqcccvyt.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gtyfiomgdv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gteitfcrnr.html

[C15] 解构 / 展开参数
来源：http://hz.smart0.xyz/gtmsrkxige.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtzvlccpsu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtjupvjrdj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yonumen.top/gttulzzuyr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgfzy.top/gtizyoeomx.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtppblkljd.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtyiprcajv.html

Ruby: a, b = pair
来源：http://hz.smart0.xyz/gtkgjcdqet.html

C#:   var (a, b) = pair;
来源：http://hz.fengsongda.top/gtfawtjhaw.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtkumqgelu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtfpmelnnu.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gtikuakoxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtywbwfivr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgfzy.top/gtlstetlvx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtukgchdst.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtzsnpbnis.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cheryme.top/gtvxrbodhw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtvkqftxpf.html

================================================================================
来源：http://hz.yuxming.cn/gtrszxpvvg.html

D. 数组 / 列表 / 集合
来源：http://hz.xziqi.cn/gtsolkiamv.html

================================================================================
来源：http://hz.wangdashe.top/gtwmtfngoe.html

[D01] 创建数组 / 列表
来源：http://hz.gzhubu.top/gtkfhllchy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtvepxpbfa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydjk.org.cn/gthmxeattl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gtlynvxfib.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gthobhzgow.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cucudq.cn/gtcbzurmlk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hywenlv.cn/gtlskklkyj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.quarkkingdee.top/gtygqlfgri.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtywpzkcve.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtwoghwxcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtppnojlnl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtfarrehtf.html

JS:   arr.push(4);
来源：http://hz.gogol.net.cn/gttpsoastv.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gttiutyxsn.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtyfwkpbdw.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtrazmpdfa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtvhrkmodi.html

C#:   list.Add(4);
来源：http://hz.jqgfzy.top/gtwfmcnzus.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtfavwrkcq.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtyanxqszf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtmuklcoxy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinyuanbaomall.cn/gtdapoqnua.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jyoumei.cn/gtmwvsoedk.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtisxkadlj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtquhrrwvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxinkj.top/gtzvbhuelz.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgufenzy.top/gthvxsobrg.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtnzmmabtz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gttimrvfhj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtjvvtlkkl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuanzx.com/gtiidqsysk.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gtdfsbghux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yangfankeji.com/gtkyydnwus.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gthubouqio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtmczqgsax.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhijiandao.cn/gtbdgrxvda.html

[D05] 访问与修改元素
来源：http://hz.52xcode.cn/gtmhxefoak.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtbkdmpxqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtqbhmwxhp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtybgqacvi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtzzoxbldw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shangyingyoupin.top/gtcksmlagg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.52xcode.cn/gtdgyykmgk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtjaoklmmg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtwqnaorcn.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtpwfaxrpo.html

Py:   len(arr)
来源：http://hz.chenlongwang.top/gtgpujhapd.html

PHP:  count($arr);
来源：http://hz.316326.xyz/gtximwfffe.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtpjnqlamj.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtxnkkjnrw.html

Java: list.size();
来源：http://hz.yueranfly.top/gtlvowwgzn.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtolbzvekz.html

Ruby: arr.length; arr.size
来源：http://hz.cucudq.cn/gtqtlgatip.html

C#:   list.Count;
来源：http://hz.yuxming.cn/gtejtpukap.html

[D07] 切片 / 取子数组
来源：http://hz.xziqi.cn/gtihwssrcd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.9152youxi.cn/gtzxuzkkpd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuetiantiany.cn/gtdabkvaby.html

JS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtdsxqjlgv.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtjqifpnsk.html

Java: list.subList(1, 4);
来源：http://hz.havefunace.top/gtfqnarpqb.html

Go:   arr[1:4]
来源：http://hz.ydjk.org.cn/gtpnspvjnr.html

Ruby: arr[1, 3]
来源：http://hz.9152youxi.cn/gtvhvmrnol.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigfzy.top/gtoihplydi.html

[D08] 合并两个数组
来源：http://hz.zycfv.cn/gtqrumuzqg.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtpbzjpwbz.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtjhivkzsd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtbnlaslfr.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gthuruytxk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.c1oappe.top/gtwfwqxuny.html

Go:   append(a, b...)
来源：http://hz.yonumen.top/gtybcblzbi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtcfgmzupa.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gtracjklrk.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtbsllqmha.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtwuretycn.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtyeebyrcp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtyunijrbc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtecyuzaoz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtjmkbxzhe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtyiqyzmfi.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtoolpfmod.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gtvdormsjl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtxaouorau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gtrstrciqs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtauieymcw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtqvahnqcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtkqrhjcgo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtcmahhalj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtvnrsqwkh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtrfkbrjce.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtytuzefas.html


<!-- 参考信息 -->