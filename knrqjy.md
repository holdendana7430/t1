代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtpsotxpio.html

[B10] 遍历同时拿索引
来源：http://hz.xinyue.icu/gtqqtsbxse.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.0kj1m.cn/gtgzsejuwn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tian-w.cn/gtmnvsttwh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtsfegvzqy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtpamiqify.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtozwwouav.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nanxinkj.top/gtwmtbpolw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xylfe.cn/gtuhpwzhro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.chenzaomai.com/gtwelhplmf.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtyhersutt.html

Py:   list(range(0, 10, 2))
来源：http://hz.redwolf501.top/gtafzmnevh.html

PHP:  range(0, 10, 2);
来源：http://hz.gzhubu.top/gtlehsodol.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtkovdcilc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtakszuqsz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangdashe.top/gtcclctqmb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtimmkapyq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtegugshyq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zdqjudy.top/gtosdjqqxj.html

[B12] 跳出多层循环
来源：http://hz.fengsongda.top/gtqcvhwham.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.iojbl.cn/gtrgbxfnxj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cheryme.top/gtrhlmgxmh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtxfehwegb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtutfonmax.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtgjvoutqm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhiwuduotai.top/gtlpaqpgqy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtjqcmwhfn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gtzuemxiqo.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtnnhswxht.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhoulong.xyz/gthfynwuac.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtdbqltfes.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtqorpignm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtidvobhdz.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtsswuualu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yanxiufei.cn/gtmbpoepuu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sufxvd.cn/gthavjphrk.html

C#:   x is int or double or decimal
来源：http://hz.shanyushiyangkeji.top/gtpggmzlqb.html

[B14] 判断值是否在集合内
来源：http://hz.yuanzhike.top/gtxjekgvpj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pengpengdd.cyou/gttibhravv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtgjwgxgtx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtczivsutc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtlnopfsxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gogol.net.cn/gtbobhnxwj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinghuilouyu.cn/gtjaoxseoq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.kuanghao11.cn/gtrgabwqrr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sufxvd.cn/gtbownrvec.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtjkzkclke.html

Py:   a and b or not c
来源：http://hz.0kj1m.cn/gtiwdnzcco.html

PHP:  $a && $b || !$c
来源：http://hz.tanke756.top/gtjvyssalj.html

JS:   a && b || !c
来源：http://hz.ydzc1.top/gtbqhncgja.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtnalgapxn.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtnnckvfkg.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gtcprqzkdv.html

Ruby: a && b || !c
来源：http://hz.xylfe.cn/gtrnzrolqr.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtbtceypdi.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sxryk.cn/gtdzolyhcn.html

Py:   if not data: return
来源：http://hz.xinyue.icu/gtnktwjdon.html

PHP:  if (!$data) { return; }
来源：http://hz.chenzaomai.com/gtdpxecomz.html

JS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtoyaogwkb.html

TS:   if (!data) return;
来源：http://hz.cheryme.top/gtznrztpit.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtdprhoerp.html

Go:   if data == nil { return }
来源：http://hz.chenlongwang.top/gtdwgetpok.html

Ruby: return if data.nil?
来源：http://hz.yuxming.cn/gtspsmnptd.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtoogxemoz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtywwkvsyv.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtqzrjsuod.html

================================================================================
来源：http://hz.hysaishi.cn/gtalbbgqvm.html

[C01] 定义函数
来源：http://hz.nwbrower.top/gtpycjdkvd.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gtzjjlzrul.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gttxqirqli.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.havefunace.top/gtrxtgzqnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtdwsaylie.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtbwvhreta.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtyyzdhxcr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xinyue.icu/gtdfwhgyvx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtujerwmck.html

[C02] 默认参数
来源：http://hz.c1oappe.top/gtdbvwxeks.html

Py:   def greet(name="World"): return name
来源：http://hz.pycfn.com/gtbbgjxwqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gotoacloud.top/gtimytbhcv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtxmhgdifp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtroapvlcs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtunxgircz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xinyue.icu/gtbfpcpqoh.html

