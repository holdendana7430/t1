代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtedrvbeke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtnydphupw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nwbrower.top/gtzkxiszaa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxinkj.top/gtwlkesxtl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtizgeuljs.html

[B10] 遍历同时拿索引
来源：http://hz.zhaomingkeji.xyz/gtlcnluazt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shzxlz.cn/gtcbuhpqtf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.c1oappe.top/gtbybsyfxs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ywan-chungtsiang.top/gtebxqmcqh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtpdntfiui.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.mhx1999.top/gtcxempntn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pycfn.com/gthncocvvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuanzx.com/gtavwxltgm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.316326.xyz/gtwpykwwap.html

[B11] 生成数字序列 / 区间
来源：http://hz.pycfn.com/gtzzhltcym.html

Py:   list(range(0, 10, 2))
来源：http://hz.cashguo.top/gtjohdziix.html

PHP:  range(0, 10, 2);
来源：http://hz.hongshengwenyu.top/gtdjrhxfpp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.kuanghao11.cn/gtmsuzvpbv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtrnugevrk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ybcxt.top/gtitgcoslr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xylfe.cn/gtfoffpsyc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhixingplan.top/gtsaudpisc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxinkj.top/gtkpjolpzl.html

[B12] 跳出多层循环
来源：http://hz.zhaomingkeji.xyz/gtwypfvxda.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gtjyydblzo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hammf.cn/gtauqlixnx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gteeryyngj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtdzfigman.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.feifeiyinyue.top/gtfjanasfk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hywenlv.cn/gtjmwkjrcu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sweek.top/gtkywbvcgh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.snrcjt.cn/gtzqqcrjub.html

[B13] 判断是否为数字
来源：http://hz.zhiwuduotai.top/gtgsyvmywc.html

Py:   isinstance(x, (int, float))
来源：http://hz.cashguo.top/gtzutcvcnj.html

PHP:  is_numeric($x)
来源：http://hz.jinyuanbaomall.cn/gtwzmdywmx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtbduntfon.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnxiangtu.top/gtyykkqyre.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtlhpwhody.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gteofcjazc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xziqi.cn/gthtpdetwp.html

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gtlcqhaeqe.html

[B14] 判断值是否在集合内
来源：http://hz.jqgufenzy.top/gttwrcrmvy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.smart0.xyz/gtjelbgioi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jiagoushi.top/gtogmstois.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtpxbihryt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtfodwyxyk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.0kj1m.cn/gtpbokxmhv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daxiang520.top/gtzpzahzqp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydzc1.top/gtbtayoapr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtisduzsmt.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtzkugamhu.html

Py:   a and b or not c
来源：http://hz.jqgufenzy.top/gtzcoqzagw.html

PHP:  $a && $b || !$c
来源：http://hz.gzhubu.top/gtvuzlcgmq.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtrsjdlhtc.html

TS:   a && b || !c
来源：http://hz.cheryme.top/gtzynsnfpv.html

Java: a && b || !c
来源：http://hz.cucudq.cn/gthwovpjbi.html

Go:   a && b || !c
来源：http://hz.zhongyouzk.top/gtpgprwdgz.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtvgnkvzpz.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtnxjmveln.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gttiglglji.html

Py:   if not data: return
来源：http://hz.jqgufenzy.top/gtrlhdcqyr.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtnnurtrwx.html

JS:   if (!data) return;
来源：http://hz.ppjwa.cn/gtgcrludhe.html

TS:   if (!data) return;
来源：http://hz.daxiang520.top/gtlppgrhvm.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gtvaarruiv.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtccnshyjv.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtarzmpmcx.html

C#:   if (data == null) return;
来源：http://hz.nanxinkj.top/gtnkshmtxx.html

================================================================================
来源：http://hz.nwbrower.top/gtdnydyzwp.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtznqeyroj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlofawsfr.html

[C01] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtrcddnqiw.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gtdkzxsxnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtfydnvpuk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yvedp.cn/gtzyinnubk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtyttljuro.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtodjzfaym.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtwytdyosq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xziqi.cn/gtgcncejhn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtpvskmiau.html

[C02] 默认参数
来源：http://hz.jqgfzy.top/gtoyaitcyi.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtzvzraznk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtisigqpxn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cqqwz.cn/gtgjkiflpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtztgvtzzm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtprbcievi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ppjwa.cn/gtygjifqpr.html

Ruby: def greet(name = "World") = name
来源：http://hz.svipenyu.cn/gttpbylblh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtikfpvxit.html

[C03] 可变参数
来源：http://hz.yanxiufei.cn/gtjdclybgi.html

