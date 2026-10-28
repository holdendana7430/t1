代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gttuaxmbub.html

JS:   while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtwysqgpaf.html

TS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtaefqaswi.html

Java: while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtpdcjbhjj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ydjk.org.cn/gtcjcndhzb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydjk.org.cn/gtqtyvqnqy.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtufyjtevi.html

[B08] do-while（至少执行一次）
来源：http://hz.yuanzhike.top/gtgctnjmyk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhixingplan.top/gtbdphhejk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtuzdqqqvg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtwtfcfaam.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtmuuuxyjl.html

Java: do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtqmzbeoil.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gtiiybrwpq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigfzy.top/gtrrdktnwd.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gttrgxanmx.html

[B09] break 与 continue
来源：http://hz.fzhhl.top/gtoyovyuok.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yongpay.top/gtpipecmxl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gttptanhkw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtadimggfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtzbybtcxv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtxhwciott.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxuanxn.top/gtskffvmnz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtmzexoykz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtxissnjui.html

[B10] 遍历同时拿索引
来源：http://hz.yangfankeji.com/gtjkkiucyz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tanke756.top/gtrtdhhvvz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhijiandao.cn/gtcdlvbaxm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtlfoleqwz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangkeji.top/gtojcmoyiz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zdqjudy.top/gtsfcccoxa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnxiangtu.top/gtpccqmvay.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guannengcc.top/gthngytbeo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258888.top/gtdsyfkrpz.html

[B11] 生成数字序列 / 区间
来源：http://hz.yongpay.top/gtecwiijhq.html

Py:   list(range(0, 10, 2))
来源：http://hz.cheryme.top/gtexovasdj.html

PHP:  range(0, 10, 2);
来源：http://hz.hnqzz.top/gtkrevwtln.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtmqpigdgq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtnigudbui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.svipenyu.cn/gtypcndubp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cdnleiting.top/gtvfibkgzh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtrltqsapy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dianchejie.cn/gtxacghmho.html

[B12] 跳出多层循环
来源：http://hz.jyoumei.cn/gtuqwtttvy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuanzhike.top/gtmoaawaqg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtqpqpglkj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtexusrcjq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtgkkhnhuw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtoccayknq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuanzx.com/gtivzpbgxe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hywenlv.cn/gtzlkdwckx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cashguo.top/gtgygennvm.html

[B13] 判断是否为数字
来源：http://hz.hongshengwenyu.top/gtdcjzbwth.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gtbetkdxiu.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtkjqojjww.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtwaqagqad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtptsfdodv.html

Java: x instanceof Number
来源：http://hz.cheryme.top/gtaavpmmxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhijiandao.cn/gtynyjxqaq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dianchejie.cn/gtysmpkchb.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtxvzmkjjn.html

[B14] 判断值是否在集合内
来源：http://hz.yueranfly.top/gtbssuebhu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtyrzzieat.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangtech.top/gttvcbjnac.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tian-w.cn/gtapcfogwp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtbgaegzpz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhijiandao.cn/gtzqynqysk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gtjxumdstk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gtlbdaasbn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtawxzntmk.html

[B15] 布尔运算与取反
来源：http://hz.chenlongwang.top/gtvqdjwqqq.html

Py:   a and b or not c
来源：http://hz.zhaomingkeji.xyz/gtagnjqrqf.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gteiyxwytk.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtqkrrbbxc.html

TS:   a && b || !c
来源：http://hz.fzhhl.top/gtbrcmdsxd.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gtvgmohimx.html

Go:   a && b || !c
来源：http://hz.dashuyun.cn/gtpkojktcm.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtvytpvwiw.html

C#:   a && b || !c
来源：http://hz.zhoulong.xyz/gtclkgaffd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yanxiufei.cn/gtrkmmcmqe.html

Py:   if not data: return
来源：http://hz.cdnleiting.top/gtkbvbiwug.html

PHP:  if (!$data) { return; }
来源：http://hz.hammf.cn/gtspwzgsyx.html

JS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtzvyxkgyo.html

TS:   if (!data) return;
来源：http://hz.jianghu66.top/gtdzjqacos.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtjcyvdgie.html

Go:   if data == nil { return }
来源：http://hz.xuanzx.com/gtbqdadlxx.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtnwtynkhg.html

