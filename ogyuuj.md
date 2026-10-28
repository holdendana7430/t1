代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtrdktjhia.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.svipenyu.cn/gtllfloriw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhaomingkeji.xyz/gtwrrdvtrt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jianghu66.top/gtgojrklkp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhiwuduotai.top/gttnzifuel.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cqqwz.cn/gtrqrnavmx.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtnynvafie.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gtunibqvpg.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtoxawgukm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ehwqpu.com/gtkbffcrkl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtxgaxztoo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtbzmhdclf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.smart0.xyz/gthmeebofm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnqzz.top/gtanhaygns.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gogol.net.cn/gtujysrawg.html

[B12] 跳出多层循环
来源：http://hz.dianchejie.cn/gtenmmtqsr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.meibo888.top/gtmqexsoft.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ydzc1.top/gtydbprqhc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtllkgxvmn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtzwepdskl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtmtgwcjvf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtcwejlykn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shangyingyoupin.top/gtchvhujnd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gaohongyu789.top/gthwhtqhij.html

[B13] 判断是否为数字
来源：http://hz.0kj1m.cn/gtawklgkvh.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydzc1.top/gtfntcsqds.html

PHP:  is_numeric($x)
来源：http://hz.guowangkeji.top/gtdetyodlz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ywan-chungtsiang.top/gtyjccenyd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtwiaynlqi.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtmiliuoik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtiftvztwn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gtszfrhimt.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gtwcoacdhp.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtqnhordjn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gtwcjoohdd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ybcxt.top/gtaykewygm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gtyhyaimqg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtycfqceln.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sxryk.cn/gtbnwbkskp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenlongwang.top/gtiykxvhgd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zdqjudy.top/gtidtxnazs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cheryme.top/gtgeugrvem.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtkugkuqbb.html

Py:   a and b or not c
来源：http://hz.aizwys.cn/gtekjjknbp.html

PHP:  $a && $b || !$c
来源：http://hz.ybcxt.top/gtkptaqfsr.html

JS:   a && b || !c
来源：http://hz.xuanzx.com/gtoipnehin.html

TS:   a && b || !c
来源：http://hz.hywenlv.cn/gtjvhytjde.html

Java: a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtqeevabdd.html

Go:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtfrgepqgv.html

Ruby: a && b || !c
来源：http://hz.hnqzz.top/gtwhafigvc.html

C#:   a && b || !c
来源：http://hz.jianghu66.top/gtjghtffzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtpyrxignv.html

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gtclntpngh.html

PHP:  if (!$data) { return; }
来源：http://hz.iojbl.cn/gtqienueam.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtvictxpfg.html

TS:   if (!data) return;
来源：http://hz.jianghu66.top/gttdphbxst.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtwmjdihmd.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtqinszurx.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtcdfyezau.html

C#:   if (data == null) return;
来源：http://hz.hfpthk.cn/gttgmarevz.html

================================================================================
来源：http://hz.yvedp.cn/gtpidmbnpt.html

C. 函数与作用域
来源：http://hz.havefunace.top/gtxuglrrnq.html

================================================================================
来源：http://hz.cdnleiting.top/gtgteddxbw.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtimtpxhgx.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtfdrggjxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtmsnsecjv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sweek.top/gtiuyeadft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtsvvkgnsx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtukpghycr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtrlomjzst.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guowangkeji.top/gtnzxqdpvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtofgtaici.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtkgtwjzzy.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gtqmxdhnjq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtvkvbiauf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhixingplan.top/gtygqcpajr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jyoumei.cn/gtzmxdyoqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenjidiqi.icu/gtfbbyenlr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jyoumei.cn/gthvjvybqc.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtqoskswxk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtdytpmxad.html

[C03] 可变参数
来源：http://hz.yanxiufei.cn/gtziojqdid.html

Py:   def total(*args): return sum(args)
来源：http://hz.daria6918.cn/gtsxoifwhy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhoulong.xyz/gtkmymwddy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtojmvuoib.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yongpay.top/gtzxpivyly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhongyouzk.top/gtzqhhwutf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gteieusoau.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jqgfzy.top/gtkfbtlnhn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ybcxt.top/gtsatgjrva.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtkvgksceh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pycfn.com/gthhzjrxwx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.redwolf501.top/gtfzrxqhjl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yvedp.cn/gtshwdlwkl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtvwtbtimp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ivvv.top/gtezrtehso.html

Go:   // 无：用配置结构体参数
来源：http://hz.redwolf501.top/gtzkrxvspm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtawmzjlkt.html

C#:   f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtxsxvstgn.html