Py:   def total(*args): return sum(args)
来源：http://hz.daxiang520.top/gtezwugreo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtodlcwgrz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtvazrlcun.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtmwckkwsp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangdashe.top/gthjachzie.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtdrzorzij.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtwesiicne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gtbmhnnjkz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtorqzvurj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jianghu66.top/gtmrujngpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangshuangyany.cn/gtnolfoned.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtfmyxzhfq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tanke756.top/gtqfqkbxtf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ehwqpu.com/gtviutdpql.html

Go:   // 无：用配置结构体参数
来源：http://hz.bjfxy.top/gtxinamijy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtqrchwbvo.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtxcjularn.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtbdzwraln.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtoruqkwyn.html

PHP:  return [$a, $b];
来源：http://hz.quarkkingdee.top/gtvxztbfqe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtlaadrgpb.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtxhhsmhim.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtonrvdpru.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtngjqpvhk.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gteiznormq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.kuanghao11.cn/gtaevswkld.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangkeji.top/gtzdxsjwmj.html

Py:   square = lambda x: x * x
来源：http://hz.gogol.net.cn/gtgolvxgfe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtogjryvsg.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtwejerdlv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtejhfnpoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pycfn.com/gtgrqnzwej.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yueranfly.top/gtnxxuaquo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aibaodan.cn/gtmboiqffg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xylfe.cn/gtqozaigro.html

[C07] 把函数作为参数传入
来源：http://hz.wangdashe.top/gtslinyyaw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhixingplan.top/gtrevcglxk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.feifeiyinyue.top/gtdpgbpufm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtljwrqgfp.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtlylvvrht.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gaohongyu789.top/gtfwlfycpm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.mhx1999.top/gtxtafjfru.html

Ruby: arr.map(&:upcase)
来源：http://hz.dianchejie.cn/gtaauqcgoe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yueranfly.top/gtkhrgxptt.html

[C08] 闭包
来源：http://hz.sufxvd.cn/gthtoevxuw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pycfn.com/gtnakfohoh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnxiangtu.top/gtildjcmjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtvxywnxof.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.smart0.xyz/gtvyfnikde.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtegcejvxi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gttocfkzve.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.iojbl.cn/gtoeovzuyz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtrtesbdvz.html

[C09] 递归
来源：http://hz.guannengcc.top/gtkevndcqf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtvudgonsm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aizwys.cn/gtbvcpecks.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtttcjshql.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtbkvnxxxq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yonumen.top/gtktqzkszo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtovaguprh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtoipavmft.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhoulong.xyz/gtoxofayvl.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtgegdcqaf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtszvviysw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhoulong.xyz/gtcohxmwci.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.c1oappe.top/gtddzkbekv.html

TS:   同 JS
来源：http://hz.cucudq.cn/gtawntkdca.html

Java: 方法内为块级作用域
来源：http://hz.chenlongwang.top/gtswaqrbob.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtmxmcluzv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yueranfly.top/gtzqycqarw.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtlaxtdvnl.html

[C11] 模块导入与导出
来源：http://hz.yongpay.top/gtdmzxmjua.html

Py:   from module import func
来源：http://hz.hongshengwenyu.top/gtckinblwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhengqikj.top/gtuluevdsq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtmsoktklj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtegqrsrej.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtuxzcjvgl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtgmyicfgf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtqjmkwvmd.html

C#:   using System.Text;
来源：http://hz.aibaodan.cn/gtindmvlzh.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtvoufryee.html

Py:   (lambda: print("run"))()
来源：http://hz.jinghuilouyu.cn/gtzcioziay.html

PHP:  (function () { echo "run"; })();
来源：http://hz.kuanghao11.cn/gtaympizjt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtphkvqrmg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtnblggyyi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gtkhktzkqw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hywenlv.cn/gtokxdyjqx.html

Ruby: -> { puts "run" }.call
来源：http://hz.hysaishi.cn/gtbsqvbbvj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xinyue.icu/gttifloxjr.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gthtnlrnoh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtwihksrrz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtacsyhvti.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtlariqsed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtfitnfhzv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtfwudvojf.html

Go:   func add(a, b int) int
来源：http://hz.jinyuanbaomall.cn/gtrdshapfk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hfpthk.cn/gtdfqfanen.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtzuntzpkj.html

[C14] 泛型函数
来源：http://hz.andypj.xyz/gtfmrnxhzr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenlongwang.top/gtdqobbyds.html

PHP:  // 无泛型
来源：http://hz.yvedp.cn/gtcqkuzzmg.html