C#:   if (data == null) return;
来源：http://hz.316326.xyz/gtyqgamkaq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbojxycuy.html

C. 函数与作用域
来源：http://hz.xylfe.cn/gtlgrspqzp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtocewgqhq.html

[C01] 定义函数
来源：http://hz.hysaishi.cn/gtlumpgasa.html

Py:   def add(a, b): return a + b
来源：http://hz.xingfuxueyuan.xyz/gtlpyhnekg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtdwalimff.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtcstljivv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtehwzyajr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtvqomcfbz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtgdkvgthq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gttfitxqlj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtqhodygan.html

[C02] 默认参数
来源：http://hz.0kj1m.cn/gtsviivknj.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtilfdtocp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtrlteksus.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gtzcagkjht.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuanzx.com/gtggjzjlwm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tian-w.cn/gtajugcluz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtbazdqjol.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtmolerbmp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.birdmap.top/gtapqyaaip.html

[C03] 可变参数
来源：http://hz.zycfv.cn/gtuqkkleui.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtyjcvznvp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daria6918.cn/gtsbizzymw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtbeyqvhjh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtfnqzluob.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.birdmap.top/gtbvrtorpo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtcewlvhjm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtbfihgfne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenzaomai.com/gthgdqqbiw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.smart0.xyz/gtqcrbroju.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtkdfksdtw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtgoxjqrag.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtsbnsddfr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cucudq.cn/gttkekbpqr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.haohaochexian.top/gtkprjbfxy.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gtlewuqdtc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtwywijkfm.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtpytbiadx.html

[C05] 返回多个值
来源：http://hz.zhijiandao.cn/gtulipvheo.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gtrxkitzjb.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtczvgttww.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtnqcpopht.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtlhaunxgj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zycfv.cn/gtyynfvyiz.html

Go:   return a, b
来源：http://hz.jyoumei.cn/gtwlcbzoqf.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtzglzjyah.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xingfuxueyuan.xyz/gtkunhaaau.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gtvfnhhpnn.html

Py:   square = lambda x: x * x
来源：http://hz.yvedp.cn/gtzomiplti.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtzgdlprag.html

JS:   const square = x => x * x;
来源：http://hz.ppjwa.cn/gttfdtlztm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pycfn.com/gtsfdhpjik.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gtfulhefic.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtdkdduvxx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fzhhl.top/gtwhhtugiq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtswqzvpgy.html

[C07] 把函数作为参数传入
来源：http://hz.yvedp.cn/gteimsztie.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtvnwbxcrl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtqcbeuklf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtnaejbfhu.html

TS:   arr.map(String)
来源：http://hz.jinqigfzy.top/gtkglcuesw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenzaomai.com/gtgpuizsaw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtkybmsmbt.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhengqikj.top/gtehkowazn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cashguo.top/gtpliylswb.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtbsyrtnhc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.0kj1m.cn/gtovcbnanr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gthbnkjudj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtntcmqnwl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtajqrivhj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangshuangyany.cn/gtwpprsqvj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtqywnthwz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtncvgokkl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtdqrgicrr.html

[C09] 递归
来源：http://hz.ydzc1.top/gtseznsynk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtqtgwexkr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gthoqsbdhp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtwsgdysad.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtcjreagjv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtmhbvbfca.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigufen.top/gtpdveehri.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtkhdirnqq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.redwolf501.top/gtbhdahqro.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtqnuiebsq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xziqi.cn/gtabsusirh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xylfe.cn/gtjpospmvm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yueranfly.top/gtpcaouvou.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtkllzmzao.html

Java: 方法内为块级作用域
来源：http://hz.jianghu66.top/gtjuogyfxy.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtgjqkwwlr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ybcxt.top/gtkkkwyvjg.html

C#:   块级作用域
来源：http://hz.cashguo.top/gtfwtdomvf.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtxzpnhtrb.html

Py:   from module import func
来源：http://hz.zhengqikj.top/gtvwjelgjf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.52xcode.cn/gtiaizqrjy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtcljgisry.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.9152youxi.cn/gtaeoucvyj.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtqagcwtrw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtvgbbixpu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtwtjpsoxo.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtyxguxvlk.html

