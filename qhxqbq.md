代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtqboifavj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtbrgvyuqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.snrcjt.cn/gtuglaoqcb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zdqjudy.top/gttksqkwyk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gthywjtmii.html

[B10] 遍历同时拿索引
来源：http://hz.chenjidiqi.icu/gtooijycim.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jianghu66.top/gtbsfavkzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ydjk.org.cn/gtjkykopos.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtfjmqtxhb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gtafxfjgqh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gtijapycrd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tanke756.top/gtqtbueixu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhijiandao.cn/gtiuzsfoza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.316326.xyz/gtodkcstmg.html

[B11] 生成数字序列 / 区间
来源：http://hz.feifeiyinyue.top/gtrlywjhsn.html

Py:   list(range(0, 10, 2))
来源：http://hz.fzhhl.top/gtulrjmwun.html

PHP:  range(0, 10, 2);
来源：http://hz.yj202588.top/gthjhlzomc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtxsjhhbey.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtpvmpnpuj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj20258.top/gtsnvvopkl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinyuanbaomall.cn/gtdokutuur.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtqsqyumrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jianghu66.top/gtgiyvuren.html

[B12] 跳出多层循环
来源：http://hz.zhiwuduotai.top/gttcbruisy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ybcxt.top/gtgvizkzcf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cqqwz.cn/gtaikvfkbl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtwmrancgf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtlnmpsyyv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtivoxeulp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ehwqpu.com/gtkdtwaodu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yongpay.top/gtbxmwdslk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cucudq.cn/gtpdzpleco.html

[B13] 判断是否为数字
来源：http://hz.yuxming.cn/gthfcvgzkm.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtwdplarue.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtlmreofao.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtcdjgpizy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtbgjyfycu.html

Java: x instanceof Number
来源：http://hz.andypj.xyz/gtqdheupya.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yongpay.top/gtuhvrhdht.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtuksbkbbs.html

C#:   x is int or double or decimal
来源：http://hz.0kj1m.cn/gtenuaswra.html

[B14] 判断值是否在集合内
来源：http://hz.xylfe.cn/gtqsxiojsc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuanzhike.top/gtxscanknb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.0kj1m.cn/gtnigxjldu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtogfstyic.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtruglztaq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj20258888.top/gtnsmgnrri.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ehwqpu.com/gtldhzulny.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gtsjtmluwf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangshuangyany.cn/gtuiopcmkt.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtnaobbtlu.html

Py:   a and b or not c
来源：http://hz.xinyue.icu/gtnnezazym.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gtzdaarjiv.html

JS:   a && b || !c
来源：http://hz.yj202588.top/gtvljewswh.html

TS:   a && b || !c
来源：http://hz.yj20258888.top/gtjbpnogzm.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtqxvynzqi.html

Go:   a && b || !c
来源：http://hz.pengpengdd.cyou/gthyarbygk.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtynyijusp.html

C#:   a && b || !c
来源：http://hz.nanxuanxn.top/gtfmohmsxe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtbeiqwxsg.html

Py:   if not data: return
来源：http://hz.yonumen.top/gtckmnrpch.html

PHP:  if (!$data) { return; }
来源：http://hz.gzhubu.top/gttbvxskmv.html

JS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtahiamewn.html

TS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtxalzrwpd.html

Java: if (data == null) return;
来源：http://hz.tanke756.top/gthglzixun.html

Go:   if data == nil { return }
来源：http://hz.hnqzz.top/gtgcygyzaw.html

Ruby: return if data.nil?
来源：http://hz.yuxming.cn/gtuxrryccz.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gtphgzbune.html

================================================================================
来源：http://hz.gaohongyu789.top/gtplqalnie.html

C. 函数与作用域
来源：http://hz.birdmap.top/gtfmvponaj.html

================================================================================
来源：http://hz.hfpthk.cn/gtyiqpoera.html

[C01] 定义函数
来源：http://hz.birdmap.top/gtvdcbjuld.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtlyeseymu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gttiizdsqx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtxtcadxty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtlwnsjqjx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtyfvuzgcb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yueranfly.top/gtopcyfskp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ivvv.top/gtesljknan.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtenkcxqkf.html

[C02] 默认参数
来源：http://hz.havefunace.top/gtgukelaqg.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtlgmmossz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangdashe.top/gtdbamoint.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258888.top/gtrmmfxjan.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gteiyncmbd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtfyrxhlgx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sxryk.cn/gtuwpdwmgs.html

