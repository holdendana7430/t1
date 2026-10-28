代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258.top/gtjegcfrle.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xuetiantiany.cn/gtktzghwvr.html

[B11] 生成数字序列 / 区间
来源：http://hz.pengpengdd.cyou/gtoynabbqq.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhongyouzk.top/gtbbpjpkhi.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgufenzy.top/gthpysawro.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtjmphwmuu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinyuanbaomall.cn/gtezlcqafm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hysaishi.cn/gttuthsqdg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tanke756.top/gtawllxhkh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ydzc1.top/gtgijowzro.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yongpay.top/gtbgfrvlfu.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gteajxaoui.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtiouwnxzr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.snrcjt.cn/gtisunwzom.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtglubjplc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtlihvlwdt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtzoydajfp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dianchejie.cn/gtyitlxeho.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gtylawdvze.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gthyxosqer.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gtnhpapced.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnxiangtu.top/gtfpsagyjt.html

PHP:  is_numeric($x)
来源：http://hz.9152youxi.cn/gtkdmzfdkq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtvihazqjv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gtyzglpxir.html

Java: x instanceof Number
来源：http://hz.havefunace.top/gtnjpdtlod.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shzxlz.cn/gtodnqqpqc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gtszhsqsyp.html

C#:   x is int or double or decimal
来源：http://hz.hammf.cn/gtxsnlxoli.html

[B14] 判断值是否在集合内
来源：http://hz.dashuyun.cn/gtomzlxelw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shangyingyoupin.top/gtgynhkryh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.kuanghao11.cn/gtylywiqpy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtuliwfsss.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtzlxgjmlm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.quarkkingdee.top/gttcwpargq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yonumen.top/gtrkkobabe.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhiwuduotai.top/gtgxmbnutv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gtbylfqwgv.html

[B15] 布尔运算与取反
来源：http://hz.sufxvd.cn/gtfnyraksl.html

Py:   a and b or not c
来源：http://hz.guannengcc.top/gtqhhdpkrg.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtgvzhzxxe.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtsifvkwrw.html

TS:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtvtbyawji.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gtfjclebqg.html

Go:   a && b || !c
来源：http://hz.ppjwa.cn/gtzmjjxexp.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtuownaqew.html

C#:   a && b || !c
来源：http://hz.xinyue.icu/gtevdcjnmm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.haohaochexian.top/gtmomsfbgs.html

Py:   if not data: return
来源：http://hz.hnxiangtu.top/gtygtmwccx.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtsnnqgzjt.html

JS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtcnsntdqx.html

TS:   if (!data) return;
来源：http://hz.aizwys.cn/gtfljswbrb.html

Java: if (data == null) return;
来源：http://hz.zhixingplan.top/gtgcjsjaad.html

Go:   if data == nil { return }
来源：http://hz.gogol.net.cn/gtccutapil.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtsefuaiuw.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtxmskoisv.html

================================================================================
来源：http://hz.ydzc1.top/gtkllqwnxu.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtfapmsdlu.html

================================================================================
来源：http://hz.hnqzz.top/gtjunrbqfw.html

[C01] 定义函数
来源：http://hz.zdqjudy.top/gtfbljvpxt.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gttopsegyw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtwgzlmmof.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hfpthk.cn/gtjqpdavqx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtcyjmrlqd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtldkquove.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gtmyujfgnn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtinhxgtpi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtkxiwdvpp.html

[C02] 默认参数
来源：http://hz.yj20258888.top/gtqkwodfgk.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtwfmcbyve.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gthijxjmlk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xziqi.cn/gtwdwsdcvw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtpwdhirhm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sxryk.cn/gtvdoayuzq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenzaomai.com/gthqjkbhee.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydjk.org.cn/gtdhrnwlqi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gttehxlttu.html

[C03] 可变参数
来源：http://hz.jiagoushi.top/gtyxmpelfq.html

Py:   def total(*args): return sum(args)
来源：http://hz.haohaochexian.top/gtcekjtvrd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guowangkeji.top/gteaoyexbm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtkiunrdpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtrfvcdzry.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.haohaochexian.top/gtbnfzcjbu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cheryme.top/gteduibbnc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.meibo888.top/gtuifhsfbv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigfzy.top/gtdrqgtyrq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtcbsxcfjx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gteckohgnm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gthtqkqaqy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtsgjijtir.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtycwcsoln.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtiqyevjhv.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gtkpalztps.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtoeradakm.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtbenfnjbk.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gtuazqdvcw.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtwwmpyisy.html

