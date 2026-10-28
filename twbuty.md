代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtexbgjipg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.9152youxi.cn/gtbeouoiov.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jianghu66.top/gtmxxcckgg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtkgoighna.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtkxpmotvc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pengpengdd.cyou/gtmnwastdx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cdnleiting.top/gttxusifva.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtzcnknbrt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtobhhrbtm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtdnydxosz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.snrcjt.cn/gturtrujyw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuanzhike.top/gtqhkcigpa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtuugrluls.html

[B10] 遍历同时拿索引
来源：http://hz.chenjidiqi.icu/gtkczzllbv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtvxpzxgao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xylfe.cn/gtshvncyit.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.aizwys.cn/gtuqrlzleh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jyoumei.cn/gtqdihqyyq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gtktdnnebw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhengqikj.top/gtfqwxgutk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xziqi.cn/gtyslrbuso.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gttlqpdnee.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtvgpfurtb.html

Py:   list(range(0, 10, 2))
来源：http://hz.yonumen.top/gtezyxayiq.html

PHP:  range(0, 10, 2);
来源：http://hz.daxiang520.top/gtpimmdumc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtbnzcdfoq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gttpmuxocr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gttpryfojm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zdqjudy.top/gtvjaqvwga.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hysaishi.cn/gtxhbyavjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenzaomai.com/gtzqatzfzz.html

[B12] 跳出多层循环
来源：http://hz.wangshuangyany.cn/gtrljindbl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gtgqmpmhga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.9152youxi.cn/gtqvarntre.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtyokbbgui.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gttnuoccbn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gttkftcaul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.aizwys.cn/gtvuzttfmq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jianghu66.top/gtngbfulto.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cqqwz.cn/gtmcsamnjz.html

[B13] 判断是否为数字
来源：http://hz.gaohongyu789.top/gtolguzadr.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtgsyqjutl.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtrxzkrrzd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtskcqjsbq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtzzxwuywi.html

Java: x instanceof Number
来源：http://hz.snrcjt.cn/gtxqzpayzq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtdfhcojac.html

Ruby: x.is_a?(Numeric)
来源：http://hz.birdmap.top/gtbslrsoev.html

C#:   x is int or double or decimal
来源：http://hz.shzxlz.cn/gtmlvondkz.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtvwtclkhd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shuidangran.top/gtnuhaqwvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.vqdsnc.cn/gtplqksutm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtmhmexwdh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtbhzvfymm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenzaomai.com/gtbmqhmjpf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.birdmap.top/gtoenkscpv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tian-w.cn/gtizsbnzuj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aizwys.cn/gtxxrxthpj.html

[B15] 布尔运算与取反
来源：http://hz.hongshengwenyu.top/gtcgvxrkgg.html

Py:   a and b or not c
来源：http://hz.aizwys.cn/gtcmczmhzo.html

PHP:  $a && $b || !$c
来源：http://hz.sysykeji.top/gtbheojgew.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtuyqsldeo.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtwhvuqioj.html

Java: a && b || !c
来源：http://hz.hfpthk.cn/gtymjsflac.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gtkocwrcfr.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gteswjgwwe.html

C#:   a && b || !c
来源：http://hz.cashguo.top/gtscyzsovu.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.havefunace.top/gtkxilwute.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gtgwktccbu.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtdrfnzuyk.html

JS:   if (!data) return;
来源：http://hz.yj20258.top/gtbehbcsqp.html

TS:   if (!data) return;
来源：http://hz.yvedp.cn/gtpqtvkuvk.html

Java: if (data == null) return;
来源：http://hz.nwbrower.top/gtonqjkovi.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtnzmolfkb.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtareuxzqp.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtarrqlpde.html

================================================================================
来源：http://hz.meibo888.top/gtbeqairsq.html

C. 函数与作用域
来源：http://hz.birdmap.top/gtoqpyqkcq.html

================================================================================
来源：http://hz.nwbrower.top/gtvqitjyqm.html

[C01] 定义函数
来源：http://hz.ydjk.org.cn/gtosakpmex.html

Py:   def add(a, b): return a + b
来源：http://hz.yuxming.cn/gtpfremluy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtamkbuzpw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtgughjwaa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtlzsiwkoy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtjyevybzm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj202588.top/gtlsechmrq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhengqikj.top/gtnsgrwpux.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gttihzrujl.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtsfwymzdx.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtrumxwkbf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.havefunace.top/gtxxaiguvh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtcdzvfkfw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtspadiylv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aizwys.cn/gtwexbnthu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtrzfiyxov.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigfzy.top/gtyrfmihas.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtebwckrvv.html

