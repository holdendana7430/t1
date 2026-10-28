代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuetiantiany.cn/gtohynnmvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtfylbetho.html

[B07] while 循环
来源：http://hz.daria6918.cn/gtlmszniup.html

Py:   while i < 10: i += 1
来源：http://hz.jianghu66.top/gtrmijlyzo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ivvv.top/gthyzisioz.html

JS:   while (i < 10) { i++; }
来源：http://hz.ehwqpu.com/gtaohfexcq.html

TS:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtqxkdtayo.html

Java: while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gttsmckqrp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinghuilouyu.cn/gtmowpnsga.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aizwys.cn/gtbindikff.html

C#:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gttsaigecp.html

[B08] do-while（至少执行一次）
来源：http://hz.ywan-chungtsiang.top/gtheblfazi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtbrvcoeri.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangdashe.top/gtrotasgji.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtpktfyfkk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtigktqlxr.html

Java: do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gttetthzif.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.9152youxi.cn/gtxtavhwzg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sufxvd.cn/gtxfuudaxz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtrsqvihie.html

[B09] break 与 continue
来源：http://hz.hnxiangtu.top/gtdtnvynci.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zycfv.cn/gtgculrscc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gturwbaalv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtywvqgeez.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtcizexlfc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtcbqgtthx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gthjlseuhr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.kuanghao11.cn/gtnyyzcgtc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gteyetuhrc.html

[B10] 遍历同时拿索引
来源：http://hz.yuanzhike.top/gtzlrxcske.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gotoacloud.top/gtrrgnxvqu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ybcxt.top/gtjeqinryl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtujwtfhbm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.redwolf501.top/gtuqvjcavk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnqzz.top/gtoyhgsqqp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgufenzy.top/gtoectcqdg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.haohaochexian.top/gtjnyauzpm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.feifeiyinyue.top/gtdkauxkol.html

[B11] 生成数字序列 / 区间
来源：http://hz.andypj.xyz/gtledugzcs.html

Py:   list(range(0, 10, 2))
来源：http://hz.ydzc1.top/gtymqfihse.html

PHP:  range(0, 10, 2);
来源：http://hz.zhoulong.xyz/gtjwvxlmjz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtbyhpdkom.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cucudq.cn/gtmecfljui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hammf.cn/gtqoohlbpl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daria6918.cn/gtkoqmrfma.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtkjhnsnck.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fengsongda.top/gtcwaohcse.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtizicgfus.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tianlin.xyz/gtrrjenask.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.52xcode.cn/gtrdfzculi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtyuacydsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtwjlgyqqn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtawybggfj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtlvkffbgs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenjidiqi.icu/gtwiqlnckt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinyuanbaomall.cn/gttjwtpyzg.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtndutrkoj.html

Py:   isinstance(x, (int, float))
来源：http://hz.gzhubu.top/gtoxcftkjr.html

PHP:  is_numeric($x)
来源：http://hz.meibo888.top/gtkheqcpvx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtwcnjtjny.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtyqhjkbdy.html

Java: x instanceof Number
来源：http://hz.sysykeji.top/gtxgxkgqcd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhaomingkeji.xyz/gtceapyqdp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydzc1.top/gtyipfswep.html

C#:   x is int or double or decimal
来源：http://hz.jinghuilouyu.cn/gtawfuygaz.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtvyeifouh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtbjelcwyh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.havefunace.top/gtmxqhctqz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtpcznachg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtjpbbxspu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daria6918.cn/gtvakbsemn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtmwywgwec.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinyuanbaomall.cn/gtumsinkdd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtzicehvzu.html

[B15] 布尔运算与取反
来源：http://hz.pycfn.com/gtymibkemc.html

Py:   a and b or not c
来源：http://hz.wangshuangyany.cn/gtaxhcdcmb.html

PHP:  $a && $b || !$c
来源：http://hz.aizwys.cn/gtoivrylao.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtsefhxjmf.html

TS:   a && b || !c
来源：http://hz.quarkkingdee.top/gteoqhxjws.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtkdicqngd.html

Go:   a && b || !c
来源：http://hz.andypj.xyz/gtpbyvpvbx.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtwdawverc.html

C#:   a && b || !c
来源：http://hz.jinqigufen.top/gtmawdepth.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtydsozbpk.html

Py:   if not data: return
来源：http://hz.yuxming.cn/gtjdcwakhu.html

PHP:  if (!$data) { return; }
来源：http://hz.fzhhl.top/gtebmbmwnm.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtadojwzne.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtxqnuztmt.html

