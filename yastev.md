代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinghuilouyu.cn/gtvdgawbjz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj202588.top/gtiptyxbmz.html

C#:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtfvgybcbs.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtpgvwegaq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hywenlv.cn/gtsydqtabz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jinqigufen.top/gtlqsljymu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gtxdbvbwhj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtajtaxjxe.html

Java: do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gthmywduop.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cdnleiting.top/gtrslufeeb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtanotfcoh.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtjvercyhm.html

[B09] break 与 continue
来源：http://hz.redwolf501.top/gtxqhrpzqm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gtcirsdgkt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shzxlz.cn/gtbxqrutru.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gthcvmvebf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtpegxqxhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtuhommohy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtfkquddpl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gtuhvirugk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtqfbpketm.html

[B10] 遍历同时拿索引
来源：http://hz.gaohongyu789.top/gthnpkltpd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ppjwa.cn/gtczmofpce.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhongyouzk.top/gtzhctnbiw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jyoumei.cn/gtjcpoltpq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj20258888.top/gtnicudtjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj20258.top/gtvemcnqwo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.iojbl.cn/gtdwenbtct.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cucudq.cn/gtsqmjgxnk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zdqjudy.top/gtmwqsvalx.html

[B11] 生成数字序列 / 区间
来源：http://hz.tanke756.top/gtlnhuqctf.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtdiperuoq.html

PHP:  range(0, 10, 2);
来源：http://hz.316326.xyz/gtawxoqokl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtnlsuypzr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtasizbyrt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cqqwz.cn/gtdcoqoxgm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tian-w.cn/gtikvkosim.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yvedp.cn/gtzryuoqdd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hnxiangtu.top/gtmaoxwzgg.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtsynycnxf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.guowangkeji.top/gtjftmzvud.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gotoacloud.top/gtwiinnjnh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtukcrzmym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtqtdgarqa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtjlyluner.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gthdlpdsub.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xziqi.cn/gtpttktinj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cheryme.top/gtqtelmtqp.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gttuvnbxgz.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxuanxn.top/gtzhcimahi.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtookluiyj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtmmnvumuf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tianlin.xyz/gtslvpdnog.html

Java: x instanceof Number
来源：http://hz.chenlongwang.top/gtjtelifdo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxuanxn.top/gtrvflknvy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.vqdsnc.cn/gtsvnmnjkz.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtpkvlcamn.html

[B14] 判断值是否在集合内
来源：http://hz.feifeiyinyue.top/gtowoohict.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gterofewoh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gogol.net.cn/gthnwoivab.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtcopkebwk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtfumavpbe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.smart0.xyz/gttvtlmivo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gthddtqkpj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yanxiufei.cn/gtjijlzwry.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gtlkoriqqt.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtknavdkvc.html

Py:   a and b or not c
来源：http://hz.shanyushiyangtech.top/gtlbzzxxcl.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtibvxxjhe.html

JS:   a && b || !c
来源：http://hz.svipenyu.cn/gthnjacoea.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gtheurkunn.html

Java: a && b || !c
来源：http://hz.tianlin.xyz/gtwgshepjq.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtynqpohgf.html

Ruby: a && b || !c
来源：http://hz.chenlongwang.top/gtcrhcdesk.html

C#:   a && b || !c
来源：http://hz.cucudq.cn/gtrhiykeka.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtlpnpgksf.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtcswgfynl.html

PHP:  if (!$data) { return; }
来源：http://hz.zhijiandao.cn/gthvuuckin.html

JS:   if (!data) return;
来源：http://hz.ivvv.top/gtzldwbrve.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtxnxryfzr.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gtmboisegn.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gtojuwtydg.html

Ruby: return if data.nil?
来源：http://hz.zdqjudy.top/gtqletsujq.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gtynqftfig.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlrwzagbq.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtohuytpjy.html

================================================================================
来源：http://hz.sysykeji.top/gtjmyiggkc.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtgyiahsps.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtguopbisx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.kuanghao11.cn/gtkbtelqqf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtbrgppamz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtvqejxhcb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtguwqragr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtwfmspzhw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guowangkeji.top/gtghxdlhru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtdzpgsfga.html

[C02] 默认参数
来源：http://hz.feifeiyinyue.top/gtesoypvst.html

Py:   def greet(name="World"): return name
来源：http://hz.vqdsnc.cn/gtwpxcseuv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gtiktymjai.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.haohaochexian.top/gtdxizicxo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtaipribir.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gtzoqmbpvc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daxiang520.top/gtedshelgp.html