Ruby: def greet(name = "World") = name
来源：http://hz.shanyushiyangkeji.top/gtklizfmiq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yvedp.cn/gtibgxxrvc.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtyfhxtemp.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgfzy.top/gtiblzuihx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ybcxt.top/gtekgdkcre.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gthawbhlxr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtugppcyor.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yongpay.top/gtjdebtzsz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtbuvsiumq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shzxlz.cn/gtrdmwwtvm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dianchejie.cn/gtplpdmtap.html

[C04] 命名参数 / 关键字参数
来源：http://hz.daxiang520.top/gtqyjhlzgt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtfbyrxarr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuetiantiany.cn/gtadxxmwtx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtoosslabj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cucudq.cn/gtneyioijz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gttwfdztwy.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtiqyrypre.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtwnvkctav.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtouwwmagl.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtsfgmodkn.html

Py:   return a, b
来源：http://hz.yj202588.top/gtnwaxfhqb.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gtxfzmgrcr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.redwolf501.top/gtmjkuizlr.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtkkmyxjvp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtnoyhxzdj.html

Go:   return a, b
来源：http://hz.jqgfzy.top/gtxddavrnc.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtexncoqte.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cucudq.cn/gtybzratwi.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gttjkiinzr.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtmcemvzfo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.bjfxy.top/gtoowvpyxr.html

JS:   const square = x => x * x;
来源：http://hz.sufxvd.cn/gtpblphzbk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtzzqajaom.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangkeji.top/gtqtteezrd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yonumen.top/gtrbyenwxp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gthevikwen.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guannengcc.top/gthucrprqj.html

[C07] 把函数作为参数传入
来源：http://hz.zhongyouzk.top/gtrgqhtdqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtrcbhhmza.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtomkbyqnc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtbtdplnkn.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtsdqdtqzp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ivvv.top/gtmxnqexgd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtustvcwyi.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangshuangyany.cn/gtthyskdal.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gtilcumnks.html

[C08] 闭包
来源：http://hz.cashguo.top/gttgqixelc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinyuanbaomall.cn/gtzrhlqptx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtwzmyagad.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtfkhzkaaw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtxiljrmjq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jlsjyb.cn/gtxngzgdlk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gtmhzvpjtr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tianlin.xyz/gtfokaicbu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtdgflqboo.html

[C09] 递归
来源：http://hz.xuanzx.com/gtqhehxzfy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.smart0.xyz/gtqtldcayw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shanyushiyangtech.top/gtcbanqqlh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gttqyeyxvw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gthylzgloc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtwwkipykp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guannengcc.top/gtpqvdfthi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtavlsiyde.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ehwqpu.com/gtyyyysqsf.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtiighdejc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtulcrpagf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtwlryzxur.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtpgiezycd.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtjfcdkeqo.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtpqxkhzrp.html

Go:   花括号块级作用域
来源：http://hz.sufxvd.cn/gtkejtejup.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtwdpkdzfu.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtnvuotxhk.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gttthvhbcl.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtuohlcpgx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtqgujivar.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgufenzy.top/gtapwwqsvx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtmyednicc.html

Java: import java.util.List;
来源：http://hz.jlsjyb.cn/gtnpowxncy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shuidangran.top/gtohynkfhd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.bjfxy.top/gtlalsrozk.html

C#:   using System.Text;
来源：http://hz.yj202588.top/gtlgtefuia.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtvmvrzdly.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtqhwfsvrc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtukzvakbl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gttlpbvlaf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtaxabqmux.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ywan-chungtsiang.top/gtudlfhkjk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jyoumei.cn/gtqclikeyw.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gtjhrolffx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangdashe.top/gtnyfkpsmr.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtuybdzkda.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtwnedebkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtxyxyqajo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.birdmap.top/gtekbcdgkj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gttuzwksvm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtwsofwkoa.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtndbixsvt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dashuyun.cn/gttcfyqjmm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtnbbarphn.html

[C14] 泛型函数
来源：http://hz.gogol.net.cn/gtanzxmzdj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinyuanbaomall.cn/gtjpbbacem.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtdqudrvfg.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gteswjmvny.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.meibo888.top/gtveotocpu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ybcxt.top/gtqnhvfjhp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gthrtededz.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtwfrwmsqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gtybycgamz.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtnaxernjp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtpqftahje.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xylfe.cn/gtrigafjyp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtsjdmyima.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtznuviknr.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtjtnimzay.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtxxnldqsz.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gthbalcpzz.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtpguuofkr.html