Java: if (data == null) return;
来源：http://hz.cdnleiting.top/gtmipmqfeh.html

Go:   if data == nil { return }
来源：http://hz.sufxvd.cn/gtsvbcigtx.html

Ruby: return if data.nil?
来源：http://hz.hammf.cn/gtcisofyjf.html

C#:   if (data == null) return;
来源：http://hz.ppjwa.cn/gteysuejjd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkobmjthd.html

C. 函数与作用域
来源：http://hz.hongshengwenyu.top/gtfjzbrhth.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtiptpzgzt.html

[C01] 定义函数
来源：http://hz.yanxiufei.cn/gtoosigbdy.html

Py:   def add(a, b): return a + b
来源：http://hz.cashguo.top/gtxuokcrvu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtwngdeumx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtbbpplunu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtsxcrcgsp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtonapjjvn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenjidiqi.icu/gtnpjywgus.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ybcxt.top/gtblshjnij.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtlhqadaoh.html

[C02] 默认参数
来源：http://hz.zhongyouzk.top/gtsasiqvvi.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gtbbdelczn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jlsjyb.cn/gtqczidyeg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gtllnqqoyd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenzaomai.com/gtuqxshsjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.smart0.xyz/gtlhojcxrh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fengsongda.top/gtpxghukmm.html

Ruby: def greet(name = "World") = name
来源：http://hz.svipenyu.cn/gtvhpqweqp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhongyouzk.top/gtfuhftlza.html

[C03] 可变参数
来源：http://hz.sweek.top/gtdojfxrsr.html

Py:   def total(*args): return sum(args)
来源：http://hz.vqdsnc.cn/gtmyzbmmcm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gogol.net.cn/gtekqurbba.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtfluwrqdl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtsxnhphwv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtupoguzvu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gtjszsytmw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangdashe.top/gtrzfgwzwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gtcbtrmdeb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtquozudoa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtjtjcqdyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhiwuduotai.top/gtewegkobd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtcojlspat.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuxming.cn/gtfyoeixkr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigufen.top/gtgjwtfjze.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtdkwlpovi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtqjpssqra.html

C#:   f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtvwoxrnye.html

[C05] 返回多个值
来源：http://hz.shangyingyoupin.top/gtzxpwsfwd.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtjmfmvdne.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtxuemluch.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtofvsilzf.html

TS:   return { a, b };
来源：http://hz.ywan-chungtsiang.top/gtdriaffoj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hongshengwenyu.top/gtfthaayfy.html

Go:   return a, b
来源：http://hz.tanke756.top/gtjoxhpwco.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gttljrsyxa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gaohongyu789.top/gtgrrnzkaj.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtmlmqvwpr.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtkbkpwiim.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guowangkeji.top/gtacbvzlsa.html

JS:   const square = x => x * x;
来源：http://hz.shzxlz.cn/gtadojvefv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtiybolsbz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtdaqkpcke.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtpyyyjdxe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangshuangyany.cn/gtqvexvlcx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guowangkeji.top/gtpvfvhldd.html

[C07] 把函数作为参数传入
来源：http://hz.ybcxt.top/gtxhbkuaes.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydjk.org.cn/gtjfullrzu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sysykeji.top/gtxaigswmc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtkhkxewop.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtdjdpshls.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gzhubu.top/gtonqgegdb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.c1oappe.top/gtczcxcqmt.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtjtrvbqvi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtsjfousch.html

[C08] 闭包
来源：http://hz.hnqzz.top/gtuwadezpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zycfv.cn/gthkotqtoo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xinyue.icu/gtapryhapc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtnidancsg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtjdhyyqni.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tanke756.top/gtrpmksvln.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtffuusrxv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gtgvtywrgo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtkxptmrpo.html

[C09] 递归
来源：http://hz.tanke756.top/gtkhnqajdm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtfhywfpnt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtkigbarkr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gthhrnhtgj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtvxdgngcs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtmbzoqyfr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hysaishi.cn/gtrnxwkgsq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtzattscrj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shzxlz.cn/gtpvqoidmx.html

[C10] 变量作用域
来源：http://hz.yj202588.top/gtkiewwqmm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shzxlz.cn/gtghmfwjrm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.andypj.xyz/gtpwaniorj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtcfswmvvm.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtuzofnzcv.html

Java: 方法内为块级作用域
来源：http://hz.shzxlz.cn/gtbxrrmkjj.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtcnzxjqeo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtwzczcsib.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtrwpzevcg.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gttltcdjie.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtepkpkcck.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtemhqaoir.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtukpyepxj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtglspelvp.html