[C03] 可变参数
来源：http://hz.redwolf501.top/gtlmpskdsg.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gtumrosdqq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gtamescoht.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtrbujuquy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtgkcgkylv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhixingplan.top/gtbuwympvv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtkvlejyml.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangkeji.top/gtbqvlaqrt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtuhjyzafe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtocweuofk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yonumen.top/gtiuonbrhs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gttfntfdqz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtxxuazojx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxuanxn.top/gtfxvmjrah.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenlongwang.top/gtbcgsssfi.html

Go:   // 无：用配置结构体参数
来源：http://hz.shuidangran.top/gtuwbbjqwn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtiialzkde.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtxneclvno.html

[C05] 返回多个值
来源：http://hz.sysykeji.top/gtwwsmszno.html

Py:   return a, b
来源：http://hz.mhx1999.top/gtpbnqmqyk.html

PHP:  return [$a, $b];
来源：http://hz.yonumen.top/gtalilhuyc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gthrojddxd.html

TS:   return { a, b };
来源：http://hz.jqgufenzy.top/gtnxmbmdly.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gttofpokkf.html

Go:   return a, b
来源：http://hz.ivvv.top/gtvihpgysf.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtwqwhnuet.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yonumen.top/gtmcksojpi.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtdnngmgjd.html

Py:   square = lambda x: x * x
来源：http://hz.snrcjt.cn/gtrrokjfsr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gtfhhcybgy.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtskuvszbx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jiagoushi.top/gtrdhvkitp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtqnaktjlj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtpmgalfun.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gtyyhtqjtl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtboyppjqy.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtlicraweg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtcstapprr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gthxmjvfae.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtgwxlbnpf.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gtrfuoybwq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtidwuuzvr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gtquwkhchz.html

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtxpgwfrwg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangdashe.top/gthvbxijgi.html

[C08] 闭包
来源：http://hz.iojbl.cn/gtlcydpffr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gogol.net.cn/gtwpggcqwd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yonumen.top/gtwcrugkan.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtgdorufcl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtztqadtbx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtilmlbrld.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtrtsubzhb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tian-w.cn/gtooydjxav.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtxgfacglx.html

[C09] 递归
来源：http://hz.meibo888.top/gtzcppsxzl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtbuonzwpk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zycfv.cn/gtiuaorsag.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtgyailztj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gtqrcshmgc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cdnleiting.top/gtrpgopeea.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtfuhnvdek.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtamgdjujb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gteheovovy.html

[C10] 变量作用域
来源：http://hz.hysaishi.cn/gtqodmxhuq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtksscyuyb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtymmhfzkn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxuanxn.top/gtpzunnyvv.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtyeynqzzq.html

Java: 方法内为块级作用域
来源：http://hz.vqdsnc.cn/gtbgcfdrkz.html

Go:   花括号块级作用域
来源：http://hz.xuetiantiany.cn/gtjjpqxvoj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.kuanghao11.cn/gtauidcytc.html

C#:   块级作用域
来源：http://hz.jinqigfzy.top/gtsmzrhcsi.html

[C11] 模块导入与导出
来源：http://hz.zhaomingkeji.xyz/gtuxnyjvxk.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtkiqnonrb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtxavpwmjo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gtvstwvpez.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtetnxnucd.html

Java: import java.util.List;
来源：http://hz.zhongyouzk.top/gtclwngrqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hammf.cn/gtiwambzyp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtgvbtfvwz.html

C#:   using System.Text;
来源：http://hz.yj20258888.top/gtamkxdpyo.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gtljuizrki.html

Py:   (lambda: print("run"))()
来源：http://hz.52xcode.cn/gtcipkfrue.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gtowtwzews.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtqpddhqtj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtyultrvdn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yangfankeji.com/gtrzftvhuu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.havefunace.top/gtzlzgerua.html

Ruby: -> { puts "run" }.call
来源：http://hz.havefunace.top/gtxhffeybf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gtrwpvquhp.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gthobgvycz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gotoacloud.top/gtajuwkqxd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtnawujtsk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtzhnlhmff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtqatcrxax.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtaurkkwkg.html

Go:   func add(a, b int) int
来源：http://hz.yonumen.top/gtizsttdkp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtlwxirdso.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtoecrexcc.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtmpyqafyt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sufxvd.cn/gtgzcluiuv.html

PHP:  // 无泛型
来源：http://hz.cdnleiting.top/gthzpshaqo.html

