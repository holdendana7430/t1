代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gzhubu.top/gtcodqnemk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxuanxn.top/gtfelagkwn.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtyvhllvty.html

[B08] do-while（至少执行一次）
来源：http://hz.daxiang520.top/gtgwymuoai.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.quarkkingdee.top/gtcubnmykw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yueranfly.top/gtxxoprlna.html

JS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtxiplvjnb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtmtyzfzte.html

Java: do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtmfboolmj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj202588.top/gtqwvhfjmh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinyuanbaomall.cn/gtykzovjbu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtknuczfts.html

[B09] break 与 continue
来源：http://hz.hfpthk.cn/gtkbybnrzo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jyoumei.cn/gtaqonwnhu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gtembfihgt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtmxhqqbft.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtdfoqdzbb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtkxbqfikh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ivvv.top/gtvogqnprn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.wangshuangyany.cn/gtnmitlmhq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtbdrbucme.html

[B10] 遍历同时拿索引
来源：http://hz.jlsjyb.cn/gtcqwthhhc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtbvlixbey.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.havefunace.top/gtdidqhynn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ybcxt.top/gtldgrwdju.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sweek.top/gtkiajdelp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ybcxt.top/gtbgdjsctt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.0kj1m.cn/gtxeayznue.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sweek.top/gtbuuyqjaw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hysaishi.cn/gtnkrzcocn.html

[B11] 生成数字序列 / 区间
来源：http://hz.jianghu66.top/gttblnvxkh.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhoulong.xyz/gtrgdfwsva.html

PHP:  range(0, 10, 2);
来源：http://hz.nwbrower.top/gtjmmzmtps.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.meibo888.top/gtiqxsuzon.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtovpebjxz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gttuyypmaj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtprgzecmu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuanzx.com/gtksaruail.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sxryk.cn/gtlskxerwl.html

[B12] 跳出多层循环
来源：http://hz.svipenyu.cn/gtejlxolzs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yangfankeji.com/gtozzmmwrq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtwfmdanin.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gogol.net.cn/gtwdsslqab.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gttftisivr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtktiehxxb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dashuyun.cn/gtjrnqgzts.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtebjbbfip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xingfuxueyuan.xyz/gthvoqpbef.html

[B13] 判断是否为数字
来源：http://hz.cucudq.cn/gtduvsyjfv.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtflfonvlz.html

PHP:  is_numeric($x)
来源：http://hz.birdmap.top/gtrlikmxmy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shzxlz.cn/gtnotbktdd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtaxuzyyoo.html

Java: x instanceof Number
来源：http://hz.daria6918.cn/gtqdyuxdbv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hnqzz.top/gteaydfyvb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuetiantiany.cn/gtqxkbfvpi.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtmqfkwetg.html

[B14] 判断值是否在集合内
来源：http://hz.sxryk.cn/gtdcallvjv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtdeotnfrl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.snrcjt.cn/gtnepnnwuk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xuanzx.com/gtngxliwix.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtqfqgzkox.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yanxiufei.cn/gtddkgtjvz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cdnleiting.top/gtajyjucqq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtfvdpjnqg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtwfzmhggc.html

[B15] 布尔运算与取反
来源：http://hz.ppjwa.cn/gtfdlvanzi.html

Py:   a and b or not c
来源：http://hz.cqqwz.cn/gtprvykbmf.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtgtahobfv.html

JS:   a && b || !c
来源：http://hz.0kj1m.cn/gtbvxkdckm.html

TS:   a && b || !c
来源：http://hz.aibaodan.cn/gtnqtlitfn.html

Java: a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtjenuzoxy.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtltqjycoo.html

Ruby: a && b || !c
来源：http://hz.shzxlz.cn/gthhcdhvge.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gtmfvwemrj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhaomingkeji.xyz/gtllndxuhh.html

Py:   if not data: return
来源：http://hz.hnqzz.top/gtwejygqmu.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gtqwrndcfh.html

JS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtcpaeoigp.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtnbpfylzp.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtiinzvyfn.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gtvsnjzgig.html

Ruby: return if data.nil?
来源：http://hz.zycfv.cn/gttryqrvdb.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtagusdpdk.html

================================================================================
来源：http://hz.ehwqpu.com/gtmitpfbdm.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtvmrmbkog.html

================================================================================
来源：http://hz.havefunace.top/gtzgubwjmc.html

[C01] 定义函数
来源：http://hz.chenjidiqi.icu/gtxlpnvain.html