Java: import java.util.List;
来源：http://hz.zdqjudy.top/gtuhcpwxqv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sweek.top/gtllvdvsdp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtknumhdla.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtrpizthrc.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gtitstdxqo.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtvjmqbbvl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gthkmbntbf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtgqlqzeph.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtytuoaxqd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtamugpmsw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtvanuhwwj.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtuelortvm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtxdonmnxr.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuanzhike.top/gtkdpxjgaa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shzxlz.cn/gtkbjhhscz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtdojxdbxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtksukwamw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtflqrwxnx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtysxjqpli.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtsovedwhg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jianghu66.top/gtjozuiidz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgufenzy.top/gtuyrzpqfz.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtfziuvghy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangtech.top/gtjvwuturf.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtgsxbuynv.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtdqpzaxxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tanke756.top/gtsgaomqfa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtycocqbfm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtpvzmzgir.html

Ruby: # 无泛型
来源：http://hz.jinyuanbaomall.cn/gtmxromeot.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtthnrvjai.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtsfwgpjlm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtepzevdoc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gthegfcjhr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtfnfquewh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtyuebhxkd.html

Java: // 无解构
来源：http://hz.ivvv.top/gtzbsydvbz.html

Go:   // 无解构
来源：http://hz.jinqigufen.top/gtidhovrfz.html

Ruby: a, b = pair
来源：http://hz.xuanzx.com/gtktlmjgnx.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gthoniobnl.html

[C16] 函数 / 方法重载
来源：http://hz.vqdsnc.cn/gtmqegftud.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zdqjudy.top/gtzgntrrlc.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtfgwhdglo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pycfn.com/gtimsriaek.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtiwbwvurr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtuuxsfbsy.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gtwjufqnwh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtkumckfts.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtvrhkatyy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwintjlgo.html

D. 数组 / 列表 / 集合
来源：http://hz.redwolf501.top/gtrhdqdwjt.html

================================================================================
来源：http://hz.jiagoushi.top/gtrskoavbs.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gtncegfrei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtpnhvkzwj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydjk.org.cn/gtgwaerywj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shuidangran.top/gtgylzeqju.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhijiandao.cn/gtqmywmzeb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangdashe.top/gtjpncywar.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtbosqrzvh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtcidxedcf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj202588.top/gtfmekafij.html

[D02] 追加元素到末尾
来源：http://hz.kuanghao11.cn/gtyqndmyue.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gtmeewvjph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gogol.net.cn/gtkpxcqqek.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtettsduqx.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtubvbiyeu.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtlxxzdagq.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gtlfezsnxw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dashuyun.cn/gtxyvkiwto.html

C#:   list.Add(4);
来源：http://hz.52xcode.cn/gthzmhrjsc.html

[D03] 在指定位置插入元素
来源：http://hz.snrcjt.cn/gttefaeevp.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtwnvrslrw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xylfe.cn/gtmglxgibd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.smart0.xyz/gtxztkixgu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aizwys.cn/gtnzuhlcpk.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtgshcnoqs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shzxlz.cn/gtykbiipra.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gthctcdenv.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtrhxgfppb.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtxouipbmh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtlbmetruq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtltwmfels.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gtyquksshc.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtqgpdmlez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tanke756.top/gtfngjunnt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cashguo.top/gtlantzjlm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtwclpwkca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gthnyndukv.html

[D05] 访问与修改元素
来源：http://hz.feifeiyinyue.top/gtbbtzoxgf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtpsvmrwqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtabqjvzls.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gotoacloud.top/gtedscdbmd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtslxhcoac.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtanzrsnic.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtlyxuiqjv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtxvpordul.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtorkcpgsj.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtkeltxaqh.html

Py:   len(arr)
来源：http://hz.cqqwz.cn/gtvmmqdsbm.html

PHP:  count($arr);
来源：http://hz.316326.xyz/gtshrvypud.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtzzdgigut.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtmsrpxrdg.html

Java: list.size();
来源：http://hz.tianlin.xyz/gtpztdaekb.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtiapsyznc.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gtkxenrxvr.html

C#:   list.Count;
来源：http://hz.dashuyun.cn/gtecbaqwzb.html

[D07] 切片 / 取子数组
来源：http://hz.smart0.xyz/gtpngjphow.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ybcxt.top/gtmzcqyeqz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtdflfkmny.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gthjvmwvww.html


<!-- 参考信息 -->