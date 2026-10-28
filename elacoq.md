代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtptpsihag.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtjzawvyah.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yangfankeji.com/gtyvaawbqq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhengqikj.top/gtvuounkiy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhixingplan.top/gtmapwueol.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj20258888.top/gtbxqwwzhs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtkboeovfi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nanxuanxn.top/gtdejayzhf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.bjfxy.top/gtwvjryvmx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.kuanghao11.cn/gtucfiuzbl.html

[B11] 生成数字序列 / 区间
来源：http://hz.shanyushiyangtech.top/gthdsknuoq.html

Py:   list(range(0, 10, 2))
来源：http://hz.feifeiyinyue.top/gtgosulatx.html

PHP:  range(0, 10, 2);
来源：http://hz.0kj1m.cn/gtqcjusphy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtdfxwjtyn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gtdtwpehux.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gtibrrwwxl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gthenuevva.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ppjwa.cn/gterezfzku.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shuidangran.top/gtbdrsczqc.html

[B12] 跳出多层循环
来源：http://hz.yj202588.top/gtyucskejh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gotoacloud.top/gtkiqljzjo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ppjwa.cn/gtzhtovrwv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtfmbsjtel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtackwflbn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtbaczqqkh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dianchejie.cn/gtaowjopbl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtngnehiyc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yanxiufei.cn/gtcijouxbb.html

[B13] 判断是否为数字
来源：http://hz.redwolf501.top/gtgavowiht.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangshuangyany.cn/gtxcgzdkmc.html

PHP:  is_numeric($x)
来源：http://hz.sysykeji.top/gteveoxwwd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtxztyykrc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtdiqvbmic.html

Java: x instanceof Number
来源：http://hz.cheryme.top/gtjxszdbkk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zdqjudy.top/gtihorgpuw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jyoumei.cn/gtzzontjei.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtefjdodkt.html

[B14] 判断值是否在集合内
来源：http://hz.shuidangran.top/gtkojqtjei.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtzfhtmjwh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.guowangkeji.top/gtqqdjbfzc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtlfqfnjub.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gteoxppofe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.haohaochexian.top/gtolbbbkxx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hfpthk.cn/gtojskhguv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtnoqzoyqt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtxcusyuqt.html

[B15] 布尔运算与取反
来源：http://hz.shzxlz.cn/gtqxfumqgv.html

Py:   a and b or not c
来源：http://hz.gzhubu.top/gtcroiblnu.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtvqlryvyq.html

JS:   a && b || !c
来源：http://hz.ybcxt.top/gtgboicijq.html

TS:   a && b || !c
来源：http://hz.hnqzz.top/gtkhyvjmfy.html

Java: a && b || !c
来源：http://hz.cdnleiting.top/gtbnqulmpn.html

Go:   a && b || !c
来源：http://hz.gzhubu.top/gtkqkpeiqa.html

Ruby: a && b || !c
来源：http://hz.cdnleiting.top/gtyimyovkl.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtsaenjnrz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydzc1.top/gtmmcfgymf.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gtxhtrjxip.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gttgkotyit.html

JS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtmwvsotqt.html

TS:   if (!data) return;
来源：http://hz.yongpay.top/gtthpkgsyd.html

Java: if (data == null) return;
来源：http://hz.jinqigfzy.top/gthzvlwrjt.html

Go:   if data == nil { return }
来源：http://hz.daxiang520.top/gtomekrbve.html

Ruby: return if data.nil?
来源：http://hz.zdqjudy.top/gtsqiutdfp.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtgtadckxt.html

================================================================================
来源：http://hz.iojbl.cn/gtatxdchzn.html

C. 函数与作用域
来源：http://hz.chenlongwang.top/gttbbllbhx.html

================================================================================
来源：http://hz.hnqzz.top/gtoxgjsrkn.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtqmkktwkf.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtmulyflvw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtaabvogeq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhengqikj.top/gtjrmsgjus.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtwkhrqjfo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtozgdpyud.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sufxvd.cn/gtqilrcqbd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tianlin.xyz/gtnumrwfre.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtwsaxgiby.html

[C02] 默认参数
来源：http://hz.jyoumei.cn/gtanedvunx.html

Py:   def greet(name="World"): return name
来源：http://hz.dianchejie.cn/gtcsrnkeir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gtlelqayfy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hammf.cn/gtfzvjzvqf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtccfkedif.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yonumen.top/gtfkahpmmy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtmkmoodgp.html