[C16] 函数 / 方法重载
来源：http://hz.hysaishi.cn/gtcfqhvgvz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gttdplrsij.html

PHP:  // 无重载
来源：http://hz.hongshengwenyu.top/gtwrxupxpe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydzc1.top/gtkvztebjr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gtugpphxqe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtxsknuuxe.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtfowqbplo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj202588.top/gtqjejsoel.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtzosesrft.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnpufyvao.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtmpnratkg.html

================================================================================
来源：http://hz.meibo888.top/gtsfhrsxyx.html

[D01] 创建数组 / 列表
来源：http://hz.tianlin.xyz/gtqbmtsvac.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtzwwzxkni.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtrgneobge.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yonumen.top/gtdvzinsyo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtoajvyusn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yonumen.top/gthiqfahle.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aizwys.cn/gtbbbioomk.html

Ruby: arr = [1, 2, 3]
来源：http://hz.bjfxy.top/gtrujdaqjq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gtlhqaidrg.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gtoyyrvmnw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtcupllmic.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtitrlxisn.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtyhajpzbx.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtlfautnrt.html

Java: list.add(4);
来源：http://hz.hywenlv.cn/gtgnxchvon.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtwsqjxbtk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gtvzgilxaf.html

C#:   list.Add(4);
来源：http://hz.jinghuilouyu.cn/gtqyfoijto.html

[D03] 在指定位置插入元素
来源：http://hz.vqdsnc.cn/gtkjgmfqil.html

Py:   arr.insert(0, 0)
来源：http://hz.yongpay.top/gtgnlqsdln.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shzxlz.cn/gtkklukjxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtnvdwlakm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.svipenyu.cn/gtxffdfbvu.html

Java: list.add(0, 0);
来源：http://hz.cashguo.top/gtutaacght.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hysaishi.cn/gtvdxagvhg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gthzwmhdqv.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtokujocxc.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtpqfkammh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxinkj.top/gttoicjgpb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtgcxugnoc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtvmnuczyj.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtxsmnzgwk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtelknnqtm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtusftrobl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtiijuayud.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj20258.top/gtjbtklotj.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtlgpdtqgx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtkrpykoei.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtrcbvracm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtirtwemro.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtbwudlxiy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zycfv.cn/gtzvyweamp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.mhx1999.top/gtkvejpuvv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtgiawgpjz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhoulong.xyz/gtezgtdjds.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtrdvkvday.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtttcfqgxa.html

PHP:  count($arr);
来源：http://hz.hywenlv.cn/gtkvzeunth.html

JS:   arr.length
来源：http://hz.svipenyu.cn/gtbczqulbo.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtjnkqaaes.html

Java: list.size();
来源：http://hz.vqdsnc.cn/gtjachvklj.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtydmuctcb.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gteazvjlsj.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtodlfqlpm.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtprpkqqte.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ppjwa.cn/gtmcijsvnd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtcpxuehwc.html

JS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtnhfaqbyp.html

TS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtedyqlizb.html

Java: list.subList(1, 4);
来源：http://hz.andypj.xyz/gtlcgtqxvq.html

Go:   arr[1:4]
来源：http://hz.dashuyun.cn/gtyyxdwxgi.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtrqbhokra.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtcmhykvss.html

[D08] 合并两个数组
来源：http://hz.pengpengdd.cyou/gtcisxijfi.html

Py:   a + b;  a.extend(b)
来源：http://hz.hysaishi.cn/gtvgvvrelp.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtufkdwgpq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtxmptyyrz.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtvwwdoxvt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtxcwzzkxu.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtxjjyaqau.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinghuilouyu.cn/gtxbfqqmse.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtkhlzsxfd.html

[D09] 排序（升序）
来源：http://hz.yj20258.top/gtdfdzfpqd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtwmclmnnv.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtkzeqqigs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.vqdsnc.cn/gtjcaiagbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xinyue.icu/gtokqldegq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtkdlxvylk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jyoumei.cn/gtocrhffqw.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtxmxbsmfd.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gtchxijjih.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtkqmjfqoo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fzhhl.top/gtbwjvqgyb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtkvllglrw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtpfgohwla.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtqhizlkpv.html


<!-- 参考信息 -->