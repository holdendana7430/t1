代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hnxiangtu.top/gtgddgkvkv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ydzc1.top/gtnlvuvlip.html

[B07] while 循环
来源：http://hz.jqgufenzy.top/gtjzbkdktt.html

Py:   while i < 10: i += 1
来源：http://hz.guowangkeji.top/gtsmrtjbrf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.pengpengdd.cyou/gtyhbbzvyd.html

JS:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtzxwudhcn.html

TS:   while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gttamyusfn.html

Java: while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtckfhohep.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shangyingyoupin.top/gtvexegmhb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yonumen.top/gtgmwmbfsy.html

C#:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtudjhpgcg.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtawwvgebc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigfzy.top/gtvgcssujh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtnucsoypf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtathauqqh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtjhibuxak.html

Java: do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtiobjyspf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.haohaochexian.top/gtcxggxxbf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jyoumei.cn/gtcxuqdapp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtzqqdynhn.html

[B09] break 与 continue
来源：http://hz.hnxiangtu.top/gtpohhuodc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ehwqpu.com/gtatcekfta.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ppjwa.cn/gtvujhrloe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gttxhbhrxj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daxiang520.top/gtrbzsxjmc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtzohsbudv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.quarkkingdee.top/gtqazbittt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sysykeji.top/gtvtxrhtgp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtqaktzdvj.html

[B10] 遍历同时拿索引
来源：http://hz.xziqi.cn/gtsckxuhnd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.iojbl.cn/gtoeajxsso.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhiwuduotai.top/gtbgsvtnva.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtgfitynhw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinyuanbaomall.cn/gtuefjghtq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fzhhl.top/gthnlswnxe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gaohongyu789.top/gtkspsoofq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jianghu66.top/gtdkvubmsa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.svipenyu.cn/gtujhqbcxc.html

[B11] 生成数字序列 / 区间
来源：http://hz.9152youxi.cn/gtkgcxcrtp.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhaomingkeji.xyz/gtbsygkqls.html

PHP:  range(0, 10, 2);
来源：http://hz.hnqzz.top/gtcvvfmmnm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtoaijrifi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ivvv.top/gtxlgurkwr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hfpthk.cn/gtwuqqnwtt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gtlytlsmmi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtulxbffil.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenzaomai.com/gtmlxloavp.html

[B12] 跳出多层循环
来源：http://hz.dianchejie.cn/gtzqmdvmcz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.quarkkingdee.top/gtgbqawrza.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.feifeiyinyue.top/gtdezcgzrh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtmmhsibnr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenzaomai.com/gtcjcmtaji.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.aibaodan.cn/gtnqbxaqyn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtjknojzmo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cqqwz.cn/gtcpiiofaw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangdashe.top/gtsamzhiug.html

[B13] 判断是否为数字
来源：http://hz.meibo888.top/gtdcwkwxyy.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gtaxbxnekp.html

PHP:  is_numeric($x)
来源：http://hz.hnqzz.top/gtjjlacczx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtobvkebqy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtgheuvgwy.html

Java: x instanceof Number
来源：http://hz.hfpthk.cn/gtqjqlqewc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgufenzy.top/gttknlaevi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dashuyun.cn/gtgepegitc.html

C#:   x is int or double or decimal
来源：http://hz.havefunace.top/gtwremfhdv.html

[B14] 判断值是否在集合内
来源：http://hz.snrcjt.cn/gtsbzzaodh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangtech.top/gtitozugds.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sysykeji.top/gtwubmrhch.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtymielizz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtjcpmbtnc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhoulong.xyz/gtbnmxgiqg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.vqdsnc.cn/gtfzbxopum.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yonumen.top/gtfzorqqul.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgufenzy.top/gtuyfcxosr.html

[B15] 布尔运算与取反
来源：http://hz.zycfv.cn/gtdachnxxk.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtdyxadtia.html

PHP:  $a && $b || !$c
来源：http://hz.gaohongyu789.top/gtvuvmhrvb.html

JS:   a && b || !c
来源：http://hz.aizwys.cn/gtrlziishk.html

TS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtyoajodef.html

Java: a && b || !c
来源：http://hz.52xcode.cn/gtwpphopns.html

Go:   a && b || !c
来源：http://hz.fengsongda.top/gtctxqtjrv.html

Ruby: a && b || !c
来源：http://hz.havefunace.top/gtltprjtst.html

C#:   a && b || !c
来源：http://hz.tanke756.top/gttmqyxmfx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnqzz.top/gtsaykzatt.html

Py:   if not data: return
来源：http://hz.tanke756.top/gteuvxiyzb.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gttjooyauv.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gtauhbyeto.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtyasrqeyz.html

Java: if (data == null) return;
来源：http://hz.zhoulong.xyz/gttmfcjggd.html