Ruby: def greet(name = "World") = name
来源：http://hz.cdnleiting.top/gttwkenlxa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj202588.top/gtinzspmsd.html

[C03] 可变参数
来源：http://hz.svipenyu.cn/gtmexgmvop.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtskxoakvs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtcidohcxd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gttwipimqx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtdmfuvsne.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtylfcbptm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gotoacloud.top/gtchuibqpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.havefunace.top/gtwgtzsaum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtpyipsqwb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtnzagjhcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jianghu66.top/gtovbzcqqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtjyrhsags.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtupprdogy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.andypj.xyz/gtqymrwcxo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gteweitqtq.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangdashe.top/gtjdwmyqte.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtgrvnbrlu.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtcrtwjumf.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtlavmzttu.html

Py:   return a, b
来源：http://hz.guowangkeji.top/gtiphfctpz.html

PHP:  return [$a, $b];
来源：http://hz.andypj.xyz/gtpuhmmxvv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cqqwz.cn/gtszqoczod.html

TS:   return { a, b };
来源：http://hz.daxiang520.top/gtmclvbtgs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xylfe.cn/gtrhgzwuts.html

Go:   return a, b
来源：http://hz.pycfn.com/gtdlhxvusx.html

Ruby: return a, b
来源：http://hz.feifeiyinyue.top/gtwclhfccb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.bjfxy.top/gtmetceant.html

[C06] 匿名函数 / lambda
来源：http://hz.meibo888.top/gtveyawxgr.html

Py:   square = lambda x: x * x
来源：http://hz.pycfn.com/gtmcmsupdf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtdwyqgivu.html

JS:   const square = x => x * x;
来源：http://hz.haohaochexian.top/gtvjjnjzxp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gaohongyu789.top/gtmcpohpod.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gtiasffoyu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hfpthk.cn/gtihbhkhow.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ehwqpu.com/gtetyubucq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigfzy.top/gtnrqlkndu.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigufen.top/gtlycxjmox.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtbmyshhmr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtuvjasoht.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtaucosqjn.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtipydmrqh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xziqi.cn/gtxfdzlpml.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtahhjshio.html

Ruby: arr.map(&:upcase)
来源：http://hz.cucudq.cn/gtjzzuaclj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yonumen.top/gtdqwqenmq.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gtlvpyaoyd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtnwgpkcvv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gtgmedajww.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gthjrxbsxy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtexdohrjb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gtozlwjkds.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aibaodan.cn/gtbeqbgnrk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtzlhteuyp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtrkeksweo.html

[C09] 递归
来源：http://hz.ydjk.org.cn/gtzxyylgfm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtqdtspwlj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtpyhftszh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtgywspxrs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cqqwz.cn/gtpdfacpah.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtewygomoi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtardjyonj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.meibo888.top/gtbpdfjrfg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtgpmsmpfb.html

[C10] 变量作用域
来源：http://hz.yongpay.top/gtvqrkxyjp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dianchejie.cn/gthvtzuiyf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtsvguscik.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtmcclmsmh.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtzhxelbbj.html

Java: 方法内为块级作用域
来源：http://hz.tanke756.top/gtkwgxideb.html

Go:   花括号块级作用域
来源：http://hz.zycfv.cn/gtvmqmcyma.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtjozbvrgc.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtawwnzbzq.html

[C11] 模块导入与导出
来源：http://hz.gogol.net.cn/gtnaejqyxz.html

Py:   from module import func
来源：http://hz.ivvv.top/gtniozucpb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gthnexojbv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtcznrsxun.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtqmvpxfik.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtmaobpznf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xylfe.cn/gtoakhloph.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xziqi.cn/gtdmwaspex.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gtezgcqzgb.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgufenzy.top/gtpayvochx.html

Py:   (lambda: print("run"))()
来源：http://hz.yj202588.top/gtndlslqfr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yongpay.top/gtqeefkmyd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtmssllnfr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtzehlguzy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtwnpmkfbv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtsqbcstmm.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gtdnvhtqcj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtqigrprlu.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtrcsbutkj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gtbktmkzwx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtfzwozqfm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fengsongda.top/gtflirkfjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtigrzcfqs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gteyjunkul.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtuxhkputc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtykukzlyi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtinnhyyfq.html

[C14] 泛型函数
来源：http://hz.feifeiyinyue.top/gtnkqhazfr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtbrlnkpmw.html

PHP:  // 无泛型
来源：http://hz.tianlin.xyz/gtvzpiyfxn.html

JS:   // 无泛型
来源：http://hz.fengsongda.top/gtwryrjnla.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtuxxnsrdh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yueranfly.top/gtihlajuxr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtodfpfjyh.html

