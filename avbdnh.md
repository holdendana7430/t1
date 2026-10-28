代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.havefunace.top/gtsqbizzoi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtqommozer.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.guannengcc.top/gtqhadwabg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.meibo888.top/gtjqzslzdw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sxryk.cn/gtibjlegpn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.smart0.xyz/gtzsdewajt.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtpkdiujut.html

Py:   list(range(0, 10, 2))
来源：http://hz.fengsongda.top/gtvoozxndm.html

PHP:  range(0, 10, 2);
来源：http://hz.zhaomingkeji.xyz/gtntwibite.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zdqjudy.top/gthpqubyxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtpbxqnbhy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yongpay.top/gtpvubrsvd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtxmvmjtfr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cdnleiting.top/gtpwvpbmmk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.bjfxy.top/gtxgcgywwr.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtmoygynbr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gzhubu.top/gtyjlmvpxa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gtqhvrybca.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtcwfgvvnd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtajmbddou.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtvuoxtrdg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtvnkicven.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.svipenyu.cn/gttcgktizl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aibaodan.cn/gtsittshyz.html

[B13] 判断是否为数字
来源：http://hz.nwbrower.top/gtywcvejgm.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gtonlkghmy.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtnwosgkun.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtcubmjnfh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtinzvcsnc.html

Java: x instanceof Number
来源：http://hz.sysykeji.top/gtmxuczcji.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zycfv.cn/gtsyfpcwpy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhoulong.xyz/gtxxxmzbvg.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtkwakkpqo.html

[B14] 判断值是否在集合内
来源：http://hz.snrcjt.cn/gtbuvsghey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.smart0.xyz/gtdnqtfcfn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.52xcode.cn/gtznypjnmf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtdxzyhitn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gttfytheec.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.0kj1m.cn/gtbnxvfsmi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxuanxn.top/gtrzqxbsag.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shuidangran.top/gtektsunsw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.snrcjt.cn/gtopsoorvg.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtqvacbzea.html

Py:   a and b or not c
来源：http://hz.gaohongyu789.top/gtjgfbbqom.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtggopmcct.html

JS:   a && b || !c
来源：http://hz.jyoumei.cn/gtjgoupqgu.html

TS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtnkmgpzbi.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtgrkjqicn.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gtmdcvgxrb.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtpeymrzwj.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtoevafjxv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sysykeji.top/gtesohgoyn.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gtzqqpeifj.html

PHP:  if (!$data) { return; }
来源：http://hz.ivvv.top/gthvsrtrmd.html

JS:   if (!data) return;
来源：http://hz.ydzc1.top/gtavnevppc.html

TS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtbfozokgu.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gtvqmuxunt.html

Go:   if data == nil { return }
来源：http://hz.ydjk.org.cn/gtwtqumrng.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtcrkkajns.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtkndpvmng.html

================================================================================
来源：http://hz.ydzc1.top/gtktppfvmw.html

C. 函数与作用域
来源：http://hz.ppjwa.cn/gtlqarmvdq.html

================================================================================
来源：http://hz.yvedp.cn/gttheieuqm.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtsysrnjtg.html

Py:   def add(a, b): return a + b
来源：http://hz.hysaishi.cn/gtvwckieyt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtahmmgkbo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtjdbvylgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtusovcfyn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtfxljcmhc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuetiantiany.cn/gtidwqhjnb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtbnqhaytk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtjffgpgho.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtfzpweqya.html

Py:   def greet(name="World"): return name
来源：http://hz.jianghu66.top/gtgtenvwpt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shangyingyoupin.top/gtjznyxkjt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zdqjudy.top/gtjsfqsppj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zycfv.cn/gttzlslhve.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtntbbaipe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj20258.top/gtnaialvnq.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxinkj.top/gtpzvlgamr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtneqvighy.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gtuulsslcd.html

Py:   def total(*args): return sum(args)
来源：http://hz.pengpengdd.cyou/gtuwmdlaqt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtzgctunzp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtwjtnynxe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gththguzhx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tian-w.cn/gtbjxmtxuc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtvxvciyug.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgfzy.top/gttkwnhedf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtxsysrsom.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtlnwqfxgq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtgtaokstk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuxming.cn/gtlpefzdki.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gthxpuhqtw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yangfankeji.com/gtkiluzfnn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hongshengwenyu.top/gttechrpai.html