Ruby: def greet(name = "World") = name
来源：http://hz.mhx1999.top/gtvoxxqhix.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.quarkkingdee.top/gtkrmptxgp.html

[C03] 可变参数
来源：http://hz.nanxinkj.top/gtafqfyrep.html

Py:   def total(*args): return sum(args)
来源：http://hz.sweek.top/gtalfspkgk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guannengcc.top/gthdiwdnkq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtadzwzmpc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtbbtsbzig.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtfttfpqkx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hongshengwenyu.top/gtrqrxqxed.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gtxfbclzzi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtvtpxcxic.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinghuilouyu.cn/gtuvfkfwfy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.vqdsnc.cn/gtuknfghbs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtugzeaibs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtlmrkcuvn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guowangkeji.top/gtjesikipy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gttcurnrzk.html

Go:   // 无：用配置结构体参数
来源：http://hz.nwbrower.top/gtlssnuoku.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtlznlgmmz.html

C#:   f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtftzjspst.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gtgqxgbize.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtybqcttiv.html

PHP:  return [$a, $b];
来源：http://hz.haohaochexian.top/gtsdhphirg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gtrqjlndaq.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtcypuggxb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gtetfgwpkl.html

Go:   return a, b
来源：http://hz.gzhubu.top/gtxkxncqlv.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtjxuqvhsx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtvjitwgzs.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxuanxn.top/gtputrcoar.html

Py:   square = lambda x: x * x
来源：http://hz.wangshuangyany.cn/gtrvbrkbkm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xinyue.icu/gtupckjfxm.html

JS:   const square = x => x * x;
来源：http://hz.jinqigfzy.top/gtykbjakyx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.vqdsnc.cn/gtouftgajw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gtzezfnrjj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zdqjudy.top/gtisgvmawh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dashuyun.cn/gtdkywmaoy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtyzsmlctr.html

[C07] 把函数作为参数传入
来源：http://hz.tianlin.xyz/gtlzooyjeu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shuidangran.top/gthoqrwgde.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtuztxcdql.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sufxvd.cn/gtqpuwratp.html

TS:   arr.map(String)
来源：http://hz.ywan-chungtsiang.top/gtihlxbyax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtrhoxlhtq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtomsfduqg.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtudwwimfr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gtohpuzvjg.html

[C08] 闭包
来源：http://hz.yj20258888.top/gtjeoqzpkg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hysaishi.cn/gtkaydfjeg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shuidangran.top/gtfculhwsd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtmdetorne.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtnhjluozk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nwbrower.top/gtqhikhbbr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigfzy.top/gtxluzvoki.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ppjwa.cn/gtdpeqcztj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtwpoojnyo.html

[C09] 递归
来源：http://hz.316326.xyz/gtwmkxdwpx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgfzy.top/gttyjnpuxo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jiagoushi.top/gtepfrilck.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtdewbwdyj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtmciokrvy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtpettybja.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.redwolf501.top/gtpmlbvitq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtlnrnpvxo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtdwofbyle.html

[C10] 变量作用域
来源：http://hz.shanyushiyangkeji.top/gthobqyucb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gtaixubvum.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtizpfmiaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daria6918.cn/gtutkihhmr.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtjtkyjvlp.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtrielslzk.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtrgqwurxw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtvmrsyfut.html

C#:   块级作用域
来源：http://hz.chenjidiqi.icu/gtmjntvkcz.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtyjfpkbaz.html

Py:   from module import func
来源：http://hz.hnxiangtu.top/gtmsgnfeco.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cashguo.top/gttvmejbyp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuxming.cn/gtikfrwgnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtydzgiymb.html

Java: import java.util.List;
来源：http://hz.xylfe.cn/gtndnvbkol.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtfubpzrig.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.bjfxy.top/gtorzzzrac.html

C#:   using System.Text;
来源：http://hz.xuetiantiany.cn/gttwtpcqxh.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gtblouujai.html

Py:   (lambda: print("run"))()
来源：http://hz.jinghuilouyu.cn/gtvnwnxvnf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtqtalstxk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtmxvurwzd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gttbdearuf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtmwhvqriq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gteugjhyqf.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gteszqriea.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtxeycrbqb.html

[C13] 类型声明 / 类型注解
来源：http://hz.jiagoushi.top/gtnsworneb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydjk.org.cn/gtapzafyls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtmeupszag.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.c1oappe.top/gtpozlmqzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtaeetjzlk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtryinghkd.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtyuybkwbr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtfecodfgj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangtech.top/gtxjdayzoj.html

