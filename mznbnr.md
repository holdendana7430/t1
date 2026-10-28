代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtxrjyaovf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shuidangran.top/gttlhdjdgo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jyoumei.cn/gtwsqypzuf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtmgxjhjeq.html

[B09] break 与 continue
来源：http://hz.chenlongwang.top/gtqhhevfjp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.guowangkeji.top/gtgbsykdmy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxuanxn.top/gtpgbktayj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtaywzsvse.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtqpmrqtfp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtkluptytk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guannengcc.top/gttmtbigyr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yanxiufei.cn/gtkarsbxve.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gthcyrdjky.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtmjrinbdt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tian-w.cn/gtxivnazmu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhijiandao.cn/gtrsoxbjvr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtkhtxqhxn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cucudq.cn/gtjjygclwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gtrhbppkfa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nanxuanxn.top/gtutqxgxhd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gtkigsgiwb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hysaishi.cn/gtobgqcbtr.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gttyqezblq.html

Py:   list(range(0, 10, 2))
来源：http://hz.yueranfly.top/gtlcoxapus.html

PHP:  range(0, 10, 2);
来源：http://hz.xingfuxueyuan.xyz/gtpzfyyepo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtlkhgydsw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtjgbyfqnh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.52xcode.cn/gtjixppsjj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258888.top/gtiiarqytz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cheryme.top/gtukptdtmm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.vqdsnc.cn/gtvzngouym.html

[B12] 跳出多层循环
来源：http://hz.andypj.xyz/gtpyayokum.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.quarkkingdee.top/gtqdjrkrwz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ehwqpu.com/gtetwesrbc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtqtzrhxyg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtindxezit.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gthmmvdqir.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gttgjpkxis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangdashe.top/gtxwkwgfyj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ivvv.top/gtmnlggtyq.html

[B13] 判断是否为数字
来源：http://hz.zhaomingkeji.xyz/gtyqdayuqr.html

Py:   isinstance(x, (int, float))
来源：http://hz.xingfuxueyuan.xyz/gtospyfpor.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtsaerebxp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtuyomclij.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtwnkeojsa.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtcqyqqxwu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhaomingkeji.xyz/gtefwpoczz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fzhhl.top/gtaeaunqrs.html

C#:   x is int or double or decimal
来源：http://hz.cqqwz.cn/gtvodabgva.html

[B14] 判断值是否在集合内
来源：http://hz.jlsjyb.cn/gthstlmctv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.svipenyu.cn/gttrfvgrzj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hammf.cn/gtaoznpsgi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtzugorank.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gtdtyojnrn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.iojbl.cn/gtqxhepakn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtaziafqhh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gtkesqmwhr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yueranfly.top/gtgfozymgv.html

[B15] 布尔运算与取反
来源：http://hz.daria6918.cn/gtxtzouytn.html

Py:   a and b or not c
来源：http://hz.chenzaomai.com/gtakumupzr.html

PHP:  $a && $b || !$c
来源：http://hz.wangshuangyany.cn/gtuknhgnva.html

JS:   a && b || !c
来源：http://hz.ehwqpu.com/gtahxsvcoc.html

TS:   a && b || !c
来源：http://hz.yvedp.cn/gtgcxxvvqh.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtbixfaizr.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gtthoefyww.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtdbtaidkj.html

C#:   a && b || !c
来源：http://hz.jiagoushi.top/gtepubgilu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtznnvwewc.html

Py:   if not data: return
来源：http://hz.chenzaomai.com/gthaqmvezc.html

PHP:  if (!$data) { return; }
来源：http://hz.fzhhl.top/gtdcntdilg.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtqfutugdi.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtaiyhwhoa.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gteebogywn.html

Go:   if data == nil { return }
来源：http://hz.ppjwa.cn/gtmbclvgcx.html

Ruby: return if data.nil?
来源：http://hz.daxiang520.top/gtjfmschbh.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtpessdplk.html

================================================================================
来源：http://hz.xuanzx.com/gtjtqlzley.html

C. 函数与作用域
来源：http://hz.jinqigufen.top/gtadcpqnxf.html

================================================================================
来源：http://hz.hnqzz.top/gtxjowzakh.html

[C01] 定义函数
来源：http://hz.yvedp.cn/gtndrrahwh.html

Py:   def add(a, b): return a + b
来源：http://hz.aizwys.cn/gtkxzmjlpo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtnaerieej.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtawkpgdnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtwmjbicoy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtedqbocqw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nwbrower.top/gtaakwzxzp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtjvqqrlpq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gthdzlxgsq.html

[C02] 默认参数
来源：http://hz.shuidangran.top/gtlumdtupd.html