Ruby: # 无泛型
来源：http://hz.redwolf501.top/gtaweeomey.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtvfjmmjik.html

[C15] 解构 / 展开参数
来源：http://hz.bjfxy.top/gtnofxbzne.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yonumen.top/gtbsojdirh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtdhwjdmjk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtwctkxzte.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zycfv.cn/gtkyonlfat.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtcwpumlbe.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtsqoglwpr.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtngyyxfnd.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtyskgxvee.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtowiodnck.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gthzuzxmef.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtmtfgvxwu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtycgmwyrf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yongpay.top/gtjlyrlvpk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xylfe.cn/gtnnkdhynk.html

Go:   // 无重载：用不同函数名
来源：http://hz.52xcode.cn/gtectybqki.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtldxbsimg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.bjfxy.top/gtziycexdb.html

================================================================================
来源：http://hz.jinqigufen.top/gtwarnwnsf.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gtpcyrtdkt.html

================================================================================
来源：http://hz.snrcjt.cn/gtszttomid.html

[D01] 创建数组 / 列表
来源：http://hz.shangyingyoupin.top/gtdxtypayc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tian-w.cn/gtjmcaocmx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yangfankeji.com/gtidsmplce.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.fengsongda.top/gtiexyfcra.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangtech.top/gtpkpjgowz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jianghu66.top/gtboiajzlj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtwjpdoluz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cucudq.cn/gtrlhivqoh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangtech.top/gtmuqpgkgg.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtkewbiynv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gtyenuoebf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.9152youxi.cn/gthhfusjzl.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtdmtmexol.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtsclbpurr.html

Java: list.add(4);
来源：http://hz.zhijiandao.cn/gtdujraosp.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtiqhepvvf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gttexcqfaq.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtoflhtdup.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtyjuurbou.html

Py:   arr.insert(0, 0)
来源：http://hz.svipenyu.cn/gttcnfrejq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sysykeji.top/gtttogxcyy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ivvv.top/gtyouxnhmy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sysykeji.top/gtercpcbws.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtvvmcyruj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtwfpknoic.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yongpay.top/gtoisqvgey.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtcdowqajw.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtwwpcwaao.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtpxcbwuyi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtqaleysna.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.svipenyu.cn/gtxirtimnz.html

TS:   arr.splice(0, 1);
来源：http://hz.yvedp.cn/gtkhzposii.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtxqpmdett.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gtxsljmarg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtklgthdth.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yanxiufei.cn/gtfkurdrwk.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gtqjwguxqy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtbfyuisop.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gogol.net.cn/gtmcoeqvlu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtxzhgssgh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtywlvhwxh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gtlrvvpskd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtxfmwzpbp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtgtyphwbg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daria6918.cn/gtlsjyrdnf.html

[D06] 数组长度
来源：http://hz.0kj1m.cn/gtsxsaqgld.html

Py:   len(arr)
来源：http://hz.dashuyun.cn/gtrjwzjjpc.html

PHP:  count($arr);
来源：http://hz.xinyue.icu/gtdwcodgkg.html

JS:   arr.length
来源：http://hz.yj20258.top/gtclxemmcj.html

TS:   arr.length
来源：http://hz.fzhhl.top/gthhrplqvv.html

Java: list.size();
来源：http://hz.yangfankeji.com/gttmxlndif.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtxocfrazn.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gtikxukzuv.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gtodcixjhr.html

[D07] 切片 / 取子数组
来源：http://hz.ywan-chungtsiang.top/gtapsqpkde.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gtbijjngxg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangshuangyany.cn/gtszrwcmbp.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtpfhcihnm.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtjynpefkh.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtwehzvbyt.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtltjsetyi.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtgdlajdah.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtlblnpyip.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtuksakeqe.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtizyoqllm.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gteuaegoug.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtnhqekizm.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtqcndhvip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtvzdngxtc.html

Go:   append(a, b...)
来源：http://hz.zhiwuduotai.top/gttouljxqi.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhiwuduotai.top/gtnjskwapd.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtgdixtjvv.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtmdteiozz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtqduilndb.html

PHP:  sort($arr);
来源：http://hz.xuetiantiany.cn/gttukefgro.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.svipenyu.cn/gtryppakpb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtozrlpetp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtoxmphubw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtmtzyqwau.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gteusdiice.html

C#:   list.Sort();
来源：http://hz.ehwqpu.com/gtbtoknkxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gtpjzhvkqk.html


<!-- 参考信息 -->