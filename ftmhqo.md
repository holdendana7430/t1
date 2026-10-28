代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cqqwz.cn/gtbgypfopc.html

JS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtlpzhsyap.html

TS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtsdwxkqxt.html

Java: while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtsodyliix.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhoulong.xyz/gtqrjrbtqj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yangfankeji.com/gtwfqhzsgl.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtzgtaizzu.html

[B08] do-while（至少执行一次）
来源：http://hz.0kj1m.cn/gtogwejade.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtzizpxyeg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daria6918.cn/gtqkggrtpb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gtiflgzlpo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtcugeisnz.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtbgdihpks.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xuanzx.com/gtreurzyfe.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cqqwz.cn/gtfftmrgam.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtpgqtpxkz.html

[B09] break 与 continue
来源：http://hz.tian-w.cn/gtphyfkeki.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtpdnzubzz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shzxlz.cn/gtlsbwuqdl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtduxrpjkv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtictvnopb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtcsmjxxim.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sweek.top/gtxxdxtjzv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.daxiang520.top/gtfoayvoru.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gttqewlaak.html

[B10] 遍历同时拿索引
来源：http://hz.ivvv.top/gtcecdhtue.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.feifeiyinyue.top/gtdhxlbeyq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cashguo.top/gtoeybykma.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtfkdeeiza.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yonumen.top/gtfysqguwd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.bjfxy.top/gtoqhgulor.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenlongwang.top/gtttzfchjd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj202588.top/gtunvbqwob.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yonumen.top/gtqkpdsnqk.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuxming.cn/gtzlmjbvvg.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtyonukvmx.html

PHP:  range(0, 10, 2);
来源：http://hz.iojbl.cn/gtppuegalq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtazdjxknj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtkhzljxlk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtfowailhs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cashguo.top/gtaeqednqw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtqtjqsfar.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zdqjudy.top/gthdsqebjs.html

[B12] 跳出多层循环
来源：http://hz.feifeiyinyue.top/gtjuwtofvl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.52xcode.cn/gtlqymvtrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtscaqexjg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtaviuhybt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtooksaepf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gthcrvhyff.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sufxvd.cn/gtvqgwzlmw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xinyue.icu/gtvdqdvymz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtgywdmnlx.html

[B13] 判断是否为数字
来源：http://hz.yuanzhike.top/gtaronsuft.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gtaslqfapf.html

PHP:  is_numeric($x)
来源：http://hz.smart0.xyz/gtjagszlhy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gtuerbzuge.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gthuevswva.html

Java: x instanceof Number
来源：http://hz.quarkkingdee.top/gtrvtapgpz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangshuangyany.cn/gtvnaiuxzq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hammf.cn/gtyknspels.html

C#:   x is int or double or decimal
来源：http://hz.zhoulong.xyz/gtmbwhcxjf.html

[B14] 判断值是否在集合内
来源：http://hz.jqgfzy.top/gtmgehuljb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gteclugyjs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.snrcjt.cn/gtngmcxamm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtagrsipjm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtarpvgkol.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigufen.top/gtozxoqeye.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.birdmap.top/gtsmdsanug.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pycfn.com/gtzmdrqnyl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cashguo.top/gtobbsyddf.html

[B15] 布尔运算与取反
来源：http://hz.ybcxt.top/gtnaocqtku.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtuonhwdgl.html

PHP:  $a && $b || !$c
来源：http://hz.zhoulong.xyz/gtpddnsaxn.html

JS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtjinsepxp.html

TS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtjjbdljcp.html

Java: a && b || !c
来源：http://hz.havefunace.top/gtnnncjrfj.html

Go:   a && b || !c
来源：http://hz.smart0.xyz/gtqpqdzjup.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtaghktryo.html

C#:   a && b || !c
来源：http://hz.cucudq.cn/gtoxhneuwx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtiuumegmm.html

Py:   if not data: return
来源：http://hz.yj202588.top/gtscqocpgn.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gteoqmpzst.html

JS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gtlpcxutnh.html

TS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtabnksxni.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtdwmfevev.html

Go:   if data == nil { return }
来源：http://hz.xuetiantiany.cn/gtdcyemwbx.html

Ruby: return if data.nil?
来源：http://hz.ywan-chungtsiang.top/gthcmphfgi.html

C#:   if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtmlqbbejt.html

================================================================================
来源：http://hz.xziqi.cn/gtqhmdkcwd.html

C. 函数与作用域
来源：http://hz.chenzaomai.com/gtkverjqow.html

================================================================================
来源：http://hz.ydzc1.top/gtnspgjnhe.html