[C05] 返回多个值
来源：http://hz.fzhhl.top/gtaplkzwaz.html

Py:   return a, b
来源：http://hz.jinyuanbaomall.cn/gtuiwbsczc.html

PHP:  return [$a, $b];
来源：http://hz.wangdashe.top/gtfsbihrmw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtvwvcpkyp.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtgemhwxnx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gttrmcqxtn.html

Go:   return a, b
来源：http://hz.tian-w.cn/gtklmgzalm.html

Ruby: return a, b
来源：http://hz.mhx1999.top/gtfonordpl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hfpthk.cn/gtfzmzdmds.html

[C06] 匿名函数 / lambda
来源：http://hz.dianchejie.cn/gthdestqzk.html

Py:   square = lambda x: x * x
来源：http://hz.cheryme.top/gtdzwiokrx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gtncvyzxva.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gtqorgjblj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yvedp.cn/gtpvgwhpob.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gtfsercyaz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtlfjpdrsb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tanke756.top/gtevpqmynq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtkseeaqug.html

[C07] 把函数作为参数传入
来源：http://hz.cdnleiting.top/gtcflfmwkl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gtechuejml.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gteziwblnm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtwenlymgr.html

TS:   arr.map(String)
来源：http://hz.shangyingyoupin.top/gtylrihbra.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shzxlz.cn/gtvztkxyop.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtvfpftiik.html

Ruby: arr.map(&:upcase)
来源：http://hz.yongpay.top/gtkqnbdhjs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.c1oappe.top/gtbphekfpr.html

[C08] 闭包
来源：http://hz.cdnleiting.top/gthfnllqku.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cqqwz.cn/gtpkqnfmit.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtaiqvjfik.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtmrydjvrw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtachkkmdb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xziqi.cn/gtdaalonsd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigfzy.top/gtnfiehjwi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtunwdkraa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtlfhtzrjp.html

[C09] 递归
来源：http://hz.shuidangran.top/gtirgqterh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtnxdnnayn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gtfwhjcpae.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtvfqlhrnz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtmeaotetn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtcsfywrad.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cashguo.top/gtzkhctrvu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jiagoushi.top/gthgbunqny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtwojznaqi.html

[C10] 变量作用域
来源：http://hz.shuidangran.top/gtrtpkdfdo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtuedpigww.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cucudq.cn/gtkcfegzdv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtsevhwmow.html

TS:   同 JS
来源：http://hz.zdqjudy.top/gtgmqojdfc.html

Java: 方法内为块级作用域
来源：http://hz.snrcjt.cn/gtjqfjsmmp.html

Go:   花括号块级作用域
来源：http://hz.jinghuilouyu.cn/gtzlbyrwui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jiagoushi.top/gtdiqvxtnu.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtfehtvtxe.html

[C11] 模块导入与导出
来源：http://hz.zhengqikj.top/gtpdlxhgyf.html

Py:   from module import func
来源：http://hz.yj20258.top/gtanhknlob.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.redwolf501.top/gtjnxogdnu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtdjeeeglu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenlongwang.top/gtxyhbjfgk.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtzgyktche.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.bjfxy.top/gtzojfwiou.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shangyingyoupin.top/gtpxibspxd.html

C#:   using System.Text;
来源：http://hz.jinqigfzy.top/gtgvsvwvmf.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxuanxn.top/gtnecnkbqu.html

Py:   (lambda: print("run"))()
来源：http://hz.smart0.xyz/gtcnsvbfol.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgufenzy.top/gtumwovodn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtinymifqa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtsqjtqxff.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtxisdnguw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtkatkzwjn.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtwhvgdsts.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtlqcxbxle.html

[C13] 类型声明 / 类型注解
来源：http://hz.xylfe.cn/gtycntmfth.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.52xcode.cn/gtlrgaijxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtwegmbyvk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnqzz.top/gtdpymybty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtptfzmfoa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtahtobjat.html

Go:   func add(a, b int) int
来源：http://hz.jinqigfzy.top/gtgwwbfrpk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtsxbulicd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtjoninblp.html

[C14] 泛型函数
来源：http://hz.havefunace.top/gtpyhhcbxv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jlsjyb.cn/gtmmtihyep.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtzcrnugmg.html

JS:   // 无泛型
来源：http://hz.xziqi.cn/gtctbkwptb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtikpjqvof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtinslfbex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtyhtqutqb.html

Ruby: # 无泛型
来源：http://hz.bjfxy.top/gtzxxpydsq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtpbxvihyf.html