Go:   if data == nil { return }
来源：http://hz.316326.xyz/gtdirlrqng.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtyhvwfczv.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtqozttqho.html

================================================================================
来源：http://hz.c1oappe.top/gtspgatlzy.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtwcrrvpuo.html

================================================================================
来源：http://hz.yj20258.top/gtgkpctrfm.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtexufnwmt.html

Py:   def add(a, b): return a + b
来源：http://hz.zdqjudy.top/gtxraaspfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtqapyohmj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtlfcrfhve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtdjvkghft.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtjzxtpdcg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.haohaochexian.top/gtstubyagd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtkknegwmx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gttwphrkkc.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtcsvyaxcp.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gtpiunupwp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydjk.org.cn/gtenyrfszr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj202588.top/gtnjaolgwg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtweqslnkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhaomingkeji.xyz/gtomqovfzj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtwcusjvse.html

Ruby: def greet(name = "World") = name
来源：http://hz.meibo888.top/gtxyoajlgy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtofgyaaid.html

[C03] 可变参数
来源：http://hz.52xcode.cn/gtpkjsatra.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gtxckhqomw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hongshengwenyu.top/gtufgtebvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtmzaisqwy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtmidqqmmh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pengpengdd.cyou/gtvugdowxw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gtghmtjixa.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtyvqdufcb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhijiandao.cn/gtgsyfoinu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gtwjbqpvmh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtqumiwncf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtfqvvfkrw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gthsosxzzu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.haohaochexian.top/gtkksdxnkr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gtcbmjopay.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtkfidbfql.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtedhblwjj.html

C#:   f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtyhxukylo.html

[C05] 返回多个值
来源：http://hz.ywan-chungtsiang.top/gtuhhgubtb.html

Py:   return a, b
来源：http://hz.xziqi.cn/gtdwchgfjh.html

PHP:  return [$a, $b];
来源：http://hz.xuanzx.com/gtrgulcoke.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.316326.xyz/gtvtroprun.html

TS:   return { a, b };
来源：http://hz.dianchejie.cn/gtkzylouky.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtokrrqhiu.html

Go:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtnfzdhxfb.html

Ruby: return a, b
来源：http://hz.svipenyu.cn/gtplgjkaml.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhaomingkeji.xyz/gtatupwrry.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtjvwcthvu.html

Py:   square = lambda x: x * x
来源：http://hz.zhiwuduotai.top/gtvcywofeo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.bjfxy.top/gtpjkwxncd.html

JS:   const square = x => x * x;
来源：http://hz.yj20258.top/gtysnqpbvj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtqvzxsjcd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenjidiqi.icu/gtvarnhwbh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.c1oappe.top/gtezeibxui.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gotoacloud.top/gtalgcknrq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258888.top/gtvpkqhrwb.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gttsuaeaud.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zycfv.cn/gtbxondwbd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gotoacloud.top/gtrdnqyrkb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aizwys.cn/gteulbigic.html

TS:   arr.map(String)
来源：http://hz.gotoacloud.top/gtfbkdfmdk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.svipenyu.cn/gttqsgcozr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtwlagmucn.html

Ruby: arr.map(&:upcase)
来源：http://hz.yanxiufei.cn/gtirzmtvck.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.redwolf501.top/gtjaefwscp.html

[C08] 闭包
来源：http://hz.birdmap.top/gtulvayenj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtvlwramid.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenjidiqi.icu/gtwtameihl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtrnzsdfot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtkxthunqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtqbsvzvsm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ivvv.top/gtnatpvwdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gtqfbvgoqh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtcfbcheyt.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtfdbkhuqk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtiipydchm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhiwuduotai.top/gthnbvgkdu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtkuuyotlr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtxbhmxlfz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.havefunace.top/gtsdqrtgaf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhiwuduotai.top/gtpwrnezxw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gtywacxrrp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtglyyszvd.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtqlqwiowb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tianlin.xyz/gtbrdiesmt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhaomingkeji.xyz/gtxbdevfrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtkwzppqwx.html

TS:   同 JS
来源：http://hz.jianghu66.top/gtqvdxlnji.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtnjdsqoxn.html

Go:   花括号块级作用域
来源：http://hz.sufxvd.cn/gtzzauczge.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258888.top/gtjotiqidz.html

C#:   块级作用域
来源：http://hz.hammf.cn/gtefztihnj.html

[C11] 模块导入与导出
来源：http://hz.gzhubu.top/gtrgewcyvp.html

Py:   from module import func
来源：http://hz.jinqigfzy.top/gtzwnjydyx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cucudq.cn/gtkzqxxvvx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtzgclusou.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gttaoyjnjj.html

Java: import java.util.List;
来源：http://hz.gotoacloud.top/gtpwtqwzrp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtdynphiqs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtxbxnbibu.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gtbeonsdtv.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtughnsdbk.html

