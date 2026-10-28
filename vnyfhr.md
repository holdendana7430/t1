代发 wailian999

[B09] break 与 continue
来源：http://hz.zycfv.cn/gtgqezzfyr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.dianchejie.cn/gtwuenkcsy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tian-w.cn/gtvczzhlci.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtijpcatbj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtogpbbcit.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtyjhkxhuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtbiqekurm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtbnvaimlw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtnmoxmxqb.html

[B10] 遍历同时拿索引
来源：http://hz.quarkkingdee.top/gtwrgehwiw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ydjk.org.cn/gtplcapwvh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.0kj1m.cn/gtimcejprc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtjlavgncq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinghuilouyu.cn/gtpdsexznq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xziqi.cn/gtntuzyayh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.redwolf501.top/gtqukamkwn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.nanxuanxn.top/gtboudeang.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sweek.top/gtigvyamfh.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258.top/gtipnjydhc.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtjnvgeipn.html

PHP:  range(0, 10, 2);
来源：http://hz.xuetiantiany.cn/gtfwyqohzc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhongyouzk.top/gtftnplwyt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtrymzezza.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtbnqyepsd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shuidangran.top/gtodrbaxei.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cheryme.top/gtglunmgbm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtkclckudh.html

[B12] 跳出多层循环
来源：http://hz.zhengqikj.top/gtzxhfkoyj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangkeji.top/gtezzcglhj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.birdmap.top/gtiiyyraar.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtdckwdftv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtuazroedy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtbexrvrbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuanzhike.top/gttlqhzwgn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dianchejie.cn/gtuynbmmxd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinghuilouyu.cn/gtjknbguem.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtuaieqmpw.html

Py:   isinstance(x, (int, float))
来源：http://hz.wangshuangyany.cn/gtzarpqmpt.html

PHP:  is_numeric($x)
来源：http://hz.xinyue.icu/gtnxprphet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.vqdsnc.cn/gttwqudrhw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtaxtgwpme.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtnpfirfkm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.svipenyu.cn/gtdqckzfyg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shzxlz.cn/gtxetjnghk.html

C#:   x is int or double or decimal
来源：http://hz.pengpengdd.cyou/gtfrnoensd.html

[B14] 判断值是否在集合内
来源：http://hz.zhengqikj.top/gtnrghpgqb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtojlwnmip.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ybcxt.top/gtdezmabvz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gtavlphmbj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gthyhnwqex.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dianchejie.cn/gtrlvvkzqb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.svipenyu.cn/gtzbqkkxzp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.smart0.xyz/gtzebcimoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xziqi.cn/gthiasohuf.html

[B15] 布尔运算与取反
来源：http://hz.hnqzz.top/gtezpeeumt.html

Py:   a and b or not c
来源：http://hz.yvedp.cn/gtqaborpuo.html

PHP:  $a && $b || !$c
来源：http://hz.hysaishi.cn/gtlccddlxa.html

JS:   a && b || !c
来源：http://hz.jinqigfzy.top/gteiaslvye.html

TS:   a && b || !c
来源：http://hz.tanke756.top/gtdvelbudx.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gtreiklbln.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gtoecbztex.html

Ruby: a && b || !c
来源：http://hz.yueranfly.top/gtasfykvcg.html

C#:   a && b || !c
来源：http://hz.yvedp.cn/gtylgqlbty.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sweek.top/gtwkthafqc.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gtjrveuqol.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gttaefdwnp.html

JS:   if (!data) return;
来源：http://hz.shangyingyoupin.top/gtjjegrnqq.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtyyxufcil.html

Java: if (data == null) return;
来源：http://hz.c1oappe.top/gtasxoqyeq.html

Go:   if data == nil { return }
来源：http://hz.xylfe.cn/gtfcdvcrhk.html

Ruby: return if data.nil?
来源：http://hz.ppjwa.cn/gtjkqlnzwu.html

C#:   if (data == null) return;
来源：http://hz.iojbl.cn/gtwfihhmea.html

================================================================================
来源：http://hz.hysaishi.cn/gtjoggqgyo.html

C. 函数与作用域
来源：http://hz.tanke756.top/gtdtbqyhdv.html

================================================================================
来源：http://hz.hnqzz.top/gtsawleuhn.html

[C01] 定义函数
来源：http://hz.c1oappe.top/gteddytlos.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtalslllrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtisknzebg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258.top/gtylbiwigb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtxyfsiube.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtbcnjoqck.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jiagoushi.top/gtipmvbvqs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.snrcjt.cn/gtaxpkmpzl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtuwvdrgvb.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtrubvgisx.html