[C15] 解构 / 展开参数
来源：http://hz.zdqjudy.top/gttzptjfos.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aibaodan.cn/gtkappcyfe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtkytlxkwq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtgmsynrzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.iojbl.cn/gtohnafcmh.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gthnvzlvhh.html

Go:   // 无解构
来源：http://hz.cdnleiting.top/gtyhdfhfbn.html

Ruby: a, b = pair
来源：http://hz.jqgfzy.top/gtkiopuaju.html

C#:   var (a, b) = pair;
来源：http://hz.yvedp.cn/gtkgvxtswe.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtgxeygebl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtiysyufdf.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gthqvrjody.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gtecewcczh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gzhubu.top/gtwkshuhbf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydzc1.top/gtzsbtmcew.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuanzx.com/gtbgooxfsr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ywan-chungtsiang.top/gtpeukdxpv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.redwolf501.top/gthjdtvjqt.html

================================================================================
来源：http://hz.yuxming.cn/gtbvbgfssm.html

D. 数组 / 列表 / 集合
来源：http://hz.yonumen.top/gtfhzylime.html

================================================================================
来源：http://hz.nwbrower.top/gteyaxjudg.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gtjjvohtbj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sufxvd.cn/gtxymptzaj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenjidiqi.icu/gtkaaloryp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxuanxn.top/gtiwsrimkg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.aibaodan.cn/gtkcljzvdb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtfxeyjenn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shzxlz.cn/gtzduoxmrh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tian-w.cn/gtzrmzelow.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pengpengdd.cyou/gtdczcpauo.html

[D02] 追加元素到末尾
来源：http://hz.hysaishi.cn/gtsqbsflzn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gtturxbqtp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtozcwpboa.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtuadaklar.html

TS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtvmdcablc.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gtekziizln.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gtvksgdemg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cashguo.top/gtzvrszjir.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtjrbtwtau.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtgdmuvlvm.html

Py:   arr.insert(0, 0)
来源：http://hz.c1oappe.top/gtrdaeacyt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gteilmjlmm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtdcihhcbr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gttmnppiab.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtgpupolor.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtknjqgshp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtxhemrzdu.html

C#:   list.Insert(0, 0);
来源：http://hz.jiagoushi.top/gtktzssfro.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtjcofkrmz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtbtrzcbcz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtpklavafq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtlzphfllt.html

TS:   arr.splice(0, 1);
来源：http://hz.daria6918.cn/gtfiwpylep.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtuidyofbe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuetiantiany.cn/gtfhmvfjkx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtudlsyibr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtucivjhmg.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtzglruyqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtifhloikx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtmluejkzb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtwmuzzdsb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tianlin.xyz/gtapodzrnj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtznhmxcrb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xinyue.icu/gtsykqsqlv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtzpfozceb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtnhltpbcj.html

[D06] 数组长度
来源：http://hz.vqdsnc.cn/gteagofbwe.html

Py:   len(arr)
来源：http://hz.gogol.net.cn/gtsgdbcbyh.html

PHP:  count($arr);
来源：http://hz.ybcxt.top/gtqvdcyrvw.html

JS:   arr.length
来源：http://hz.aibaodan.cn/gtxzkpzwlv.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtbuxdrtbc.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtxaeliyeg.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtigxuxnpi.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtrbwtmzpj.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtngsbcyxk.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gtdbkmsmvx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tianlin.xyz/gtlwlixhke.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gttzjfdate.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtdrhlfmch.html

TS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtcotfbomd.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtlpcjubic.html

Go:   arr[1:4]
来源：http://hz.zdqjudy.top/gtpofwpbjq.html

Ruby: arr[1, 3]
来源：http://hz.fengsongda.top/gttplsubro.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtiqhxjnxl.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtbxbktwmp.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtbcglnivs.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtflcqheti.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtclfuvcqc.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtvuwnbkdv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.svipenyu.cn/gtefrnkocm.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtrlwejdmy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtaxzaugyk.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgfzy.top/gtozjiqxrx.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangkeji.top/gtwmdxqlis.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtvicwirge.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gtyjeimqpr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtlsckildl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.birdmap.top/gtiboejnls.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtrxikloxb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yueranfly.top/gtlkrcarmc.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtxgelmszs.html

C#:   list.Sort();
来源：http://hz.yuxming.cn/gtrqzbypns.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gthgjiohlh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gthbdzxfcm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gtiytxeuzx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtqmuqighx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtyabmukdd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gthcrzjbxh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtjbizxhgs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.andypj.xyz/gtzketiiiy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hysaishi.cn/gtfmzdbcal.html


<!-- 参考信息 -->