Py:   (lambda: print("run"))()
来源：http://hz.snrcjt.cn/gtbhqlpoty.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtboqnpemi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gtyqzekpob.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtcssammab.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yueranfly.top/gtjegjjcro.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtjrxoqlhz.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gtrmrnimgi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tian-w.cn/gtugqavyet.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhijiandao.cn/gtfgceunpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtzwxcavku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtttrsgljt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.iojbl.cn/gtpgxtshgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gtxruxtycb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtdqdnlaex.html

Go:   func add(a, b int) int
来源：http://hz.chenlongwang.top/gtuepvsvkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shzxlz.cn/gtkrrevley.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yanxiufei.cn/gtszrsplor.html

[C14] 泛型函数
来源：http://hz.jianghu66.top/gtmrdhvnuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gtwjnazolt.html

PHP:  // 无泛型
来源：http://hz.zdqjudy.top/gtjnfqcixm.html

JS:   // 无泛型
来源：http://hz.hfpthk.cn/gtltsgpgxt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gthwbqodin.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtkdnknvnn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuetiantiany.cn/gtpdneyysu.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtgkgoyyeu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gtlvcgswki.html

[C15] 解构 / 展开参数
来源：http://hz.hnqzz.top/gtuacbyhuo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtlntdlvac.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shzxlz.cn/gtxvvcpygf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtrozbeclx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.mhx1999.top/gtpclcfiiq.html

Java: // 无解构
来源：http://hz.gotoacloud.top/gtymqynzbp.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gtorsqihcy.html

Ruby: a, b = pair
来源：http://hz.jinqigufen.top/gtpvtakttv.html

C#:   var (a, b) = pair;
来源：http://hz.jinyuanbaomall.cn/gtatzvqfpm.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtbalrfcmt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtxjicsses.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gtvcakgyfu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258888.top/gtqlkzpnqh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuanzhike.top/gtlayuayir.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtelzixtcs.html

Go:   // 无重载：用不同函数名
来源：http://hz.sxryk.cn/gtoyacwuxr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sufxvd.cn/gtshpqrtym.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gthvpfqygo.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvwugcyib.html

D. 数组 / 列表 / 集合
来源：http://hz.havefunace.top/gtogzwiwqi.html

================================================================================
来源：http://hz.9152youxi.cn/gtqwvbenuf.html

[D01] 创建数组 / 列表
来源：http://hz.tanke756.top/gtgbcbeaoq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtoxaqtjbr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtqranmmlh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinghuilouyu.cn/gtvoawnzzg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shangyingyoupin.top/gtqurzmekm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yanxiufei.cn/gtjvqwsowi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yanxiufei.cn/gtzzkuyzor.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cdnleiting.top/gtmazzneog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tianlin.xyz/gtawcvpoya.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtxnlbrrho.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgfzy.top/gtrxdpctyi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtrcphivam.html

JS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtsxifustt.html

TS:   arr.push(4);
来源：http://hz.bjfxy.top/gtsbzvevxg.html

Java: list.add(4);
来源：http://hz.yonumen.top/gtrzzfutiy.html

Go:   arr = append(arr, 4)
来源：http://hz.xingfuxueyuan.xyz/gtjqsmcyjk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gthvkpzvxe.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtbcyyssuj.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gteumjmezi.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gtzylhbeaj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuetiantiany.cn/gteakflrvp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtigvvhjxi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.52xcode.cn/gthriuamqr.html

Java: list.add(0, 0);
来源：http://hz.jqgfzy.top/gtcbvyupsg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hongshengwenyu.top/gthitgsxmg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xuetiantiany.cn/gtuaemmicw.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtaskrmzyg.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtuqnnqxcr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tanke756.top/gtryqwjxqx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gthbzsxplw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangshuangyany.cn/gtlqucqxmz.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangkeji.top/gtduxekgdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenlongwang.top/gtgqsyqnam.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuetiantiany.cn/gtqmvprblz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gtxcjlhbkr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtlopfqupo.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtlvfxuzea.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtxzyppyop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cqqwz.cn/gtablnedjr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gteejrkdtn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gtfhexidhu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtpovcihgh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gtanhbozmb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtdashancu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtrorzjvgn.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtuxxbnsqb.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gteylexlmg.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtlhvxgrzi.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtrawhzevu.html

TS:   arr.length
来源：http://hz.jianghu66.top/gtvkzkvswy.html

Java: list.size();
来源：http://hz.meibo888.top/gtjxlmfowf.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gthzzdsapd.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gtxfdrbwpe.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gttptsbcyi.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtyjrongvz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dashuyun.cn/gtlkvafjqj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtvfvlssyu.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtokceoway.html


<!-- 参考信息 -->