Py:   def greet(name="World"): return name
来源：http://hz.jinghuilouyu.cn/gtorcnunlf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dianchejie.cn/gtdevwnnow.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuxming.cn/gtmxghmgmi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtbvxokjlk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.c1oappe.top/gtavieflvp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtxgzgodil.html

Ruby: def greet(name = "World") = name
来源：http://hz.dianchejie.cn/gtflnzraui.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.316326.xyz/gtegzvbvox.html

[C03] 可变参数
来源：http://hz.cdnleiting.top/gtitsxeqhg.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtakwomqdq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gtwgmqdpgh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtexuhktuw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gthbtcifbz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtoeukzcgo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtiautsxit.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtxblabzfl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gtigvohsgb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xingfuxueyuan.xyz/gtvoeqkwuh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gtcfomxjqp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shzxlz.cn/gtrbqdnwtc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtqzcmdjoh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.316326.xyz/gtcwhqfaku.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.haohaochexian.top/gtwpcvbeeq.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtdmayursl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtrihzfzfn.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtwbhcnlml.html

[C05] 返回多个值
来源：http://hz.xuanzx.com/gtxosyyqar.html

Py:   return a, b
来源：http://hz.smart0.xyz/gtwrsbzjma.html

PHP:  return [$a, $b];
来源：http://hz.9152youxi.cn/gtbxsdoyld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gzhubu.top/gtphmysiqi.html

TS:   return { a, b };
来源：http://hz.jqgfzy.top/gtbjqzwfai.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jiagoushi.top/gtsklilghy.html

Go:   return a, b
来源：http://hz.dashuyun.cn/gtniriomrj.html

Ruby: return a, b
来源：http://hz.daria6918.cn/gtuftlegqz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtlsjsakfm.html

[C06] 匿名函数 / lambda
来源：http://hz.andypj.xyz/gthvojnbpz.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtoyxpttss.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ydzc1.top/gtbsxkrqgs.html

JS:   const square = x => x * x;
来源：http://hz.chenlongwang.top/gtpifufsuo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtpfrlpzww.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gaohongyu789.top/gtetrpkghs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.iojbl.cn/gttimpjrmv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtmnuvzmob.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtczvggcnj.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gtekyxdxui.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtmspzclbh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yanxiufei.cn/gtzxdencae.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtslmneisu.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtyzqxaxcq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhengqikj.top/gtyrtifudq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtosohqbsr.html

Ruby: arr.map(&:upcase)
来源：http://hz.kuanghao11.cn/gttrixjdfo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.c1oappe.top/gtvuzymjxf.html

[C08] 闭包
来源：http://hz.shanyushiyangkeji.top/gtdccafyro.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xylfe.cn/gtbxkgxlfb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gtpslikliv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtbwmxmyji.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtwpaelfti.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtvngxnlsv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.vqdsnc.cn/gtdpfrkbew.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtmlhrxvmo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtwlpivtky.html

[C09] 递归
来源：http://hz.cqqwz.cn/gtmrysrxkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sxryk.cn/gtzfhqrepd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ybcxt.top/gtlfufinog.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gtumjpvhdb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtbjmipatp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtmjuilbzr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtsljocusc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtcfhwmcua.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ppjwa.cn/gtcgthxwds.html

[C10] 变量作用域
来源：http://hz.ybcxt.top/gtumsjdnlj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gtioppwqjc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zdqjudy.top/gtxvpwebxt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtjmgwykbm.html

TS:   同 JS
来源：http://hz.wangdashe.top/gtnyfxtwuk.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtlrisqpty.html

Go:   花括号块级作用域
来源：http://hz.316326.xyz/gtsvhqphfg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shanyushiyangkeji.top/gtmlvuwrsx.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtccnpjomp.html

[C11] 模块导入与导出
来源：http://hz.dashuyun.cn/gthplijdoq.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtsbvgpnbr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgufenzy.top/gtlgznqpnt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guannengcc.top/gtwipslecp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuxming.cn/gtoorvrcrq.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtjizwwxuw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ybcxt.top/gttlsphofa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtjksvhxev.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gtxymymham.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gtotjofwup.html

Py:   (lambda: print("run"))()
来源：http://hz.sufxvd.cn/gtkemvevab.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtklvnkxct.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtszcjthft.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gogol.net.cn/gtkgliqogb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gttcgtiytp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cqqwz.cn/gtgvoxsguv.html

Ruby: -> { puts "run" }.call
来源：http://hz.fengsongda.top/gtjhtggjxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtptsdzvlc.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtkkjjxuzd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xylfe.cn/gttdocpale.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gttvamuxyp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gtvgevrovx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hongshengwenyu.top/gtrbxlgllc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtahhvupwb.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtsqtdxttq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtlacznxwj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dianchejie.cn/gtxxxsqgmi.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtiszrrtjd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.havefunace.top/gtsibveuim.html

