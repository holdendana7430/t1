代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.ehwqpu.com/gtlhkbhhse.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.kuanghao11.cn/gtqeoauufw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtxqzgwyja.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtmqonekwi.html

Java: do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtslpdpxzn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jlsjyb.cn/gtyfdacaex.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gotoacloud.top/gtrsivrenq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtvuglzwyz.html

[B09] break 与 continue
来源：http://hz.hnxiangtu.top/gtyouptimu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnxiangtu.top/gtwqvtmgup.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jiagoushi.top/gtaoamhdlf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gthonhobnl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtspgywukf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtfrjocxot.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtggkhijyo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hongshengwenyu.top/gtngjvjxkr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgufenzy.top/gtxeqjwojb.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gttmzwkfaw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yonumen.top/gtqgsiepae.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cheryme.top/gtekkntkfz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nanxinkj.top/gtiagbbfzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtmalpkgwv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtlysntsix.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yvedp.cn/gtzeonuqmd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.vqdsnc.cn/gtwdufcyhj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pengpengdd.cyou/gtpipaehlq.html

[B11] 生成数字序列 / 区间
来源：http://hz.shangyingyoupin.top/gtdqnaivci.html

Py:   list(range(0, 10, 2))
来源：http://hz.ydzc1.top/gtjqiqnpnn.html

PHP:  range(0, 10, 2);
来源：http://hz.mhx1999.top/gtngnwiasx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gtyzxykwmo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtnpjtmjls.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gtbvkxbfut.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtrripuvno.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuetiantiany.cn/gtahonvbdt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shzxlz.cn/gtmgaewatq.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtyccdbgrf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhoulong.xyz/gtsndlcrwh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.9152youxi.cn/gtyanqawuv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtihqpjoiu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtxybacqqb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtpqapiyqi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtwoegtzjp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dashuyun.cn/gtmzlwwjec.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yongpay.top/gtzakhwibc.html

[B13] 判断是否为数字
来源：http://hz.zycfv.cn/gtjffyqbmf.html

Py:   isinstance(x, (int, float))
来源：http://hz.hysaishi.cn/gtoampyopv.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtiidddunj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuxming.cn/gtdxvvabmg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gtxcfctgaz.html

Java: x instanceof Number
来源：http://hz.yj20258888.top/gtpxphhlul.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhongyouzk.top/gtlapvojkt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtyqxdlpzs.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtloefvxvi.html

[B14] 判断值是否在集合内
来源：http://hz.0kj1m.cn/gtetizugew.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xingfuxueyuan.xyz/gtndnonuos.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xingfuxueyuan.xyz/gtporelzof.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtvzddghdn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtaojdrrnu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgfzy.top/gterdxapjm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhiwuduotai.top/gtbhqsnbii.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nanxuanxn.top/gtmksmpoon.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.daxiang520.top/gtrccbdyau.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gtifmquzem.html

Py:   a and b or not c
来源：http://hz.svipenyu.cn/gtmduylsqm.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtkhmlyrxp.html

JS:   a && b || !c
来源：http://hz.316326.xyz/gtnlzajzlg.html

TS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtqfhjqzji.html

Java: a && b || !c
来源：http://hz.jqgfzy.top/gtahgzlkyl.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gteisbdxjz.html

Ruby: a && b || !c
来源：http://hz.sufxvd.cn/gtydhfqxzq.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gthntqvzkb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtaqkjltdo.html

Py:   if not data: return
来源：http://hz.nanxuanxn.top/gtsqlxjxpd.html

PHP:  if (!$data) { return; }
来源：http://hz.kuanghao11.cn/gtzxmshraw.html

JS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtwppvcppe.html

TS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtqzbpeqii.html

Java: if (data == null) return;
来源：http://hz.nanxinkj.top/gttshrunsw.html

Go:   if data == nil { return }
来源：http://hz.kuanghao11.cn/gtwrcbxnpq.html

Ruby: return if data.nil?
来源：http://hz.birdmap.top/gtgzxuetke.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gtcemwngtu.html

================================================================================
来源：http://hz.snrcjt.cn/gtlanajoef.html

C. 函数与作用域
来源：http://hz.chenlongwang.top/gttvuuvqky.html

================================================================================
来源：http://hz.smart0.xyz/gtobvxlcon.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gtkaranwzt.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtjzvbutul.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtghkuzaxd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtdgwefsdd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtmlugzwzc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtocnzhxps.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cucudq.cn/gtgwfnclwi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtfzhjiqln.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtxuwlcmby.html

