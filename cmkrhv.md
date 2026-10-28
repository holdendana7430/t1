代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.nanxuanxn.top/gtdxucbwck.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gtpbpgezin.html

TS:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtljkzyils.html

Java: while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtnfzhfysk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tianlin.xyz/gtkluvomne.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhiwuduotai.top/gtkckjsnkc.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtijgaucqq.html

[B08] do-while（至少执行一次）
来源：http://hz.jiagoushi.top/gtwytvrgkb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhixingplan.top/gtilanquec.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ppjwa.cn/gtryoszfrm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtertpvuyf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtdmsoqqzl.html

Java: do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtdhufotbj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shanyushiyangtech.top/gtqpxjsund.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shuidangran.top/gtgjbtwjev.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtujwwoagf.html

[B09] break 与 continue
来源：http://hz.jinghuilouyu.cn/gtxpjsbuxj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tanke756.top/gthwmkcyib.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gtcoukqqrn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtighqploj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtgkrhcydr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtjzvzmzid.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxinkj.top/gtjbrwzqoi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.smart0.xyz/gtvexxeiiu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtiperqnxt.html

[B10] 遍历同时拿索引
来源：http://hz.zdqjudy.top/gtocxonkre.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xinyue.icu/gtbwitbtmx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tianlin.xyz/gtudakailk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtkhsbopnj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtkztnbyes.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtplquicxd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xylfe.cn/gtrgmpoykl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yangfankeji.com/gtqaeygwls.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daria6918.cn/gtjmchwsum.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gtopxlslnm.html

Py:   list(range(0, 10, 2))
来源：http://hz.yuanzhike.top/gtlwlvqvhm.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtgpiuqtcc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtwsbgivwn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gotoacloud.top/gtmhvygkbf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jiagoushi.top/gthowbmoez.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cheryme.top/gtdnzcnxfc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtasfspskv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pengpengdd.cyou/gtydytxkbj.html

[B12] 跳出多层循环
来源：http://hz.cucudq.cn/gtiykhyxcw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangkeji.top/gtoqcrecjb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtejmwklmx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gttkrvnckj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtxxxrdfxf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtcdlmgaxh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gtpvphlyqx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtzupmwrdj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhixingplan.top/gtcizbfwly.html

[B13] 判断是否为数字
来源：http://hz.jinyuanbaomall.cn/gtwevucqyz.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtfbwisimu.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtpybzkdww.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtybjmewtd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtdajgtfmu.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtgcxplplt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gtgvzsyqqy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.haohaochexian.top/gtnbyeredk.html

C#:   x is int or double or decimal
来源：http://hz.chenlongwang.top/gtfovwzmbd.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtekgcgjbr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtqqayvtyh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gtqtcsxhab.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtmlptfizh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtwxkvyoqi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cheryme.top/gtkeouzgss.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ybcxt.top/gtdhwfiqcj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hammf.cn/gtwlyrpmld.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtyajpabwy.html

[B15] 布尔运算与取反
来源：http://hz.ydzc1.top/gtiidxtehk.html

Py:   a and b or not c
来源：http://hz.52xcode.cn/gtxvznlxdo.html

PHP:  $a && $b || !$c
来源：http://hz.zhiwuduotai.top/gtnsuxfnfl.html

JS:   a && b || !c
来源：http://hz.0kj1m.cn/gtjvebgwgb.html

TS:   a && b || !c
来源：http://hz.smart0.xyz/gtdpnqztqo.html

Java: a && b || !c
来源：http://hz.pycfn.com/gtdphjnipn.html

Go:   a && b || !c
来源：http://hz.nanxuanxn.top/gtwbrlumjy.html

Ruby: a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtuqiqfrpr.html

C#:   a && b || !c
来源：http://hz.yj20258888.top/gtugmysnlk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtyytorxvg.html

Py:   if not data: return
来源：http://hz.yanxiufei.cn/gtpxabizgo.html

PHP:  if (!$data) { return; }
来源：http://hz.sweek.top/gtqsusmedn.html

JS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtjinxgbar.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtohfsqfrp.html

Java: if (data == null) return;
来源：http://hz.snrcjt.cn/gtplnnoync.html

Go:   if data == nil { return }
来源：http://hz.jinqigfzy.top/gtrgqtqzlm.html

Ruby: return if data.nil?
来源：http://hz.nanxinkj.top/gtgaciwyte.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtjttdfzes.html