Go:   // 无：用配置结构体参数
来源：http://hz.gaohongyu789.top/gtupibeayt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtdmmswrfq.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtecfgsxgo.html

[C05] 返回多个值
来源：http://hz.jlsjyb.cn/gtweforxtu.html

Py:   return a, b
来源：http://hz.sweek.top/gtftzqgkve.html

PHP:  return [$a, $b];
来源：http://hz.yuanzhike.top/gtmfbyumvp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtkllkzunz.html

TS:   return { a, b };
来源：http://hz.redwolf501.top/gtycykgyjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hysaishi.cn/gtweuasxiq.html

Go:   return a, b
来源：http://hz.daxiang520.top/gtlvoerfrg.html

Ruby: return a, b
来源：http://hz.jinghuilouyu.cn/gtoljtcxwh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.fengsongda.top/gtcgicdect.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgfzy.top/gthlhknibj.html

Py:   square = lambda x: x * x
来源：http://hz.cucudq.cn/gtitnesjao.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtpckydjjg.html

JS:   const square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtvdfqfnmh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj202588.top/gtqpkxrcog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gtguuniqhx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtnwalseee.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtxwskbsct.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxinkj.top/gtknzxqdvp.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gtawayhbtz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gtnwwpgydj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daria6918.cn/gtthykkgrd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigfzy.top/gtfsqylzea.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtbonbsyvd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj20258888.top/gtksploxer.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.9152youxi.cn/gtotlbygng.html

Ruby: arr.map(&:upcase)
来源：http://hz.cheryme.top/gtmqugdmzb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangdashe.top/gtngzvdmag.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtkxlnkjgu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.birdmap.top/gtpbsnhlie.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhaomingkeji.xyz/gtaihjdndc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtbjbmsvye.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtbdzlkqbt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pengpengdd.cyou/gtcixbcvnl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guannengcc.top/gtffbkramv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.snrcjt.cn/gtnniiathp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtyurkrwwo.html

[C09] 递归
来源：http://hz.dashuyun.cn/gtnbovmpti.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtrfdgiwtu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gtdxbskiyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtqzkqynvk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtuvpdqeun.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yonumen.top/gtnmnhpegm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtpzdsmrup.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtgttoahqo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gtwrwnvhvv.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtlhwmgdxg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gzhubu.top/gtovqgjmaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cheryme.top/gtcdzaztty.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.feifeiyinyue.top/gtjyyzkmxr.html

TS:   同 JS
来源：http://hz.svipenyu.cn/gtkkqmqiob.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtjciypaks.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtdhnshvjn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gtqnwmjymt.html

C#:   块级作用域
来源：http://hz.xuetiantiany.cn/gtaoaiypai.html

[C11] 模块导入与导出
来源：http://hz.jianghu66.top/gtshjidrfs.html

Py:   from module import func
来源：http://hz.jqgufenzy.top/gtoqkgncwz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtxjvftubl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtlnuksxbb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtsexejryc.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtsmesrjjz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtnmhlyrjl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gtkukiexgr.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gttfujzxsk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtainudjtc.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigufen.top/gtiahtzsnp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gttzwudjnz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtkxsioinj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtvysnyqte.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yuxming.cn/gtfnohdsgy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangshuangyany.cn/gtgefaqrxi.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhoulong.xyz/gtoyyhsgux.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.bjfxy.top/gtgrzyqgck.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtnvtxgovd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ywan-chungtsiang.top/gtvplwvpbr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtjefljbpj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigufen.top/gtljkpcrmd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtbizidwfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtjmhizetq.html

Go:   func add(a, b int) int
来源：http://hz.yanxiufei.cn/gtmyuclwdo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gthrzmvbfu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtobhxjiok.html

[C14] 泛型函数
来源：http://hz.nwbrower.top/gtdshszelm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gtdjenxlsp.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtrzmkeyht.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtqklijorg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtzblcawxa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hysaishi.cn/gthbvhjzfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhijiandao.cn/gtpptpqyds.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtuuvofaps.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jianghu66.top/gtfrxjylpt.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gtuaabzcyz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jianghu66.top/gtiqduunnn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtkprgblhq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtcopjhmyk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtzpfkmcsz.html

Java: // 无解构
来源：http://hz.ydjk.org.cn/gtecmorxas.html

Go:   // 无解构
来源：http://hz.pengpengdd.cyou/gtcpgryneu.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtkqueoksf.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtfzvalubc.html