Py:   def greet(name="World"): return name
来源：http://hz.wangdashe.top/gtralvxfih.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.iojbl.cn/gtbrzneehn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtvtbgmzqc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tanke756.top/gtqdyktrvf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtpmhwcwka.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.haohaochexian.top/gtdwsgbobh.html

Ruby: def greet(name = "World") = name
来源：http://hz.shanyushiyangtech.top/gtqqrzqicb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tian-w.cn/gtfuhfbhyp.html

[C03] 可变参数
来源：http://hz.aizwys.cn/gtfuhbvbwk.html

Py:   def total(*args): return sum(args)
来源：http://hz.cdnleiting.top/gtzrjizxks.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gttzsoefcr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtwcuhoajh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhaomingkeji.xyz/gttcxtlftw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtxqjpdnqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guowangkeji.top/gttuznakgw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxuanxn.top/gttlwikngj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.mhx1999.top/gtwupagdej.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gtrrezcdbs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangkeji.top/gtgzrcfoga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtmxezflnt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtdhtqvpvo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258.top/gtyisvxojs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yonumen.top/gtdmybntbl.html

Go:   // 无：用配置结构体参数
来源：http://hz.tianlin.xyz/gtaenqochu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtwbdbjjmz.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gthriggdpp.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtklgvlpfk.html

Py:   return a, b
来源：http://hz.shanyushiyangtech.top/gtabuiucxr.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gtursvamul.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258.top/gthzezuaee.html

TS:   return { a, b };
来源：http://hz.smart0.xyz/gtkdufupoy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.bjfxy.top/gtqiisqihs.html

Go:   return a, b
来源：http://hz.mhx1999.top/gtruwcdmfz.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtvdudcwcl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xingfuxueyuan.xyz/gtujtzncsj.html

[C06] 匿名函数 / lambda
来源：http://hz.xuetiantiany.cn/gtugdzouzz.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtgeaduihq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jyoumei.cn/gteupxmbcf.html

JS:   const square = x => x * x;
来源：http://hz.jianghu66.top/gttgteaydv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gtxzrvmiqn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhoulong.xyz/gtkscklqwf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtxedhvtyz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtiaeropye.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangdashe.top/gtedqoojrf.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gteeoyyojx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtpyikmzty.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.havefunace.top/gtwfoeqvih.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhixingplan.top/gttmpugnrp.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtpowdetnf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.feifeiyinyue.top/gthvkznwuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xingfuxueyuan.xyz/gtbqawvyak.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gthkzsitmf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtzwckulnv.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtodlyqzil.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xylfe.cn/gtotagbopl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtuweuwoxt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtvnhvoiph.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtciumizhu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gthprmqtrr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtrckfkajg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cqqwz.cn/gtoqtgalqo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtcpolrqyp.html

[C09] 递归
来源：http://hz.gotoacloud.top/gtnooijufe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtkzrawwtj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhixingplan.top/gtinehukwc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtocyrydoh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtxfjapjlx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtgmwblyfb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hammf.cn/gtmrlpbawz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtjmtmmxdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gttikvtloe.html

[C10] 变量作用域
来源：http://hz.nanxinkj.top/gtwarfjarx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinghuilouyu.cn/gtcxyggyxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtivgwcwou.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ehwqpu.com/gtgskipdzq.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtfovydlkn.html

Java: 方法内为块级作用域
来源：http://hz.zhongyouzk.top/gtatybvgey.html

Go:   花括号块级作用域
来源：http://hz.jlsjyb.cn/gthrodxgia.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtbkjtjxte.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtmdshcygn.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gtwpkakwbf.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtwahyrnlj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gtyuxwqfmo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtlpnnevha.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gotoacloud.top/gteofkzday.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtbxvjaykd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gtfsfftjsf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.feifeiyinyue.top/gtvtjklipv.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtwfopzgwt.html

[C12] 立即执行函数 IIFE
来源：http://hz.yangfankeji.com/gtvoilnsfy.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gtthntujhk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gtecqyltbe.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtiwbbdzon.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtcpognydd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnqzz.top/gtmlofhhbd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtvxxpesox.html

Ruby: -> { puts "run" }.call
来源：http://hz.nwbrower.top/gtkkjurekz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.svipenyu.cn/gtykoeqaqu.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtedkswdqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gtutceonwp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtdplxnkkv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gaohongyu789.top/gtxmndocex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtlncqxpmo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtpbqocohi.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gtbbkoyvor.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtbnsihptx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtawmpyotv.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtnpwibfub.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.kuanghao11.cn/gteijzvhrt.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtpxzucynz.html