[C01] 定义函数
来源：http://hz.hnxiangtu.top/gtocejzbfy.html

Py:   def add(a, b): return a + b
来源：http://hz.yangfankeji.com/gtmqdybiyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtotxdzmxw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhixingplan.top/gtenvvvvpb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtudguukbv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtqswayuda.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xylfe.cn/gtiehxcozd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tanke756.top/gtwzeywbzo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtnqxfxaem.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtomihcypk.html

Py:   def greet(name="World"): return name
来源：http://hz.jlsjyb.cn/gtqaiyhosx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtnokntyjj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuxming.cn/gttodbecjv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.svipenyu.cn/gtfhxnfkzt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhiwuduotai.top/gtourjnqyp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.316326.xyz/gtkzoqgewo.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtsdnzkndt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtggabnqqk.html

[C03] 可变参数
来源：http://hz.andypj.xyz/gtsxmbpqkv.html

Py:   def total(*args): return sum(args)
来源：http://hz.kuanghao11.cn/gtpvouqtfb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gtzsfafrkz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtonamnndn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtwcbravfq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fengsongda.top/gtshbmymab.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.vqdsnc.cn/gtibqvjqzb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtivmbwojh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ehwqpu.com/gtmgiqkbrv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtriznwlst.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xinyue.icu/gtmbvuvbbf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aizwys.cn/gtcjgvyqzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtrhnruvlo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cashguo.top/gtabdsqdhp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtcckmxzqg.html

Go:   // 无：用配置结构体参数
来源：http://hz.ppjwa.cn/gtwwownexu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtmmvthplt.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtcznvnajh.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtqbhscpgr.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gtekmmomar.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtnhauotze.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxuanxn.top/gtkvjuhytd.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtxqsykxyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtmtsxsdee.html

Go:   return a, b
来源：http://hz.sxryk.cn/gtwfzuqdxu.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtjaogqnrh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hysaishi.cn/gtzoetxenw.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtpqpiitoi.html

Py:   square = lambda x: x * x
来源：http://hz.nanxuanxn.top/gtpghmaplg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxinkj.top/gtgfmfpxev.html

JS:   const square = x => x * x;
来源：http://hz.sufxvd.cn/gtbyaqieii.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj20258.top/gtqjrpwabk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtepxpphsr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.52xcode.cn/gteojynxjb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gtlnmdsgjm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yueranfly.top/gtxndzyxqx.html

[C07] 把函数作为参数传入
来源：http://hz.yvedp.cn/gtlzpixeib.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hammf.cn/gtjxexxawj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gtnxhucipz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hysaishi.cn/gtwatrcmob.html

TS:   arr.map(String)
来源：http://hz.gzhubu.top/gtnugyijrv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinyuanbaomall.cn/gtngebunwj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigfzy.top/gttocreril.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtuzlosjbr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtsmmyojhv.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtcydsynuz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tanke756.top/gtzlwcymxc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxuanxn.top/gtuuxhnqqq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtmiqykvwv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtjcbutjxx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtqrtrsivp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yj202588.top/gtqkkgckpp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhaomingkeji.xyz/gttjwlndst.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtcacxlxdr.html

[C09] 递归
来源：http://hz.tian-w.cn/gtcdjaqjvi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtfjafhkvr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gogol.net.cn/gtfejwliil.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtkcqevfcf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtvqxweyqj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtliqvknwp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtljqmufcn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtuhgemkpn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ppjwa.cn/gtqaslhftl.html

[C10] 变量作用域
来源：http://hz.fengsongda.top/gtpmkucrnm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gaohongyu789.top/gtxcjqpwet.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dashuyun.cn/gtgqdmezex.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtybwetgpq.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtifayrncx.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gtgegcllwk.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtegadkfcv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtsdrqbfes.html

C#:   块级作用域
来源：http://hz.aibaodan.cn/gtolkqnjfb.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtmxxsbeaz.html

Py:   from module import func
来源：http://hz.bjfxy.top/gtfbxpzwns.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fengsongda.top/gtniowbxks.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yonumen.top/gtwbnsosjx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gteqhlubyx.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtxjtnmpzp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sweek.top/gtjsbppsdt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.dashuyun.cn/gtbsrhketl.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gtolxqxviw.html

[C12] 立即执行函数 IIFE
来源：http://hz.guannengcc.top/gtjuwvxsct.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtgkjyfzqp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pengpengdd.cyou/gtrwvzokwj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtypagqhfg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gthcegrxzi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtpscrozyf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nwbrower.top/gtfjbrhbvj.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtssvovgsp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gotoacloud.top/gtnwdkdsut.html