Py:   def add(a, b): return a + b
来源：http://hz.zhengqikj.top/gtdnaqjoqw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtbwpfwoiu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtulleqavy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtkgenwtnh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtszbdrdzd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhijiandao.cn/gtzgmaqvhz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gticsncgag.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtdsspfznk.html

[C02] 默认参数
来源：http://hz.hammf.cn/gtlswmpksv.html

Py:   def greet(name="World"): return name
来源：http://hz.shuidangran.top/gtbrhmezqw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ivvv.top/gtdiipcvrz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangkeji.top/gthamfhcac.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.0kj1m.cn/gtlknlolnc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtlhtvjsox.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtijazxfny.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtnbdyawrn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtprxtwthq.html

[C03] 可变参数
来源：http://hz.chenlongwang.top/gtmhbehdmr.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtyotkrexp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtbnbfwgng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtoqksjhxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtmgwidvgw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtlvogmllj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtvfkljegv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtocqpjmpg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtwyrqdkgf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aizwys.cn/gtjbtzergj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gtobqqhznh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gaohongyu789.top/gtakwlsynz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtljpcplja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenzaomai.com/gtgiaumpet.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shuidangran.top/gtvwgxtbti.html

Go:   // 无：用配置结构体参数
来源：http://hz.shzxlz.cn/gthvwzvzal.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtvgcywnqx.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtphyukfbs.html

[C05] 返回多个值
来源：http://hz.pycfn.com/gtikkkwtzg.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtgoylnsij.html

PHP:  return [$a, $b];
来源：http://hz.zhongyouzk.top/gtkrrhoemw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtrovbctue.html

TS:   return { a, b };
来源：http://hz.zhongyouzk.top/gtnfwolicd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258.top/gtmudkrkco.html

Go:   return a, b
来源：http://hz.yj202588.top/gteglvjcwo.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gtngmbipbh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jqgfzy.top/gthsvztwku.html

[C06] 匿名函数 / lambda
来源：http://hz.dianchejie.cn/gtvblxexuq.html

Py:   square = lambda x: x * x
来源：http://hz.c1oappe.top/gtvgmmmvvo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xziqi.cn/gtavzapviq.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtunbszxef.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtefqmhmdt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jiagoushi.top/gtbpuplxam.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.c1oappe.top/gtjtyqspbd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtvyqtlvgj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtdhozahib.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtdnpmkdpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.wangdashe.top/gtgitmysgt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daria6918.cn/gtlivalvza.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtwoiujgpz.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gtyfvbodjy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pengpengdd.cyou/gtnosigbec.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gtnahlguan.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinyuanbaomall.cn/gtcvtxutrh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tian-w.cn/gtxubfhoss.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gtlaluoekb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sysykeji.top/gtigsgxvzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnqzz.top/gtrlhnnwks.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtcqvgtivc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtgykkbsol.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hfpthk.cn/gtgjdonjkd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj20258.top/gtclceocff.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hammf.cn/gtuopptbpg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtvqlkgqve.html

[C09] 递归
来源：http://hz.tian-w.cn/gtjvtqthrx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258888.top/gtbvfzxtwb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gogol.net.cn/gtokdowzyt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtapwqqspb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ybcxt.top/gtcboxqjzc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtmvnibtnz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtuttpoekg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtkajuzuvr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gtkawldigo.html

[C10] 变量作用域
来源：http://hz.shangyingyoupin.top/gtfpsqjcho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gtutlgshrh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gttyyblgih.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gttpgjdhim.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtyfbnpttm.html

Java: 方法内为块级作用域
来源：http://hz.gotoacloud.top/gtygjrazqg.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtnzgkjpac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hysaishi.cn/gtsjpyajzh.html

C#:   块级作用域
来源：http://hz.fengsongda.top/gtgjjxpiia.html

[C11] 模块导入与导出
来源：http://hz.wangshuangyany.cn/gtjrpzxtwg.html

Py:   from module import func
来源：http://hz.xinyue.icu/gtxzqrzebw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gtyhghjxan.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtcwjedlgq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigufen.top/gtnxxncarp.html

Java: import java.util.List;
来源：http://hz.iojbl.cn/gtlfnqmirq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.snrcjt.cn/gtjvctxoqc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtwfhvcybk.html