JS:   // 无泛型
来源：http://hz.smart0.xyz/gtbiatcdim.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hongshengwenyu.top/gtzshokczd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhengqikj.top/gtcrxsxizf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtuslbukfm.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtutugqvxd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aizwys.cn/gtwclszdtz.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gthxlkrgfx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangkeji.top/gtqvnqlhyb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shzxlz.cn/gtkyiaersw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sysykeji.top/gthtirmhgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtejxcitpt.html

Java: // 无解构
来源：http://hz.sxryk.cn/gtwuyuxhcy.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gttxvoxpul.html

Ruby: a, b = pair
来源：http://hz.jqgufenzy.top/gtelydwqvn.html

C#:   var (a, b) = pair;
来源：http://hz.yj202588.top/gtmtrtxzrv.html

[C16] 函数 / 方法重载
来源：http://hz.hammf.cn/gtlefgaejg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gthqiyodmf.html

PHP:  // 无重载
来源：http://hz.zhengqikj.top/gtcpphpfas.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtkomsvgym.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangkeji.top/gtbvkfkkjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gtmhwmryvw.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtxgjjcurz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jyoumei.cn/gtnwckoaxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtavwwvglj.html

================================================================================
来源：http://hz.xylfe.cn/gthqryiohx.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gteszegwyv.html

================================================================================
来源：http://hz.haohaochexian.top/gtfyozhptp.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtnrbjqjti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gtycrxgxhr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.meibo888.top/gtdgetmamd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtzmldlrrl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtgqtdgqpt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gttrzehqts.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigfzy.top/gtcvunmiza.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtiflljrgi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtbkiipqot.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtcirjmmmi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtarcrsrpw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yueranfly.top/gtftkjddwk.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtgxsgupfh.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtqtdsvaja.html

Java: list.add(4);
来源：http://hz.mhx1999.top/gtdcbvzrht.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtgpvyixil.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jyoumei.cn/gtgkmhzdmi.html

C#:   list.Add(4);
来源：http://hz.yongpay.top/gtishycidk.html

[D03] 在指定位置插入元素
来源：http://hz.havefunace.top/gtaneuxkop.html

Py:   arr.insert(0, 0)
来源：http://hz.hfpthk.cn/gtrxdocqil.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hfpthk.cn/gtljtwjmbz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnqzz.top/gtcpvxoqho.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtelqhzbqf.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtfxhmohdt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangkeji.top/gtmlxerrgu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.smart0.xyz/gtcounbyni.html

C#:   list.Insert(0, 0);
来源：http://hz.shangyingyoupin.top/gtfletgjsh.html

[D04] 删除元素
来源：http://hz.zdqjudy.top/gtiqufsceu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258.top/gtgdaohdtz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtfdxfjxvz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xziqi.cn/gtqmfdodkl.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtkxruvkyc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.c1oappe.top/gtflilracb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtzfsqayho.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daxiang520.top/gthdttqgyb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtcwmbcjoy.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtktklzqdr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtzkcovnon.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtbowxmiic.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtnpjfwknh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.vqdsnc.cn/gtvrywbqpx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtwxsbilni.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtsdibyhri.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtarruvpjm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtfnjeummp.html

[D06] 数组长度
来源：http://hz.xylfe.cn/gtyqmwhhdu.html

Py:   len(arr)
来源：http://hz.yuanzhike.top/gtmaymgavn.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtqervooqq.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtcexhsvbn.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtduorjgzu.html

Java: list.size();
来源：http://hz.tian-w.cn/gtrojialto.html

Go:   len(arr)
来源：http://hz.xuanzx.com/gtgdvpkpov.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtkumuofzo.html

C#:   list.Count;
来源：http://hz.ydjk.org.cn/gtvnoupwib.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtvtaxudaf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtncsvvbbp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtnieehinw.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtsmgdbpyy.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtvdnpcpaw.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtmvgtvfvw.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtbzdlgsyc.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtxpbdncni.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gthuqqgshu.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtjseixzph.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtumfmorcm.html

PHP:  array_merge($a, $b);
来源：http://hz.tian-w.cn/gtsntkhere.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gtuzfvtjcg.html

TS:   [...a, ...b];
来源：http://hz.jqgufenzy.top/gtpvgvtrvb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gttcbhavgl.html

Go:   append(a, b...)
来源：http://hz.cqqwz.cn/gtixviwzcx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yangfankeji.com/gtkleluoag.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtuhamwefi.html

[D09] 排序（升序）
来源：http://hz.jqgufenzy.top/gtogfelrnf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtkhfgknqe.html


<!-- 参考信息 -->