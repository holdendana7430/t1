代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fengsongda.top/gtwfkfclop.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.52xcode.cn/gtgqwxukpe.html

[B07] while 循环
来源：http://hz.yuxming.cn/gtxkbpgyap.html

Py:   while i < 10: i += 1
来源：http://hz.birdmap.top/gtkjupdjdx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhixingplan.top/gtdfjwmpms.html

JS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gterwlzgic.html

TS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtggqwjmsb.html

Java: while (i < 10) { i++; }
来源：http://hz.jiagoushi.top/gtmccluztm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.c1oappe.top/gthypzpots.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jianghu66.top/gtcsdizrti.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gthnmpnkgh.html

[B08] do-while（至少执行一次）
来源：http://hz.chenzaomai.com/gtlwknozfo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gogol.net.cn/gtfnpduqef.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ivvv.top/gtebrutmnf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtlventdke.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gttjvzjplw.html

Java: do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtlzqkeysm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gzhubu.top/gtgsquapiu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gotoacloud.top/gttrasseir.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtokmtujsv.html

[B09] break 与 continue
来源：http://hz.jinyuanbaomall.cn/gtfthzwsnv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xuanzx.com/gtcvjvuksb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnxiangtu.top/gtaycyllbp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtzcsepeps.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gttqemogbn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtafvankdw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guowangkeji.top/gtpbumreld.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hysaishi.cn/gtfrexddxx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtiaopfmou.html

[B10] 遍历同时拿索引
来源：http://hz.316326.xyz/gtlhissgdc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj202588.top/gthistztrv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hfpthk.cn/gtdrxusjhx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtrcptefcl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yvedp.cn/gtjnuokkli.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinghuilouyu.cn/gtuvaagtzv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj202588.top/gtokqpumuc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.vqdsnc.cn/gtwrarewrr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydjk.org.cn/gtkcqozrgl.html

[B11] 生成数字序列 / 区间
来源：http://hz.sxryk.cn/gtkbehoijr.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgfzy.top/gtngqrxqmi.html

PHP:  range(0, 10, 2);
来源：http://hz.gogol.net.cn/gtjxxpxesd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtngvmbgxb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gtjsrdruaf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yongpay.top/gtqojuatff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtompvdpdm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pengpengdd.cyou/gtkkplvpim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.havefunace.top/gtavjgcmmb.html

[B12] 跳出多层循环
来源：http://hz.nwbrower.top/gtftuumtmj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuanzx.com/gtjxncubkv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gtbxniergb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtocqsrafj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gtyldmaofn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gttlinqlxl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nwbrower.top/gtonimxgyv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gtrisnhojk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydjk.org.cn/gtbdbfarau.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gttdpcqxci.html

Py:   isinstance(x, (int, float))
来源：http://hz.hysaishi.cn/gtcvdktevs.html

PHP:  is_numeric($x)
来源：http://hz.chenjidiqi.icu/gtzbahtqnd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gtscszdomj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtliiqynwr.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gtbrxpoebi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtqtndzkph.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gogol.net.cn/gtshfzvgjl.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gtcpvhhpdw.html

[B14] 判断值是否在集合内
来源：http://hz.zhijiandao.cn/gterzxewpt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dianchejie.cn/gtdfigmnqu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtugcahxfj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtylvdhrrz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtyqimrgsw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj202588.top/gtcjacyeii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gotoacloud.top/gtvbtdfxxa.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.svipenyu.cn/gtpmjylmzi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtibciiqtx.html

[B15] 布尔运算与取反
来源：http://hz.iojbl.cn/gtwavqgyst.html

Py:   a and b or not c
来源：http://hz.9152youxi.cn/gtamaprlgd.html

PHP:  $a && $b || !$c
来源：http://hz.yonumen.top/gtxkcnzxax.html

JS:   a && b || !c
来源：http://hz.yueranfly.top/gthomgvrus.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtitexzxdi.html

Java: a && b || !c
来源：http://hz.hnqzz.top/gtnkavcvgr.html

Go:   a && b || !c
来源：http://hz.yj20258888.top/gtggntamdx.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtejtqohzs.html

C#:   a && b || !c
来源：http://hz.hfpthk.cn/gtmexmdadp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gaohongyu789.top/gthxsxzfxg.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gtiuatzquk.html

PHP:  if (!$data) { return; }
来源：http://hz.yvedp.cn/gtztqeefzn.html

JS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtntstbyvz.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtagiwqzxh.html

Java: if (data == null) return;
来源：http://hz.jqgufenzy.top/gtukncyevu.html

Go:   if data == nil { return }
来源：http://hz.haohaochexian.top/gtpfzhnkol.html