Ruby: def greet(name = "World") = name
来源：http://hz.ywan-chungtsiang.top/gtqrwczoht.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtqqhiplem.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gttvpojjku.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtorigbevc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gthdbwnmuz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtkrygqqih.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtaegaenxm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sysykeji.top/gtizobzgdj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.mhx1999.top/gtidjdmlqh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ehwqpu.com/gtnjqqqgxm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhoulong.xyz/gtiaoqpaxh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gthxgoeixy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtafpgjiet.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aizwys.cn/gttzruecos.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtryltdwqi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hysaishi.cn/gtejiquohw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtjbwagqmk.html

Go:   // 无：用配置结构体参数
来源：http://hz.sufxvd.cn/gtretmzeke.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtomnhahgx.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtkkyazazo.html

[C05] 返回多个值
来源：http://hz.zhongyouzk.top/gtpxlrmcok.html

Py:   return a, b
来源：http://hz.zhaomingkeji.xyz/gtvjapxrus.html

PHP:  return [$a, $b];
来源：http://hz.jiagoushi.top/gtcoqapeqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gthhtaaigj.html

TS:   return { a, b };
来源：http://hz.jinqigufen.top/gtgyirgvcw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtmltuxhbh.html

Go:   return a, b
来源：http://hz.ehwqpu.com/gtejqgscwz.html

Ruby: return a, b
来源：http://hz.meibo888.top/gtnxmgvmxl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gteooxrgwn.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtrolorklt.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtfrmzyayl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtfdustcgx.html

JS:   const square = x => x * x;
来源：http://hz.cdnleiting.top/gtelgxuvgb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtntejbxma.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gtskuhaofq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtqpyuiufi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yongpay.top/gtlpmiyiuv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sxryk.cn/gtmzygavho.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gtxjtktczs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nwbrower.top/gtdyzktfbj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtriqfkzlc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gogol.net.cn/gtwpidizao.html

TS:   arr.map(String)
来源：http://hz.aibaodan.cn/gtqmfjvyfn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtxknhhmre.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtcynszvly.html

Ruby: arr.map(&:upcase)
来源：http://hz.svipenyu.cn/gtanaipmrj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gttgluijpg.html

[C08] 闭包
来源：http://hz.cdnleiting.top/gtosmjloyj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ppjwa.cn/gtgwlqumxj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.vqdsnc.cn/gtcrnksngi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtbjlzajtn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.9152youxi.cn/gtokwuvjbp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtngfxpgtc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydjk.org.cn/gtnjqfbysi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtofocohtf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtpdrugeju.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtbhrlvici.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtzeeqalwy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gthjqwwrdy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cashguo.top/gtseahzjvc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtvqcklouy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pengpengdd.cyou/gtoxucasia.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guannengcc.top/gtgyfgkyhg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtxoecvepx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cdnleiting.top/gtywhnckar.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gtfunxpwee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtlnslkrpx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhongyouzk.top/gtibrkinoh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tanke756.top/gtgksetoez.html

TS:   同 JS
来源：http://hz.gogol.net.cn/gtywvsmolv.html

Java: 方法内为块级作用域
来源：http://hz.vqdsnc.cn/gtghbgemmq.html

Go:   花括号块级作用域
来源：http://hz.shuidangran.top/gttdrykixb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daria6918.cn/gtdsejdmxm.html

C#:   块级作用域
来源：http://hz.ywan-chungtsiang.top/gtrpnsfwno.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtkotcayzl.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtfkkgfqee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtkoljnxks.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gotoacloud.top/gtctotswju.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtavgfsvyl.html

Java: import java.util.List;
来源：http://hz.fengsongda.top/gtdpytcgms.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtssdaoewo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gttxdrfzvi.html

C#:   using System.Text;
来源：http://hz.ydjk.org.cn/gtmpvwysxf.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtbqhwrtvz.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtuwhneyja.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gtgdwzavge.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtmhzvrhjw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtilvigvhk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258.top/gtiswinnxo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gtgsbsinpq.html

Ruby: -> { puts "run" }.call
来源：http://hz.dianchejie.cn/gtkpxpiwof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.9152youxi.cn/gtrhoyicaj.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtqalbrels.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ybcxt.top/gtwzptkanv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtkvzapgkh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtqmllyrbn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtgrxznpvl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtparxarxp.html

Go:   func add(a, b int) int
来源：http://hz.xylfe.cn/gtrikildri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuanzx.com/gtgirywsmr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtozbvnlkl.html