[C02] 默认参数
来源：http://hz.yj202588.top/gtetxqqfiu.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtoiwssenx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnxiangtu.top/gtsvywprmr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtvqitkuts.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtyhjfkymp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtalbxufhh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tian-w.cn/gtbprwylmi.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtluxlglbt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gaohongyu789.top/gtcikvanqt.html

[C03] 可变参数
来源：http://hz.yuanzhike.top/gtnazgthtv.html

Py:   def total(*args): return sum(args)
来源：http://hz.yongpay.top/gtetrqcfwi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258888.top/gtovifariu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtsyqfwmiu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gthsyqmhgk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangshuangyany.cn/gtnyhcdqoo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.bjfxy.top/gtbsbuudfq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shzxlz.cn/gtjywpawci.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gtugghkjxc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hywenlv.cn/gteblolpyy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtbxdatexl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cucudq.cn/gtmntdezpu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtncckofkz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shzxlz.cn/gtecprpzmc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtcobdnpbt.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtsmjpopqn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtdxtrqxlv.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtpjrwyhzm.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtztjhnbhd.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gtsiuvargz.html

PHP:  return [$a, $b];
来源：http://hz.9152youxi.cn/gtsdtknvbz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnqzz.top/gtkdheqsiy.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtqhevvvrz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtyxcbktsy.html

Go:   return a, b
来源：http://hz.ybcxt.top/gtrhtnudqg.html

Ruby: return a, b
来源：http://hz.shanyushiyangkeji.top/gtrndemnqu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtdzmlzjql.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtxhcdzuue.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtsjndwavc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtcaebxjlm.html

JS:   const square = x => x * x;
来源：http://hz.zhengqikj.top/gtzisvwvcj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shzxlz.cn/gthjcanmuh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.feifeiyinyue.top/gtoxexvqsd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hfpthk.cn/gtpsmdaxrk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aibaodan.cn/gtyqeetjes.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.birdmap.top/gtuitkayby.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtzinigrza.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gotoacloud.top/gtmnqivjue.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gtoqqmkkjw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtelinhqzd.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gtifsevxua.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shuidangran.top/gtwuybejnq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtcacdklnk.html

Ruby: arr.map(&:upcase)
来源：http://hz.ehwqpu.com/gtbrshezzk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtclgcilzt.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gttiktppfr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtwgbejeum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtmgnqwooh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtjnrfddom.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtkvtosbyx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xziqi.cn/gtcrfsxucw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtwqsvyajq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sweek.top/gtoojzmwnd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtsrxcwvog.html

[C09] 递归
来源：http://hz.ppjwa.cn/gthzicjzts.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shuidangran.top/gtubmqxzkm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hysaishi.cn/gttonglwbc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtjvnoaevq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtdifzablx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtphworxum.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtijsrnzfo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.andypj.xyz/gtvkhznhfe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtbpjepxpb.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtorwhckle.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hfpthk.cn/gtrefllhaj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtieqkyijf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.smart0.xyz/gtaewyfave.html

TS:   同 JS
来源：http://hz.gogol.net.cn/gtkjfmdsry.html

Java: 方法内为块级作用域
来源：http://hz.zhiwuduotai.top/gthzqycryh.html

Go:   花括号块级作用域
来源：http://hz.nanxinkj.top/gtjyfzrgys.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gtyxlckavs.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtlcnafvne.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtbvpzxhti.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtfozcttnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tanke756.top/gtkzkfbbvu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenzaomai.com/gtswnjshga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tianlin.xyz/gtpwfyiaob.html

Java: import java.util.List;
来源：http://hz.yj202588.top/gtquomfpiv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yanxiufei.cn/gtnqxdrpjx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangkeji.top/gtebdhzsje.html

C#:   using System.Text;
来源：http://hz.zhixingplan.top/gtsxmoorph.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtmzecfehg.html

Py:   (lambda: print("run"))()
来源：http://hz.hywenlv.cn/gtbapxgezw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtglasvyzf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtnnaxibcs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtluvocnbu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.chenlongwang.top/gtzgddbppx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gtrydczqii.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gtubqjhqpk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtzpuhanpe.html

[C13] 类型声明 / 类型注解
来源：http://hz.ehwqpu.com/gtnjlqzrkq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hammf.cn/gtvqjcioiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtwteuepkw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hywenlv.cn/gtieohkprm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gthycrnfoi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtpmmikloq.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gtwstkfvut.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gtlhhozles.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhaomingkeji.xyz/gtydzgfsfz.html