PHP:  return [$a, $b];
来源：http://hz.pycfn.com/gtrsmxmobv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhixingplan.top/gtoimkchlp.html

TS:   return { a, b };
来源：http://hz.feifeiyinyue.top/gtuyqbfneo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sufxvd.cn/gtigmapthl.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtmfaudtyo.html

Ruby: return a, b
来源：http://hz.fzhhl.top/gtytsahikg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daxiang520.top/gtcqckmgwa.html

[C06] 匿名函数 / lambda
来源：http://hz.hnqzz.top/gtilubztzq.html

Py:   square = lambda x: x * x
来源：http://hz.sysykeji.top/gtzjneewei.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shuidangran.top/gtomgsrlsc.html

JS:   const square = x => x * x;
来源：http://hz.ivvv.top/gtkeuwmjls.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gthlcusdio.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtpniezskr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtvcgrghsf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxuanxn.top/gtzpuprtoe.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtxjokzfik.html

[C07] 把函数作为参数传入
来源：http://hz.52xcode.cn/gtqimdgxdk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gtypxftzhj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtkhzbyasq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangdashe.top/gttarxpvju.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtrnvbsirm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.andypj.xyz/gtdzkudsek.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gthoacnuau.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtoowengeu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtzsqjozwd.html

[C08] 闭包
来源：http://hz.xingfuxueyuan.xyz/gtdxfpomrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hongshengwenyu.top/gtychzokda.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.haohaochexian.top/gtsqukdmmd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtghquqcyv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtligdvlak.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pengpengdd.cyou/gtopyolpsd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj202588.top/gtfrivkmga.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gtgkovrnjx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtukyumksg.html

[C09] 递归
来源：http://hz.nanxinkj.top/gtkpqwfmib.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.bjfxy.top/gtmvcxzbsf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtdwguapqx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtkcdstmna.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtzndlupvt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtecgwxokx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtlblobxsc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtqsewldzz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuanzhike.top/gtechmharq.html

[C10] 变量作用域
来源：http://hz.haohaochexian.top/gtuvxniuyi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtzxttglqk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtytvjaojq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtuclzroqy.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtqyvrexoc.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtnqlriygq.html

Go:   花括号块级作用域
来源：http://hz.ywan-chungtsiang.top/gthhwpbrjl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhixingplan.top/gtvbowpyfl.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gttgekelwj.html

[C11] 模块导入与导出
来源：http://hz.jiagoushi.top/gtnndsehjp.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtrgxusvkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtjigvvzil.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gotoacloud.top/gtmptpddww.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shangyingyoupin.top/gtrditnjxx.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gthaydxzgz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgfzy.top/gtnebaqcnn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtihkaiidw.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtcluprxrk.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtzvcdjmqu.html

Py:   (lambda: print("run"))()
来源：http://hz.feifeiyinyue.top/gtwkbgygmi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtuhxkzbsu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtozrjhzdr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtrlxxwzpb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydjk.org.cn/gtfqwldpyr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dianchejie.cn/gtmchbnyfv.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtfabbcgzq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtjzvchkxj.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gthxxbdleh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtciapyzus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtxsxugcrw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zycfv.cn/gtmfvoaqea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtfrutiqwv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtzcafldai.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtwntmdbxm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.feifeiyinyue.top/gtgjapevcg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtiimpfkyx.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtigdhgymc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.haohaochexian.top/gturkdqobd.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtkzypgzqs.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtzloekzhz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.bjfxy.top/gtxynfakmm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtxtieswwz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtxoxvtyjb.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gtdkanbvqf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangdashe.top/gtfjmiudrn.html

[C15] 解构 / 展开参数
来源：http://hz.jqgfzy.top/gturomgxkk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zdqjudy.top/gtygbbtneh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtesjautzc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtzjvbywpk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xylfe.cn/gtfgjhyaza.html