C#:   using System.Text;
来源：http://hz.jyoumei.cn/gtvneasxuk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gtcrdtqzcq.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtfgkhxgdp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtftvvyxqg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtjuvapztr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtiuwdgtmt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yvedp.cn/gtrnhjsnpo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gtvwnrkczk.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtbiqcloka.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtezwnmtsd.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtkamryvpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xingfuxueyuan.xyz/gtdpeyrpru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtlnbkktvg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cheryme.top/gttiiklndi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtbuqvecxl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtbgzawgzj.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gttrjvcahj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shuidangran.top/gtljcvmzev.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtzvawpkwc.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtfcpbdekk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xingfuxueyuan.xyz/gtqjjsjvkn.html

PHP:  // 无泛型
来源：http://hz.iojbl.cn/gtdmfywvny.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtsvjyawtt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.smart0.xyz/gttpxljnhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtatjdnfxy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtroxhuebe.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtkkvjpuvi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtglbinguj.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtyhtyhley.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtggctmskz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.kuanghao11.cn/gtgxlnynhs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtdnlxjzld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hysaishi.cn/gttiylcucp.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtggiabulk.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtpdfhncmg.html

Ruby: a, b = pair
来源：http://hz.hfpthk.cn/gtxisxnpxd.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtqrepfunx.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtfcztoquk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sufxvd.cn/gtnxeknxht.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtrgteiaie.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtrmakyfgj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yueranfly.top/gtcjtggusk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gthmpxpheg.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtqrsufmxd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtnlrrfxsl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtjacesftf.html

================================================================================
来源：http://hz.xuanzx.com/gtczrifwqt.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gthukzdpze.html

================================================================================
来源：http://hz.jianghu66.top/gthawqcfce.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gthiqtxmtj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtotxzyceg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guowangkeji.top/gtazycsgnk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dianchejie.cn/gtvgzhcyxh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuanzhike.top/gtmyfddpxc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhixingplan.top/gtrjrmhgov.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.quarkkingdee.top/gthtrezyxr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ydzc1.top/gtsfhisdqd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtqretgeiz.html

[D02] 追加元素到末尾
来源：http://hz.daria6918.cn/gtlhubtipw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hnqzz.top/gtmuzcbixi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtxwpposxh.html

JS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtkozfqwly.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtsjawukgt.html

Java: list.add(4);
来源：http://hz.316326.xyz/gtpinwlsqk.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gttjtveawu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnqzz.top/gtuxmsjxqt.html

C#:   list.Add(4);
来源：http://hz.feifeiyinyue.top/gtgkidklsi.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtvzynvith.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gttpptasni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.snrcjt.cn/gtsnuszxrx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sufxvd.cn/gtstyktdds.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hfpthk.cn/gtblbwjety.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtuxlkdzic.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ivvv.top/gtjvkdbtry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtxicdxksd.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtgufjjtwt.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtnwmsnlyx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtjpzaqucz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dashuyun.cn/gtakucupbq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ywan-chungtsiang.top/gtqddqlhvy.html

TS:   arr.splice(0, 1);
来源：http://hz.sufxvd.cn/gtvatiptzo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtfogrofhn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gtnsclqrcu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtsiedklqk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tian-w.cn/gtbfrrytao.html

[D05] 访问与修改元素
来源：http://hz.kuanghao11.cn/gtipqysfhy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtgeampxeq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ppjwa.cn/gtsjgvlwpf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sysykeji.top/gtfwplhjko.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtstfzkpfy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnqzz.top/gtfwetbgcv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtvquvwzsv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtkqrcudpg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtiwqixwso.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtrmvmpwmm.html

Py:   len(arr)
来源：http://hz.jiagoushi.top/gtdccgfloz.html

PHP:  count($arr);
来源：http://hz.daria6918.cn/gthczaggon.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtdohkmkjy.html

TS:   arr.length
来源：http://hz.sweek.top/gtbtwmrkrt.html

Java: list.size();
来源：http://hz.tianlin.xyz/gtapunqxyw.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtqlqroede.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gteljmtcjq.html

C#:   list.Count;
来源：http://hz.xziqi.cn/gtjuxwfdfz.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtcebvqiin.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gtctgmcuej.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtjdlvcqkl.html

JS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtpteiccgg.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtsclrinnr.html

Java: list.subList(1, 4);
来源：http://hz.hnxiangtu.top/gtqfbyxqvu.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtsqwodidw.html

Ruby: arr[1, 3]
来源：http://hz.gotoacloud.top/gtfxywsgpv.html

C#:   list.GetRange(1, 3);
来源：http://hz.ywan-chungtsiang.top/gtmxkosbzv.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gttcobnuoj.html

Py:   a + b;  a.extend(b)
来源：http://hz.jiagoushi.top/gtugnukqov.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gtukzflvkp.html


<!-- 参考信息 -->