[C12] 立即执行函数 IIFE
来源：http://hz.guannengcc.top/gtlewdfmti.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtsooaexhu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gotoacloud.top/gtrppbwfga.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtzzzdqszd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtvitxofne.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtwqyzylno.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tian-w.cn/gtjnbwtuhw.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtzvftfvhj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.wangdashe.top/gtrbzlpxtn.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gtalzkizem.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtqjfoktpl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtngfpmobq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtpdyxrybe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtacjghpes.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtuqgbdbni.html

Go:   func add(a, b int) int
来源：http://hz.zhaomingkeji.xyz/gtmnwpfcwh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gtfwyobljv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtufmqtlac.html

[C14] 泛型函数
来源：http://hz.cucudq.cn/gtghcyyolc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtxoxpcugw.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtxpogryhj.html

JS:   // 无泛型
来源：http://hz.gaohongyu789.top/gtjtbveyrl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtotngfenr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yueranfly.top/gtucdzxnon.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhixingplan.top/gtqmvsihmi.html

Ruby: # 无泛型
来源：http://hz.9152youxi.cn/gtargphhaf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.havefunace.top/gtohylnpuf.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtwfdpimzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtnqwpsmme.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fzhhl.top/gtwdlvorrq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtierpwwgj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sxryk.cn/gtfrmwnhai.html

Java: // 无解构
来源：http://hz.daria6918.cn/gtnvfjhwvs.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtnzmuovvy.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtnjjfqump.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtqsiapsja.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtvkwtggxk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtrlkowesa.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtjgyjusfp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangtech.top/gtlxylotuu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtigvomjni.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.mhx1999.top/gtgmdxztgc.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtvxbzplso.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aizwys.cn/gtxcjjozha.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtfehemwgh.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzxuwhphq.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gthioqeqou.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthtakbxnx.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtsqiopoxy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtookthvqb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtoyoeizdn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gtpvrotjgi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtcqluimzd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhijiandao.cn/gtbkvlwekr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.mhx1999.top/gtyatpfpgz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sufxvd.cn/gtllrfpamr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.iojbl.cn/gtcmmskqaa.html

[D02] 追加元素到末尾
来源：http://hz.jinghuilouyu.cn/gtckndhoyt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gtxokskhlm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtporpjlnx.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtfkuysyom.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtevzdpwac.html

Java: list.add(4);
来源：http://hz.hnxiangtu.top/gtkkeagari.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtuoqdibni.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgfzy.top/gtrarwxdlm.html

C#:   list.Add(4);
来源：http://hz.yongpay.top/gtpgckktlf.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gtpultyspm.html

Py:   arr.insert(0, 0)
来源：http://hz.ybcxt.top/gtitboqgfy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtbmkvhdcm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gtpdofezcp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nanxuanxn.top/gtluzquouc.html

Java: list.add(0, 0);
来源：http://hz.ppjwa.cn/gtrnggwuqg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtmsunjbsw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtelgsudfw.html

C#:   list.Insert(0, 0);
来源：http://hz.mhx1999.top/gtsorffzjj.html

[D04] 删除元素
来源：http://hz.redwolf501.top/gtlmxuvmmr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtvojeptvw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtolmvhfff.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shangyingyoupin.top/gtuyeaytab.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtxtqmxfoa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtyvvdslrr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtwqsgwpwu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.birdmap.top/gtbyapuixl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhijiandao.cn/gtpajvexgp.html

[D05] 访问与修改元素
来源：http://hz.yj202588.top/gtirvmpupe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtsplqrjgj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gthlmzwafz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtfaamvffr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.316326.xyz/gtgnigmhza.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.vqdsnc.cn/gtjemvocpe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtshiyldnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtpbsqcvct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtnaohgprf.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtbyeonhbe.html

Py:   len(arr)
来源：http://hz.jinqigfzy.top/gtfepqaxdp.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtpdosnxzt.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtwwoewkat.html

TS:   arr.length
来源：http://hz.sweek.top/gtvsffdjyw.html

Java: list.size();
来源：http://hz.sweek.top/gtcvpjfkzb.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtkxadgcih.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gttjeloqwy.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtbzizqrga.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtnszrqouu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zdqjudy.top/gthmhzorbo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gthxaaenao.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtaiomcemt.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtjmhgjnfs.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gtbkhklluo.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtqrffbety.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtoudkqgog.html


<!-- 参考信息 -->