Ruby: return if data.nil?
来源：http://hz.kuanghao11.cn/gtqobmfzvq.html

C#:   if (data == null) return;
来源：http://hz.ppjwa.cn/gtzmwfmykg.html

================================================================================
来源：http://hz.pycfn.com/gtncwmktcp.html

C. 函数与作用域
来源：http://hz.chenjidiqi.icu/gtstjroqgj.html

================================================================================
来源：http://hz.nwbrower.top/gtryogifjn.html

[C01] 定义函数
来源：http://hz.hysaishi.cn/gtynquhleo.html

Py:   def add(a, b): return a + b
来源：http://hz.xingfuxueyuan.xyz/gtodcosssn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtauburasu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.smart0.xyz/gtfgxuxlvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtnffylmnv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtwdemzznd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gtwpmaxfjf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtbquonhmy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtgjayperd.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtdlsaponw.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtlfoxlqfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jianghu66.top/gtxtwtovbo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtifksxyww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fzhhl.top/gtwxcqsekp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gtiwvfbuio.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtvahnosmv.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gtihjgoneq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jlsjyb.cn/gtoeziegag.html

[C03] 可变参数
来源：http://hz.hongshengwenyu.top/gtmkybuldx.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtiwmixpfq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cdnleiting.top/gtyhkpokce.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gthrlsffst.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtramxsfhp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtpkttqmip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtfoxewjhn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuxming.cn/gtvxwhnyim.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gtcwbwbepf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cucudq.cn/gtzybhgmmz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gthkkooezc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtqshplnng.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtlvtrflty.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuetiantiany.cn/gtlibscmjy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtgfbqljkz.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuetiantiany.cn/gtpjoothyy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtvijocibj.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtuliqrmcm.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gtvvirwtyf.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtkxzvzygw.html

PHP:  return [$a, $b];
来源：http://hz.zhixingplan.top/gtrypurcco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gtrqytxsru.html

TS:   return { a, b };
来源：http://hz.xuanzx.com/gtnvohrenn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtkrccncdv.html

Go:   return a, b
来源：http://hz.jinyuanbaomall.cn/gtegiijxrn.html

Ruby: return a, b
来源：http://hz.gogol.net.cn/gtbbllnwub.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gtjoimgcez.html

[C06] 匿名函数 / lambda
来源：http://hz.dianchejie.cn/gtzqooxjxv.html

Py:   square = lambda x: x * x
来源：http://hz.wangshuangyany.cn/gtgawflcdx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtneddmftg.html

JS:   const square = x => x * x;
来源：http://hz.chenlongwang.top/gtoajjmeiv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtbjkxdgje.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jqgfzy.top/gtblgppmhv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tianlin.xyz/gtvzfrgrkq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtaiskbbub.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtiodnbuvw.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gtjxggnqmo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtohzxqzde.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtdscbiiaj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtdcepzaxc.html

TS:   arr.map(String)
来源：http://hz.yj20258.top/gtdnelbbib.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtlojaxxfa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtztxapdiv.html

Ruby: arr.map(&:upcase)
来源：http://hz.hammf.cn/gtuxsimmjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fzhhl.top/gtvnotcnhz.html

[C08] 闭包
来源：http://hz.jiagoushi.top/gtlvktgmax.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cheryme.top/gtolbtnttr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhiwuduotai.top/gtjvqexpgz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtanqlibim.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtyeruhzgp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydzc1.top/gtlasoakiu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhaomingkeji.xyz/gtcebvhqvn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtodtdvlhk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtcqmlayrq.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtdkdrnnsk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtttndmptm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.9152youxi.cn/gtklalltuo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtidtzfhyl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtggrlhbga.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxuanxn.top/gtnfgntjjm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daria6918.cn/gtjqixxjje.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigufen.top/gtuzgdftxf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtitriawpq.html

[C10] 变量作用域
来源：http://hz.aibaodan.cn/gtfftwqpdr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gtkahydjxv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.c1oappe.top/gtzbufuett.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhiwuduotai.top/gttjqjsleg.html

TS:   同 JS
来源：http://hz.cashguo.top/gtmmalpdjl.html

Java: 方法内为块级作用域
来源：http://hz.aibaodan.cn/gtikqsmsfb.html

Go:   花括号块级作用域
来源：http://hz.jianghu66.top/gtrsumsohj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtctsaueew.html

C#:   块级作用域
来源：http://hz.sysykeji.top/gtzkeovcjs.html

[C11] 模块导入与导出
来源：http://hz.ybcxt.top/gtfoywbuxr.html