================================================================================
来源：http://hz.sweek.top/gtibmpotyw.html

C. 函数与作用域
来源：http://hz.smart0.xyz/gtnipjgilt.html

================================================================================
来源：http://hz.quarkkingdee.top/gtodickyao.html

[C01] 定义函数
来源：http://hz.shuidangran.top/gtfpajdfzk.html

Py:   def add(a, b): return a + b
来源：http://hz.cucudq.cn/gtylnqskjt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtwsalnvyr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtsdhkkehe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtpdecrefw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtfqnordvx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daxiang520.top/gtvwecowsl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jyoumei.cn/gtznhwwlei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtrfdnuuqj.html

[C02] 默认参数
来源：http://hz.tian-w.cn/gtmbofofbw.html

Py:   def greet(name="World"): return name
来源：http://hz.pycfn.com/gtamyzmjjy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangshuangyany.cn/gtchzwqpuf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhijiandao.cn/gtktsfdwke.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.mhx1999.top/gtciupudms.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yueranfly.top/gtmtzwqidl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hnxiangtu.top/gtghgnwdeq.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtmtmdkxcm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhongyouzk.top/gtiivtnunl.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtbkqpkyrb.html

Py:   def total(*args): return sum(args)
来源：http://hz.yanxiufei.cn/gtggusayfo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtrtwboaka.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtzjswvikz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gtfxkghjbm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghu66.top/gtwyjiqeoy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtfpcftfyt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtxpqhubms.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtbljfahbq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhiwuduotai.top/gtvesnspok.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtlulbtpxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jlsjyb.cn/gtqqkbobwn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtbenuzpoj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gthqcmqcrw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtqeikhwax.html

Go:   // 无：用配置结构体参数
来源：http://hz.tianlin.xyz/gtgatqezqp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtalwewkxy.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtdegkacgw.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtietqfous.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtcubnhyvh.html

PHP:  return [$a, $b];
来源：http://hz.shuidangran.top/gtwlfdtghn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigfzy.top/gtruciyxgl.html

TS:   return { a, b };
来源：http://hz.yj20258888.top/gtadtjptvf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtzxpztonq.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gtmwvcoqgs.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtxrjevanz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtdcwmriwi.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtzlxvnrzr.html

Py:   square = lambda x: x * x
来源：http://hz.dashuyun.cn/gtcugotlmi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.havefunace.top/gtqvjnclcm.html

JS:   const square = x => x * x;
来源：http://hz.9152youxi.cn/gtzludqdky.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuxming.cn/gtlnmjnean.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenlongwang.top/gtgfxzoykt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigfzy.top/gtxgzmisxa.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtnrxbtawj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtxrrqciku.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtfiwcqkja.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fzhhl.top/gtmbintvzg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.mhx1999.top/gtddywehag.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sufxvd.cn/gtpbsobdxe.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtaybsbjry.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtmctsoezw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yongpay.top/gtxlugawbg.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtqkoichdv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtkdluuzxa.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtioqzuwyk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tanke756.top/gtfvuevbns.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtjrcowyxe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gteiyxoubz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtzsxaqegq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gtachhnxii.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yanxiufei.cn/gttvsohpxh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtffdckgbl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtszikifpw.html

[C09] 递归
来源：http://hz.birdmap.top/gtvjkbzoro.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtaplzzvdu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtcxvuzxmt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtfddmbtvs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtfvtljatq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtyfhmyqqu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj202588.top/gtmqkepzqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtasoaiqbd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dianchejie.cn/gthryfwdrb.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtlhzzeucl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtckjfhzho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtlhlwutww.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ppjwa.cn/gtnyzmhhlr.html

TS:   同 JS
来源：http://hz.yj20258.top/gtwdkyydep.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gttnnqhnhj.html

Go:   花括号块级作用域
来源：http://hz.xuanzx.com/gtauhszpnr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.mhx1999.top/gtldcncfse.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtwijmmxnc.html

[C11] 模块导入与导出
来源：http://hz.zhijiandao.cn/gtqmgiejvk.html

Py:   from module import func
来源：http://hz.pycfn.com/gtkbbalevp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.redwolf501.top/gtcxqdmdug.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gthxhtxcth.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigufen.top/gtsoredoua.html