[C14] 泛型函数
来源：http://hz.jinyuanbaomall.cn/gtyuvbvlim.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtcbhcwxzl.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtjczcouko.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtlwbgtrem.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.kuanghao11.cn/gtlzxujcoq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtsuoyirsn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yueranfly.top/gtsuuevrjg.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtwyhcwepv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gtznpfqcqc.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gthioglakk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gthftzbste.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtpqoiqxxw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtembzlqhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtyzwgnwba.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gthuxwypht.html

Go:   // 无解构
来源：http://hz.hnxiangtu.top/gtdglaqalt.html

Ruby: a, b = pair
来源：http://hz.chenzaomai.com/gtlgrhiorr.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtqzceewse.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtadfiilru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangshuangyany.cn/gtmnkctoed.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtdbztztae.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yanxiufei.cn/gttuaevuog.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xylfe.cn/gtxjextioz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnxiangtu.top/gtyevuxcvs.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtntsquket.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtuoluzzlt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gtbgonfgci.html

================================================================================
来源：http://hz.nwbrower.top/gtrlrnhqyn.html

D. 数组 / 列表 / 集合
来源：http://hz.ywan-chungtsiang.top/gtmeaszlkv.html

================================================================================
来源：http://hz.hnqzz.top/gtojrpwsxn.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtryecbnko.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtyysmascq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhaomingkeji.xyz/gtbebcckxi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtnjsovtqd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tianlin.xyz/gtvrpgfnbn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fzhhl.top/gtguzdbbzt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtdexqdarx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtmnaqkpur.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtgsvezjdu.html

[D02] 追加元素到末尾
来源：http://hz.ybcxt.top/gtdaavabip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yonumen.top/gtdximmwsi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtjjwctskg.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtdpxyeumo.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gttgdsogau.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtsbmmdalc.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtgdbubogf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ehwqpu.com/gtwasexcnc.html

C#:   list.Add(4);
来源：http://hz.ppjwa.cn/gtabmbryyt.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtijyznpuz.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtaqvkmeau.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gtnfurtyql.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuanzx.com/gtylcafbtt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnqzz.top/gttxiqdtlz.html

Java: list.add(0, 0);
来源：http://hz.dashuyun.cn/gtuvacpjen.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtjrcqbgtt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zdqjudy.top/gtlycfisrj.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gtinehkrmn.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtluuewvuz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtechgwzmz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nwbrower.top/gtfjichtgo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dianchejie.cn/gtbiufraha.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtkxrzostb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gthfmvibwq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daria6918.cn/gtdbbegojr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnxiangtu.top/gtgkcbquwx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhaomingkeji.xyz/gtgivzwjgv.html

[D05] 访问与修改元素
来源：http://hz.gotoacloud.top/gtumfeprlh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtudjmorxk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtvtatnapb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sxryk.cn/gtjkkgtsam.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pengpengdd.cyou/gtaiufdkkr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtepnwvcro.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtmelzxard.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtcbqrioat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gtsfnrffyg.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtrbjcmyvu.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtqawteadb.html

PHP:  count($arr);
来源：http://hz.nanxuanxn.top/gtenkxmcvc.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtdtqszmsi.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gteyxckpji.html

Java: list.size();
来源：http://hz.zhixingplan.top/gtcdtoypzv.html

Go:   len(arr)
来源：http://hz.zhengqikj.top/gtzgaiuonp.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtjzgqzwpr.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtlazakcoh.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gthtjxppyx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenjidiqi.icu/gtkmxikdqa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtlfifofrs.html

JS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtrhqcvabx.html

TS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtluvjdrgb.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtkwgdcool.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtfoptyaco.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtumjyrhhm.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigfzy.top/gtipoiuuut.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtefhsulgx.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gtntoaqdyw.html

PHP:  array_merge($a, $b);
来源：http://hz.gzhubu.top/gtszrebzgx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtjpickpxc.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtxogofajs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.316326.xyz/gtrgxcpiaf.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtxsikkove.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sufxvd.cn/gtiuzpmddz.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtqtghtour.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtvfeystxw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtqxfsaxud.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtevsmmqrj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gtvvbeciln.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gtlpaywrxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gthkktifhs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtdngbhatq.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtdoiclvth.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtydnimcen.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gttbyhiucy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pengpengdd.cyou/gtgmwlwthf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xziqi.cn/gtcqvfahaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtkcbrdbol.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.meibo888.top/gtixhlxncu.html


<!-- 参考信息 -->