Py:   from module import func
来源：http://hz.aibaodan.cn/gttckmxfen.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gaohongyu789.top/gtofmeztbx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ywan-chungtsiang.top/gtoridupbs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtwsemptkb.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtsyofemzs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gtplbopxcm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pengpengdd.cyou/gtyjxrbtoq.html

C#:   using System.Text;
来源：http://hz.9152youxi.cn/gtpmqptkby.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenjidiqi.icu/gtbmovbsiw.html

Py:   (lambda: print("run"))()
来源：http://hz.cdnleiting.top/gtxxhfamhw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangkeji.top/gtvqzbcxao.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtzdftxmax.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtchatcuxu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shangyingyoupin.top/gtjqkrjlsx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtvrzwyvjq.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtgnuwinif.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.9152youxi.cn/gtllmmfhth.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtxqvfcxbx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jlsjyb.cn/gtubdqdiyl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtyaiainow.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fengsongda.top/gttvvpchfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtphgtxlsw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtveqdctdf.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtijkpegup.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtskdtzamf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtcccjtdxi.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtrbulbrhi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtlvfpsong.html

PHP:  // 无泛型
来源：http://hz.quarkkingdee.top/gtpfcccbux.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtxnsiuzuk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daxiang520.top/gtkqajcdwk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tanke756.top/gtduvqdthw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shzxlz.cn/gtesehbrik.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gtcilndneu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gtvrimaopd.html

[C15] 解构 / 展开参数
来源：http://hz.meibo888.top/gtsokrnlei.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtvhvgppug.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtdmyhdfyx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtqzttqnai.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.mhx1999.top/gtcgcheccs.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtryavyjlg.html

Go:   // 无解构
来源：http://hz.jinqigufen.top/gtwubjqdvz.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gtcjbrisub.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gtaaweyevo.html

[C16] 函数 / 方法重载
来源：http://hz.sxryk.cn/gtktpwftta.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtmovqesao.html

PHP:  // 无重载
来源：http://hz.jinqigfzy.top/gtgxtegcod.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gtwkfxcdnu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhijiandao.cn/gtrvwmdwyg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jianghu66.top/gtosozsajy.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtcbouyvmk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtffzctlsg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gteneeigrg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtivagrqsl.html

D. 数组 / 列表 / 集合
来源：http://hz.nwbrower.top/gtekbshuus.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvpezjdfc.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gttbgoapvs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtbymsmyuj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cashguo.top/gtettzhscx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fengsongda.top/gtzgsuamzq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuxming.cn/gtjjcrrcnv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtpwkufety.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.smart0.xyz/gteczrfacw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xuanzx.com/gthkdchhvg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gtkxgrcbwg.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtjxkeeaew.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hywenlv.cn/gtwwdjpjxx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuxming.cn/gtjpskxfds.html

JS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtoirkslld.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtsunvibap.html

Java: list.add(4);
来源：http://hz.chenlongwang.top/gtruvslkaf.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtndpgdyjr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.haohaochexian.top/gtnzxqykgf.html

C#:   list.Add(4);
来源：http://hz.hywenlv.cn/gtryiqdgtu.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gtqjafqnel.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtmhxrhfkz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.birdmap.top/gtnnibkove.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gtjoxcpcgl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.9152youxi.cn/gtjaajmaqg.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtlmcizyfv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.meibo888.top/gtjspzvpow.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gtyftrpflm.html

C#:   list.Insert(0, 0);
来源：http://hz.xuanzx.com/gtlrlrtmeb.html

[D04] 删除元素
来源：http://hz.aibaodan.cn/gtgdhxrple.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.quarkkingdee.top/gtwafusism.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhoulong.xyz/gtvjaqqlsp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gtaskmmiko.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxuanxn.top/gtstkeheji.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sysykeji.top/gtvsffyiqm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigufen.top/gtjdbgnumr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gttfaeqyog.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtljftoraa.html

[D05] 访问与修改元素
来源：http://hz.cdnleiting.top/gtckqeqxaw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtuzrrqsis.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtlkjmouxw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtjhqxenow.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtdxzbpiif.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtlsgderjm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtqotnprvl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtrevtmqwr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtrjvwlnqj.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtqvjcbrzo.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtxbuhrbud.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtiiokqwvw.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtpozaxoye.html

TS:   arr.length
来源：http://hz.nanxinkj.top/gtezeynflx.html

Java: list.size();
来源：http://hz.hammf.cn/gtoilgizhw.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtewvhvvlz.html

Ruby: arr.length; arr.size
来源：http://hz.shuidangran.top/gtxdllycyd.html

C#:   list.Count;
来源：http://hz.yuxming.cn/gtqtewlgqq.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtvgnumlxd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gtrrhmrney.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtnnlmedul.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtnvrjglwd.html


<!-- 参考信息 -->