Java: // 无解构
来源：http://hz.hammf.cn/gtghundjfj.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtypuqlhan.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtyehhksqs.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtpismcvda.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtdchqqvok.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtbzfbkfvv.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gtfcdkjjbb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cdnleiting.top/gtkqbqojqx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtykicwubn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtiegtkvoe.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtyqhcvzzu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtofvaqpvp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtjmwntolt.html

================================================================================
来源：http://hz.svipenyu.cn/gtqjqenvos.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gtxvihyjay.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtakifyhym.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gtdohekyuw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtwlqbngyj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtqnqnaida.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtqbvlqvbd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jyoumei.cn/gtzgpzvnsm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daxiang520.top/gtlbxduubz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.0kj1m.cn/gtzcopdumm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtkkhnihwa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.bjfxy.top/gtidkkftxu.html

[D02] 追加元素到末尾
来源：http://hz.yj20258.top/gthinptsoe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.kuanghao11.cn/gtarttpoij.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtdyadtobn.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtkcgvczjf.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtktkphsrj.html

Java: list.add(4);
来源：http://hz.sufxvd.cn/gtunslwjnp.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gthbcrxpor.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zdqjudy.top/gtthiucpnd.html

C#:   list.Add(4);
来源：http://hz.yj20258888.top/gtfprcowpn.html

[D03] 在指定位置插入元素
来源：http://hz.shangyingyoupin.top/gtlfmxkyzr.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtxyzpnftz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cqqwz.cn/gteevjnlyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgufenzy.top/gtlwowyiff.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhoulong.xyz/gtwgvbdejk.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtqxiqohtl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shangyingyoupin.top/gtalrruemv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtgpdfjlis.html

C#:   list.Insert(0, 0);
来源：http://hz.xuanzx.com/gttmracowr.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtavrqbtzz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtwljwnymx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtmjfbdcyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtcnryloly.html

TS:   arr.splice(0, 1);
来源：http://hz.zhijiandao.cn/gtbwjcxnqo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.haohaochexian.top/gtmhytjubg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gttdwmumdr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtljceusqc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinghuilouyu.cn/gtygiizjbq.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtaqzzenyx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtrhfiwlij.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yvedp.cn/gtxxldkqbl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yueranfly.top/gttrewhxaa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gtpwtihsxe.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinyuanbaomall.cn/gtzdtprbqw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtwiwghzxr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtrmnvdmfq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtrrgbuqmc.html

[D06] 数组长度
来源：http://hz.feifeiyinyue.top/gtdcddpgsl.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtfcikckpg.html

PHP:  count($arr);
来源：http://hz.yvedp.cn/gtwhbdelke.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtbwgijuac.html

TS:   arr.length
来源：http://hz.nanxinkj.top/gttntxioco.html

Java: list.size();
来源：http://hz.jinyuanbaomall.cn/gtmkdomzdr.html

Go:   len(arr)
来源：http://hz.xuetiantiany.cn/gtkmiigzok.html

Ruby: arr.length; arr.size
来源：http://hz.hongshengwenyu.top/gtpoowfpsz.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtlwaflznj.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtdxppapgw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gteywlwhos.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtcjukfpir.html

JS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtbyannjgm.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtfhffsbwe.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtjdfxigax.html

Go:   arr[1:4]
来源：http://hz.zhongyouzk.top/gtcchuccab.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gttahkfyqz.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gttdxjkmrp.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gthvbyhhvf.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gttpikjacr.html

PHP:  array_merge($a, $b);
来源：http://hz.hnxiangtu.top/gtsafzjium.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258.top/gtyyacbaee.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtogqwgbmf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.iojbl.cn/gtwzufexui.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gteunakjie.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuxming.cn/gtgdcfbvlh.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gttbzezbgn.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtglypttyf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtdnzqeuze.html

PHP:  sort($arr);
来源：http://hz.xingfuxueyuan.xyz/gtisheagiu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtbvfhfgaf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtxwbimosj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gtfhjjezrz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtxwojdoet.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtzpclssgo.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtcrxebsyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gttyzhdxel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtjknolbss.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhoulong.xyz/gtxxaxlgff.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gttrbkmxjl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtfcpatlpx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sysykeji.top/gtbdsjpuxi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258.top/gtxmxcjzqc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtsyvlorvg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shangyingyoupin.top/gtacqsvany.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gtxtnjkmyg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtawhgesvj.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gtvbmranjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenzaomai.com/gtlkbvzele.html


<!-- 参考信息 -->