Java: import java.util.List;
来源：http://hz.nanxinkj.top/gtlntpujmc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gttggnainb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtuipfvgfe.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gtipunvqap.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gtentrtrdy.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgfzy.top/gtbxaycskn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtmklhmreh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtbelbkvvc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtydawmcem.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenzaomai.com/gtjdwrpogd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.kuanghao11.cn/gtabomgvec.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtqepwgosm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.0kj1m.cn/gtyldfdjty.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gtdfrftksb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtbxqontmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtqpfnwgca.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtjqjsrkfj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gticvwvhzl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtnplcfqqw.html

Go:   func add(a, b int) int
来源：http://hz.zhiwuduotai.top/gttwleahsy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtfplfuzfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zycfv.cn/gtnuuqupkh.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtfzjtcost.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtvzcdylcn.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtdprhpjyo.html

JS:   // 无泛型
来源：http://hz.shangyingyoupin.top/gtbrbxtykb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.0kj1m.cn/gtlpuosrxn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtdlopjeog.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtobkvglyg.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtagnepzvr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtjlqaemur.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtfczsvdde.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jianghu66.top/gthfpojmxt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtggildiil.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtcabwilqf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtmdorhuym.html

Java: // 无解构
来源：http://hz.tianlin.xyz/gthkbesxvd.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtkepdimgf.html

Ruby: a, b = pair
来源：http://hz.hammf.cn/gtzhikbhge.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtzbwtzfke.html

[C16] 函数 / 方法重载
来源：http://hz.cqqwz.cn/gtbzoqdrxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.vqdsnc.cn/gttqswogav.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtxymkwqqv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtdqumbvqx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtrfdfeogk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtkllapicq.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtjkyrqbeg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinghuilouyu.cn/gtwbeovpfe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.haohaochexian.top/gtlcizcpgd.html

================================================================================
来源：http://hz.zhengqikj.top/gtlkmchiyr.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangkeji.top/gtaeowtvjt.html

================================================================================
来源：http://hz.chenzaomai.com/gtwytqvors.html

[D01] 创建数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtfzcqcypg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtotlvucds.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.svipenyu.cn/gtklhtypvb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuxming.cn/gtnrylyuow.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtwtzgzlut.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinghuilouyu.cn/gtirwwevfq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gtuvmokqvu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtwajtmroi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtkoubcwzi.html

[D02] 追加元素到末尾
来源：http://hz.zycfv.cn/gtjjrzjrlo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtskinxugh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hfpthk.cn/gtboaemjhj.html

JS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtoppinmre.html

TS:   arr.push(4);
来源：http://hz.tanke756.top/gtsecccvwa.html

Java: list.add(4);
来源：http://hz.tianlin.xyz/gtebiayzfp.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtxchrnquw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gtzumxjnvr.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtyftniyrd.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtqzjtugfe.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigufen.top/gtrftsgrij.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtiarlghqs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtbvqubkun.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.haohaochexian.top/gtgjzoptpw.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtdwfaxsqd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jiagoushi.top/gtyydergmf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gthenbzdux.html

C#:   list.Insert(0, 0);
来源：http://hz.yonumen.top/gtipjuvwnu.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gtrwsnxmtt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtsjemwpma.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtbglaupli.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtwifmnukf.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtgqfageyq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.bjfxy.top/gtecucivwr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daria6918.cn/gtrxrwxgsv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtobdkquil.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinyuanbaomall.cn/gtggywfymt.html

[D05] 访问与修改元素
来源：http://hz.jqgufenzy.top/gtyojlyncc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtnwecpgwb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xziqi.cn/gtlafyefef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gthlibbcfb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtopurzghr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gtbuwsqzkb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtpsrqiacv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtvpnbgtmi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydzc1.top/gtvlrotyxn.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gthutszlxo.html

Py:   len(arr)
来源：http://hz.chenzaomai.com/gtnydzskqj.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtoszfsrwi.html

JS:   arr.length
来源：http://hz.ppjwa.cn/gtymvarcvd.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtivwgwpbs.html

Java: list.size();
来源：http://hz.haohaochexian.top/gtopmvsvpk.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtwgyhaknj.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtkysijxdm.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtnhnnoeno.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gthaiovqbk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtqrkmdtlo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gtkwoogoam.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtiiqjjcsd.html

TS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtmxszbtyn.html

Java: list.subList(1, 4);
来源：http://hz.zhijiandao.cn/gtsbmurfgr.html

Go:   arr[1:4]
来源：http://hz.jinyuanbaomall.cn/gtvhuhohyd.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gtrlfhhkuo.html


<!-- 参考信息 -->