[C14] 泛型函数
来源：http://hz.svipenyu.cn/gtqjzwkima.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258888.top/gtmomxenij.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtcccxfbwd.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtvobdxaji.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtdsuaetql.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtloowaags.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtfmkrpfxx.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtffguevxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtrdesspli.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtpqneeykb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtjfcohfwe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtpfwnlwnd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtwymsgqvz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtacsmmbcn.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtvwiplqly.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtavznrhvq.html

Ruby: a, b = pair
来源：http://hz.smart0.xyz/gtcmpsozxk.html

C#:   var (a, b) = pair;
来源：http://hz.fengsongda.top/gtziqmqwrf.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gtsfkwqriq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtphdpsujz.html

PHP:  // 无重载
来源：http://hz.zdqjudy.top/gtwuwquzps.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtbhdgsagd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtzvtmhpkh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gaohongyu789.top/gtikacoxik.html

Go:   // 无重载：用不同函数名
来源：http://hz.svipenyu.cn/gtnjfnvbvh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtrwerfbpl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtkihfunkx.html

================================================================================
来源：http://hz.xinyue.icu/gttuoaqtkb.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtwkdyflfk.html

================================================================================
来源：http://hz.zhengqikj.top/gtezlafylf.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtozfksufs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtwnkjeqdj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtqtvwfhvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtucpeixpp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yvedp.cn/gtrxjbddyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydjk.org.cn/gtcjzayflh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtptqzuotp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtpoqizqks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ywan-chungtsiang.top/gtqtouhwqe.html

[D02] 追加元素到末尾
来源：http://hz.gotoacloud.top/gtpmguvfqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtjkubdfff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.meibo888.top/gtaoramkqq.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtxpjdphji.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtawrbdygo.html

Java: list.add(4);
来源：http://hz.cdnleiting.top/gttcalijut.html

Go:   arr = append(arr, 4)
来源：http://hz.quarkkingdee.top/gtzximjfgy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gttyqxlfpv.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtxouonobv.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtazvgrlxb.html

Py:   arr.insert(0, 0)
来源：http://hz.yangfankeji.com/gtrxmprqjd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtmsgasgqr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuxming.cn/gtsfbtvtmy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.fengsongda.top/gteijmexzr.html

Java: list.add(0, 0);
来源：http://hz.sxryk.cn/gtbidjuvfo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtsghubbwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gtlwcwofms.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtfvspuvty.html

[D04] 删除元素
来源：http://hz.cheryme.top/gtehpqxhho.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtuffmlkhw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydzc1.top/gttadhhazi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.vqdsnc.cn/gtslzddxlm.html

TS:   arr.splice(0, 1);
来源：http://hz.zhixingplan.top/gtsnovyufp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenlongwang.top/gtvswsamjj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhengqikj.top/gtiucbnvcq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258888.top/gtwkoydiix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gthpnvtdke.html

[D05] 访问与修改元素
来源：http://hz.shuidangran.top/gtbulthuwz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtzjlwzlzw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtltgrsjbv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtzztszmus.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtmtrdnbma.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtkgftxaxd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtqlcbmjze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtibafkzgi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hywenlv.cn/gtqdiapsaz.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gtyfkeajyi.html

Py:   len(arr)
来源：http://hz.guannengcc.top/gtbiexhjkb.html

PHP:  count($arr);
来源：http://hz.quarkkingdee.top/gtblqvarrx.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtoywkfhfa.html

TS:   arr.length
来源：http://hz.cdnleiting.top/gtvdjhlivl.html

Java: list.size();
来源：http://hz.yuxming.cn/gtqlxapzha.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtleywaail.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtegmsemdm.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gttubkaqts.html

[D07] 切片 / 取子数组
来源：http://hz.zhoulong.xyz/gtjgjhdzfa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtxfxwoulj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yongpay.top/gtgygebwrq.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gthylkovqa.html

TS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gttoulyzov.html

Java: list.subList(1, 4);
来源：http://hz.jinyuanbaomall.cn/gttxpbwiou.html

Go:   arr[1:4]
来源：http://hz.vqdsnc.cn/gtzwoiphhq.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gthpibrphw.html

C#:   list.GetRange(1, 3);
来源：http://hz.smart0.xyz/gtndqjjcsp.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtxeashxtu.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtcleqlhry.html

PHP:  array_merge($a, $b);
来源：http://hz.sufxvd.cn/gturcjjcts.html


<!-- 参考信息 -->