JS:   // 无泛型
来源：http://hz.yuxming.cn/gtqcmlcnfi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.kuanghao11.cn/gtzfxfsdfm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtwqhjdbek.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtkgoliiza.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtoooniepe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cucudq.cn/gtixyzlkxb.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtrtnyvsyh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.quarkkingdee.top/gtspvuqglb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtzbxxzjkh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtelgwhtsd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtvnwrwbta.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtmrsefusc.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtqlkdslhm.html

Ruby: a, b = pair
来源：http://hz.jqgufenzy.top/gtvfdaosax.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtvhqszcka.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtpvsjomio.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtjsnfccfe.html

PHP:  // 无重载
来源：http://hz.meibo888.top/gtvgmoiyyg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yangfankeji.com/gtajodaajw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigufen.top/gtcgostdbb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gtqfarpuzc.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtvqxzunjj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fengsongda.top/gtekrnxdcc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhongyouzk.top/gtyxaadogg.html

================================================================================
来源：http://hz.shuidangran.top/gtzkxdrtxb.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtjntqoslj.html

================================================================================
来源：http://hz.redwolf501.top/gtxyeusdwr.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtmbygrcxr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtbqztjfre.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenjidiqi.icu/gtieqxbojh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gthdxdycaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtpsuewlfm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtiijkfrnf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jyoumei.cn/gttmsphoud.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fzhhl.top/gtyymwvflw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtkvuwmxnj.html

[D02] 追加元素到末尾
来源：http://hz.bjfxy.top/gtplbihvww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtmwcgkzyn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtcdbhsoif.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gtmnhcifzt.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtojohwgkr.html

Java: list.add(4);
来源：http://hz.zhaomingkeji.xyz/gtdvmgzxtt.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtajbdtcwr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guowangkeji.top/gtfrgbphhq.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gthbhrqonf.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtiydyszod.html

Py:   arr.insert(0, 0)
来源：http://hz.xziqi.cn/gtcxyvbjtc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gtsgeqhaxv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtfymmmdzo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gogol.net.cn/gteszfqcxj.html

Java: list.add(0, 0);
来源：http://hz.vqdsnc.cn/gtozjwfilp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hfpthk.cn/gtrucufudn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtujwihbjp.html

C#:   list.Insert(0, 0);
来源：http://hz.yongpay.top/gtjsvvjhhj.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtjmdmfpky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtamcqycfv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guannengcc.top/gtkslvmzds.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.feifeiyinyue.top/gthnqsbglx.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtxtsgafrn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtotkwjyup.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtqthbqofy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtillptqfn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtibaiehuh.html

[D05] 访问与修改元素
来源：http://hz.cqqwz.cn/gtyljwsfxa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gttylhtfox.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtafrkzhhk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuanzx.com/gtrleduuzo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtoamfirks.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtwbvvrjfd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtcabyfyxf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtnfkzcuch.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtohnnazfn.html

[D06] 数组长度
来源：http://hz.yuxming.cn/gtkptsitmh.html

Py:   len(arr)
来源：http://hz.cheryme.top/gthhfzupzt.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtlzmyzdno.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtaatkbwfz.html

TS:   arr.length
来源：http://hz.mhx1999.top/gtgfltnnyp.html

Java: list.size();
来源：http://hz.svipenyu.cn/gtcoiqqlnz.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtedzzpxnj.html

Ruby: arr.length; arr.size
来源：http://hz.zhijiandao.cn/gtexqjwtoe.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtvwwdghbu.html

[D07] 切片 / 取子数组
来源：http://hz.shangyingyoupin.top/gtnnzculql.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtytdvnjpq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gtaucuezxt.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtsfwxrgnw.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtziybclxx.html

Java: list.subList(1, 4);
来源：http://hz.vqdsnc.cn/gttfcycets.html

Go:   arr[1:4]
来源：http://hz.xylfe.cn/gthofirpuq.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtlgdbtnyr.html

C#:   list.GetRange(1, 3);
来源：http://hz.ybcxt.top/gteiifxnxp.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gtewpxhjdl.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtxwaeivxt.html

PHP:  array_merge($a, $b);
来源：http://hz.nwbrower.top/gtqgjoapsf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhiwuduotai.top/gtousazkot.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtqkcvfdtc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtbbwmtrbf.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtaipudoox.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtwmbmzaqw.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtmgpmipfc.html

[D09] 排序（升序）
来源：http://hz.jinyuanbaomall.cn/gtwxghvewd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtemscoivn.html


<!-- 参考信息 -->