[C16] 函数 / 方法重载
来源：http://hz.jiagoushi.top/gtftowalag.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gtpizzesfv.html

PHP:  // 无重载
来源：http://hz.cqqwz.cn/gtdlswbatr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gtrmbhjlrz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtdeozsmcc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtzohyxkpt.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuetiantiany.cn/gtacvsstdj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.feifeiyinyue.top/gturhzisla.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtlpxepwyc.html

================================================================================
来源：http://hz.xuanzx.com/gthmqcztrh.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtjqlyeasl.html

================================================================================
来源：http://hz.cheryme.top/gtcfixrabe.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtrgioppmu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hongshengwenyu.top/gtrihasnpv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtlsanbyuu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnxiangtu.top/gtjrsjyoar.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtbsrjujga.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigufen.top/gtmzkyxciq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtclsswfvl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtpcouznbj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtyfrjfqgf.html

[D02] 追加元素到末尾
来源：http://hz.shanyushiyangkeji.top/gtrrwxiblg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gtyrufzbfo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtjkrvivly.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtmwldrzvb.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtpokxdrdq.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtygkapmbu.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtidodypfg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gttbaqifyg.html

C#:   list.Add(4);
来源：http://hz.yongpay.top/gtjnpdjqlp.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtcgaouvwr.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtqchgqrkf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tanke756.top/gtyejqfbwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtpxvhntvj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ivvv.top/gtbxojtahw.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtjjasdvvw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guowangkeji.top/gtxdmqhatr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhengqikj.top/gtcxvlgixa.html

C#:   list.Insert(0, 0);
来源：http://hz.cdnleiting.top/gtvrqkavyk.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gtkhngitey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.haohaochexian.top/gtbaixepdp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtjhbltykl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dashuyun.cn/gtxeyybehu.html

TS:   arr.splice(0, 1);
来源：http://hz.52xcode.cn/gtqfprevet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cheryme.top/gtowqpfytt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtcjiewahu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtwledjgye.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtwryaiwqp.html

[D05] 访问与修改元素
来源：http://hz.0kj1m.cn/gtyqnrhkxd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtncsjztsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gtmdctdodm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtrgaaddrp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dianchejie.cn/gtkttpqceb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ywan-chungtsiang.top/gtskkoiwbt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtrrneovza.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtuegzzvvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtlsdfypzt.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtfkejnfpl.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtvqosxmsy.html

PHP:  count($arr);
来源：http://hz.jqgfzy.top/gtrhpbvauk.html

JS:   arr.length
来源：http://hz.nanxuanxn.top/gtzdsvhjqe.html

TS:   arr.length
来源：http://hz.yvedp.cn/gtpnxbhtnp.html

Java: list.size();
来源：http://hz.wangdashe.top/gtpxsmgqxp.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtmpwermkm.html

Ruby: arr.length; arr.size
来源：http://hz.feifeiyinyue.top/gtmjojwzce.html

C#:   list.Count;
来源：http://hz.shuidangran.top/gtulaxaevq.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtcnnuzbqz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gtnsicixtd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtrvwozaoe.html

JS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtaojmomji.html

TS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtsegojsrx.html

Java: list.subList(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtucukhjyb.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtgzcshpqn.html

Ruby: arr[1, 3]
来源：http://hz.ppjwa.cn/gtmaemnswq.html

C#:   list.GetRange(1, 3);
来源：http://hz.havefunace.top/gtzbxgzjer.html

[D08] 合并两个数组
来源：http://hz.yanxiufei.cn/gteotzmnle.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gtrveaejht.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gthmafngtp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nwbrower.top/gtdibjhocq.html

TS:   [...a, ...b];
来源：http://hz.yuanzhike.top/gtcygldxlj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtkemokcha.html

Go:   append(a, b...)
来源：http://hz.yuanzhike.top/gtddbhhrgd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258.top/gtjzinosyb.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtgehpmfjl.html

[D09] 排序（升序）
来源：http://hz.ydzc1.top/gtswcilgsq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtxivijfbz.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtcywefzem.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtxqyrtluk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtksoprgoa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xingfuxueyuan.xyz/gtiiopasji.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtuzuxnflo.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtonocvcef.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtufdjauug.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jlsjyb.cn/gtulzzpsuj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnxiangtu.top/gtexvgjwrj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtcxufoytk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtylrixmti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtonaijtxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtkxnysadt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtadfhmfcv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtmakbytxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtscoimkdd.html


<!-- 参考信息 -->