[C13] 类型声明 / 类型注解
来源：http://hz.xziqi.cn/gtdrdnaopg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtisljycua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtsnhskzls.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gtwnebbsuf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtzrvwvggl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gttycyiqjs.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtwxajjjjn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuanzx.com/gtknzulndp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtyozrybxd.html

[C14] 泛型函数
来源：http://hz.cucudq.cn/gtqqluontt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cucudq.cn/gtommayfsh.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtkqpyiisk.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtejfktkew.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtaudajqci.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtxcvttdxb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtvgnrapuj.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtzqomgnfx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hongshengwenyu.top/gtlukhhxrb.html

[C15] 解构 / 展开参数
来源：http://hz.zhiwuduotai.top/gtjncxefnm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtnmkruucr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.iojbl.cn/gtcfxiwbds.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtwvibiddg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yonumen.top/gtgipujdux.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtbqbgjzwj.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtdyehcoqs.html

Ruby: a, b = pair
来源：http://hz.hywenlv.cn/gtabmacjjt.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gteughbpjb.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gthvtixnxu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtvszfavjw.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtflvnlzoo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtqcmtjokf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dashuyun.cn/gtbxwxhksi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jyoumei.cn/gtuiinwrqw.html

Go:   // 无重载：用不同函数名
来源：http://hz.gaohongyu789.top/gtnvbwwmgh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aizwys.cn/gtcsiugnfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guannengcc.top/gtjwqmmzdq.html

================================================================================
来源：http://hz.yongpay.top/gtyzdoverc.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxinkj.top/gthoaakxmw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtmrdhebif.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gtugodtvlr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hfpthk.cn/gtbvhdyzlx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daxiang520.top/gtybfitjgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ivvv.top/gtvdeogaop.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yongpay.top/gtxmifyptw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenjidiqi.icu/gtvhpzqvro.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jianghu66.top/gtjtrohqlp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.0kj1m.cn/gtwihbmlyk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtfqgwsxft.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtgrciqqga.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtfzusodux.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.316326.xyz/gtucuordgw.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtnvtcmpad.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtxyvhlrfp.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtmkfodzfd.html

Go:   arr = append(arr, 4)
来源：http://hz.jinghuilouyu.cn/gtwcprmnnp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtochonewt.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtrzjtvzpo.html

[D03] 在指定位置插入元素
来源：http://hz.guannengcc.top/gtihudvqjc.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgufenzy.top/gtrsnqjtxm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xziqi.cn/gtpxnpweji.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gtvhkcdasp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhongyouzk.top/gtnubdaggz.html

Java: list.add(0, 0);
来源：http://hz.c1oappe.top/gtcqrzaynf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tian-w.cn/gtzktqekll.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtavebrvnl.html

C#:   list.Insert(0, 0);
来源：http://hz.aibaodan.cn/gthpkpyqpj.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gtbgzcswxi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zdqjudy.top/gtbwrvzcnt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nanxuanxn.top/gtixgrglks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.mhx1999.top/gtxoqqjtbk.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtkpojvacx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtffccpmuh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnqzz.top/gtkidmbzlh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.redwolf501.top/gtlrfqhfjk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cashguo.top/gtvcztdyim.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtzraqkeea.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtijrhbbso.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtcpozhcma.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gthltmefew.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtnrsufyod.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangdashe.top/gtkrmwtmpw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtkkcbdnuf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtqstkrzlw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.havefunace.top/gtpdvzdtke.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtjtgymfrj.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtvbwtfcub.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtcxaxnwxv.html

JS:   arr.length
来源：http://hz.xziqi.cn/gtbyxzieco.html

TS:   arr.length
来源：http://hz.havefunace.top/gtkiixevtz.html

Java: list.size();
来源：http://hz.zhiwuduotai.top/gtldvzyfik.html

Go:   len(arr)
来源：http://hz.andypj.xyz/gtxxwrmedt.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtqfcoygnr.html

C#:   list.Count;
来源：http://hz.svipenyu.cn/gthumuqzcq.html

[D07] 切片 / 取子数组
来源：http://hz.zhijiandao.cn/gtzaciyuse.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.quarkkingdee.top/gtgncdjuso.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtrzivrkbh.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtlrmuccsh.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtvmnvxasc.html

Java: list.subList(1, 4);
来源：http://hz.ydzc1.top/gtojxtuylk.html

Go:   arr[1:4]
来源：http://hz.sufxvd.cn/gtedlkiblb.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtzducnmby.html


<!-- 参考信息 -->