[C14] 泛型函数
来源：http://hz.jqgufenzy.top/gtdotgfkcn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guowangkeji.top/gtgyzrxdve.html

PHP:  // 无泛型
来源：http://hz.vqdsnc.cn/gtjjqzkmqg.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtmsxwjkuz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtbyvvdgah.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtzzqizxbu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxinkj.top/gtiyquoqtk.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtfflvbqau.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtmvstvidw.html

[C15] 解构 / 展开参数
来源：http://hz.chenzaomai.com/gthubwfuyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtjsyyissn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gtngqkfzuh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtgewyaljs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhixingplan.top/gtifioggmh.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtqgoyfarl.html

Go:   // 无解构
来源：http://hz.316326.xyz/gtvzxbkxwi.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtltjunjss.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtvepgjciz.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtmpqushvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtsuxlfcrr.html

PHP:  // 无重载
来源：http://hz.xuetiantiany.cn/gttzrqfbpp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.havefunace.top/gtacoapaqb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtjgnbskid.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gtxxynrnqr.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtripnrpel.html

Ruby: # 无重载：靠动态参数
来源：http://hz.feifeiyinyue.top/gtniklnmmd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtzitbjqmw.html

================================================================================
来源：http://hz.jqgfzy.top/gtpjkkdpnv.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigufen.top/gtsocyttoe.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfptshofa.html

[D01] 创建数组 / 列表
来源：http://hz.sufxvd.cn/gtasyvtuwx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtkqjpqwvg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtrnjifmoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtyslprwci.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shangyingyoupin.top/gtssbebmbx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtmsonyusd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtxzlxqxgd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jyoumei.cn/gtfxqmbawl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.svipenyu.cn/gtfwhrxumd.html

[D02] 追加元素到末尾
来源：http://hz.daxiang520.top/gtrggnfmqw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtbqmslrnj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtdwgiztpx.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtivylvixz.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gttwcyvcwa.html

Java: list.add(4);
来源：http://hz.vqdsnc.cn/gtngflejrb.html

Go:   arr = append(arr, 4)
来源：http://hz.zhijiandao.cn/gtfbwpfpsx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtlmtyyrgu.html

C#:   list.Add(4);
来源：http://hz.cucudq.cn/gtaicvlkhe.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtoatprpkk.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtwsicflmh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258.top/gtpistqtfv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtqcxxxyre.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtqxuvrqgs.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtwgvfctzp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gttkzilmci.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtgzthqaus.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtqmqgxrhq.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtmsdwizjf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tianlin.xyz/gtftzeghij.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtphfcrqwk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtunlcoyhv.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtiamyjzvm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtignltetd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtosqxllsd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.quarkkingdee.top/gtvbvcsegf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtqqvutill.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtfpizywcs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtsujhxpzt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jianghu66.top/gtxoekoymi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yanxiufei.cn/gttbnhmpza.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtvsphbnso.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.redwolf501.top/gtnzcvqbwu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shzxlz.cn/gttpeziybb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtfzxfkdsf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgfzy.top/gtybpljpau.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtleoegjch.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtninvtvon.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtqhwtdsst.html

JS:   arr.length
来源：http://hz.nanxinkj.top/gtrlolwdou.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtqmfanpgs.html

Java: list.size();
来源：http://hz.andypj.xyz/gthakyhetr.html

Go:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtotfqmqmk.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtxpsfteuf.html

C#:   list.Count;
来源：http://hz.mhx1999.top/gtxebddwtt.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258888.top/gtwfascfbu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gteenduwjg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtmgtasayg.html

JS:   arr.slice(1, 4);
来源：http://hz.tanke756.top/gtqfitjfff.html

TS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtcmqfwgmp.html

Java: list.subList(1, 4);
来源：http://hz.jinghuilouyu.cn/gtlloremjr.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtutrrfzql.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gtaxuastft.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtyhskroml.html

[D08] 合并两个数组
来源：http://hz.jinqigfzy.top/gtlyhfjwdt.html

Py:   a + b;  a.extend(b)
来源：http://hz.sysykeji.top/gtfeyjrirz.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtmlrfxbcr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fzhhl.top/gtjplxfrgm.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtdwigxmun.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guannengcc.top/gtdqbuztve.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtqomqzecd.html


<!-- 参考信息 -->