PHP:  // 无泛型
来源：http://hz.ehwqpu.com/gtzhmvyfcy.html

JS:   // 无泛型
来源：http://hz.meibo888.top/gtqnbkgyxa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtapppjtkz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtjulbakno.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinghuilouyu.cn/gtvqbxzfre.html

Ruby: # 无泛型
来源：http://hz.gogol.net.cn/gtsggsrore.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtnfbbnfnd.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtpodlwygh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtloefuhcs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.52xcode.cn/gtmbgpvpcy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtyitebmlf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtfkqfakdc.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtcfjvzjgo.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gtnscioqfq.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtrwkwkudw.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtyfvrracy.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtkbrgjzto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuxming.cn/gtwaigears.html

PHP:  // 无重载
来源：http://hz.wangdashe.top/gtheafdkmd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daria6918.cn/gtmcxhpkmt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhoulong.xyz/gtrjbpuqhp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sufxvd.cn/gtsnbperas.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtmixysido.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinghuilouyu.cn/gtrmwpfqfi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tanke756.top/gtbcdgflyr.html

================================================================================
来源：http://hz.hysaishi.cn/gtqlfuefqx.html

D. 数组 / 列表 / 集合
来源：http://hz.zycfv.cn/gteiyghqxv.html

================================================================================
来源：http://hz.havefunace.top/gtagikvcxd.html

[D01] 创建数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtmdrchmtw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtijdokgye.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtqrbmmcmm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jlsjyb.cn/gthhabjaqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cqqwz.cn/gtwiiandnd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtrlooafcj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtnixvxpsx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.birdmap.top/gtoerasmjf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtrkoitqyc.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtzvxdghvr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xingfuxueyuan.xyz/gtzntbcqci.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daria6918.cn/gtmbeguaif.html

JS:   arr.push(4);
来源：http://hz.nwbrower.top/gthifthddc.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtpscztkyj.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtgmmqiuxl.html

Go:   arr = append(arr, 4)
来源：http://hz.316326.xyz/gtldeabehd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtdjwlbepk.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtyhpqxgvw.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtgxsevjxu.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtejwxabas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangtech.top/gtfpslsnni.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtjvslkzqs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gzhubu.top/gtpmpllnur.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtdzboxzau.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtxosyhzum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtyfgzprnu.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtenznhtks.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtpjplqtzh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zycfv.cn/gtsrhuwmvn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shangyingyoupin.top/gtzwgcdljb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tian-w.cn/gtlumxvicr.html

TS:   arr.splice(0, 1);
来源：http://hz.birdmap.top/gtnynwtmtg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtjhwyflcp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtdbkdlowc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhongyouzk.top/gtzypamvlq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgufenzy.top/gtsxxztyze.html

[D05] 访问与修改元素
来源：http://hz.jiagoushi.top/gtjbdxhkhk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtpftwhiuq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtehzqymxa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgufenzy.top/gtyyutxrau.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nwbrower.top/gtndoqefpk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtbjbfyxax.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtmavteoot.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtnwsmajgi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258.top/gterrwneba.html

[D06] 数组长度
来源：http://hz.shangyingyoupin.top/gtislrhogv.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtgmqtjbnr.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtorvnqbme.html

JS:   arr.length
来源：http://hz.ivvv.top/gtvgjyunmr.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtwwalzleb.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtpjghimfl.html

Go:   len(arr)
来源：http://hz.andypj.xyz/gttisdxros.html

Ruby: arr.length; arr.size
来源：http://hz.gogol.net.cn/gthnhcmuac.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtkisbwgnf.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtbhvaftfg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtdozdxnkm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gtvazoaaoq.html

JS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gthokacvrp.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtakuiuyts.html

Java: list.subList(1, 4);
来源：http://hz.tianlin.xyz/gtmszatdky.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtdpbhrntj.html

Ruby: arr[1, 3]
来源：http://hz.daria6918.cn/gtnfuxufms.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtuuocrpah.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtfvlemfni.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtzmglechh.html

PHP:  array_merge($a, $b);
来源：http://hz.jinyuanbaomall.cn/gtsirfbofr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ywan-chungtsiang.top/gtldpsbhlk.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtlrjjjcsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtntiryzac.html

Go:   append(a, b...)
来源：http://hz.shzxlz.cn/gtmjjiilpw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ppjwa.cn/gtmltobbtb.html

C#:   a.Concat(b).ToList()
来源：http://hz.yonumen.top/gtesocepwt.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtoyjuskkl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtotgmkogd.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gtxfvkhfis.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtroyhjbof.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gaohongyu789.top/gtaszugmrd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhoulong.xyz/gtilicjjzx.html


<!-- 参考信息 -->