JS:   // 无泛型
来源：http://hz.yj20258888.top/gtdktpzvod.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gotoacloud.top/gtamzncods.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtxrlxwdjj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sweek.top/gtvysxhncp.html

Ruby: # 无泛型
来源：http://hz.hysaishi.cn/gtzhrnlboj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtobitwrcc.html

[C15] 解构 / 展开参数
来源：http://hz.hysaishi.cn/gtafqxxldm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.havefunace.top/gthesjtzfj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gtslkcwczt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtublrtagx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtcbegluym.html

Java: // 无解构
来源：http://hz.cucudq.cn/gtxntltjzo.html

Go:   // 无解构
来源：http://hz.jiagoushi.top/gtkmogajcq.html

Ruby: a, b = pair
来源：http://hz.daria6918.cn/gtzdgnpsio.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gttdjxzrrt.html

[C16] 函数 / 方法重载
来源：http://hz.xinyue.icu/gtvsxmklqu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtzdzqmtma.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gtlhxnhwkj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gtphvrehxn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtughljdor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gtzdajrrlm.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gtxezknozi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtcovwubtc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xingfuxueyuan.xyz/gtlfmafviz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjartbuow.html

D. 数组 / 列表 / 集合
来源：http://hz.zhengqikj.top/gtqsppbsuu.html

================================================================================
来源：http://hz.zhengqikj.top/gtsugbbapq.html

[D01] 创建数组 / 列表
来源：http://hz.ybcxt.top/gtyqkrxgoo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.havefunace.top/gtqmljqzhk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aizwys.cn/gtjiwlbvha.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtousyqjir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtocyjvulg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtscrkjpze.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jiagoushi.top/gtsftvqzgf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtrnsykyeu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gotoacloud.top/gtlpgsdwta.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gthibesegc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtccdcbftf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.c1oappe.top/gtkaptxuyr.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtgxhaedxt.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtkilhkqtt.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtmqgurhoz.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtpaicoxkb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtehasgokc.html

C#:   list.Add(4);
来源：http://hz.yanxiufei.cn/gtxgxcxick.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtgdsxbaam.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtqoyupjgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gtldvksatl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhijiandao.cn/gtjhvthukm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gtpvdmrfgz.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtzylehzti.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gthpouubyp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtmrxcinsr.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtukrptoha.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gtcoidhdqb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.9152youxi.cn/gtfsgxtbpe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gzhubu.top/gtzbuwarqo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gtingcdnxn.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtlmrvccoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtfsdwhnst.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gtwjbfoxwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guowangkeji.top/gtvwzlprtp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtnlrbxzpo.html

[D05] 访问与修改元素
来源：http://hz.hfpthk.cn/gtklvqiqyf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtbrywlawm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gttvkysysr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtkdqbhmle.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtxeobeoee.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtqveezyif.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtzeejzkum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtpmktyvjk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gaohongyu789.top/gtfxraeqte.html

[D06] 数组长度
来源：http://hz.aizwys.cn/gtbggpkcla.html

Py:   len(arr)
来源：http://hz.yongpay.top/gtrfdfqhrg.html

PHP:  count($arr);
来源：http://hz.fengsongda.top/gtrevojnff.html

JS:   arr.length
来源：http://hz.316326.xyz/gtmgrqpxyh.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtmjxiaknz.html

Java: list.size();
来源：http://hz.nwbrower.top/gtmuufsvqi.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtxhwraggn.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtmxpqzllh.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtlykythlm.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtldxfxxme.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuanzhike.top/gtnqplqykq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.havefunace.top/gtayohjaut.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtofpliveu.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtashnmndh.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtoglbmkuv.html

Go:   arr[1:4]
来源：http://hz.nanxuanxn.top/gtknfopuqr.html

Ruby: arr[1, 3]
来源：http://hz.nwbrower.top/gtqrmodktk.html

C#:   list.GetRange(1, 3);
来源：http://hz.hnqzz.top/gtlfhzkbxd.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtazqbrihs.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhiwuduotai.top/gtpbbzfbrg.html

PHP:  array_merge($a, $b);
来源：http://hz.zhengqikj.top/gtauriiqty.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtdbhuohdc.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtibbqurkn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guannengcc.top/gtpwlgeolq.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtlttfunrg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtmruyrewt.html

C#:   a.Concat(b).ToList()
来源：http://hz.sweek.top/gtdkwgkiwt.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtwbitvjgz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtepcsjiab.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtccsighrq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenlongwang.top/gtxvldoumm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.birdmap.top/gttinltmmw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtnnywhlzf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtufcuinip.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtryqzihsi.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtkfosbpgc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gttkmcllep.html


<!-- 参考信息 -->