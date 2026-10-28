代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtkinjatei.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtotyhppwu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtepmiycsa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.andypj.xyz/gtmeatowhp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtbsrzrgir.html

[B10] 遍历同时拿索引
来源：http://hz.sufxvd.cn/gtcyhnimtl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sxryk.cn/gtndiexhen.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.316326.xyz/gtllanvius.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtiebadysm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.andypj.xyz/gtdkoiosdt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.birdmap.top/gtixddpelj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gzhubu.top/gtocjiwzxb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guannengcc.top/gtnbcltcqa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.mhx1999.top/gtplppshif.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtjxwnboqc.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtcptmjtwf.html

PHP:  range(0, 10, 2);
来源：http://hz.dashuyun.cn/gtipcbtlpo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxinkj.top/gtuhlyqqdq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtanetnvjl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.gogol.net.cn/gtquprucsh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.c1oappe.top/gtogggqqsw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hammf.cn/gtavxzvmpb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhongyouzk.top/gtyowspjge.html

[B12] 跳出多层循环
来源：http://hz.cucudq.cn/gtboyrgujl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gaohongyu789.top/gtuwbngahq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xuanzx.com/gterdvcbna.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtdwizujts.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtowjqooss.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtdewsfgdx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nwbrower.top/gtqwnkwkfp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cdnleiting.top/gtgjdlkcrf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtmfjpphun.html

[B13] 判断是否为数字
来源：http://hz.havefunace.top/gtqoeimytq.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gtcyjvfqwb.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtwtohpedh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtducaemuf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtkgiilpae.html

Java: x instanceof Number
来源：http://hz.9152youxi.cn/gtktmltsxg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhaomingkeji.xyz/gtqicrmtpa.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuanzhike.top/gtwijiyeyr.html

C#:   x is int or double or decimal
来源：http://hz.ehwqpu.com/gtcakqohkr.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtxhbzvzoq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtxpgyooiv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenlongwang.top/gtjcuqujvx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtkiwuugfp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtferbaqeg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtadixurxz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtehnqyomq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydjk.org.cn/gtrfofdyqm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yonumen.top/gtanqfrlzt.html

[B15] 布尔运算与取反
来源：http://hz.birdmap.top/gtitasrjok.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gtemlvyurj.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtzcgsyyms.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtstingbrq.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtfhwrzyia.html

Java: a && b || !c
来源：http://hz.snrcjt.cn/gtmanzpgre.html

Go:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtboxicrsn.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtqkoeakmi.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gttqnlyvpf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtrwcbzvqk.html

Py:   if not data: return
来源：http://hz.gogol.net.cn/gtvlulxdgu.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgufenzy.top/gtlxbuwjob.html

JS:   if (!data) return;
来源：http://hz.yonumen.top/gtcatwfdhu.html

TS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gttqliydfb.html

Java: if (data == null) return;
来源：http://hz.jiagoushi.top/gtfxryjibw.html

Go:   if data == nil { return }
来源：http://hz.xylfe.cn/gtklwyjayo.html

Ruby: return if data.nil?
来源：http://hz.gaohongyu789.top/gtnrekummu.html

C#:   if (data == null) return;
来源：http://hz.gaohongyu789.top/gtqgkaxbih.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwqcpdhij.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gtwciewriv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqtukfapx.html

[C01] 定义函数
来源：http://hz.0kj1m.cn/gtacylxwjn.html

Py:   def add(a, b): return a + b
来源：http://hz.jyoumei.cn/gtzcyyjkwd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtvmhjpwik.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtjjtlmroe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtvizgeypk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtjonmsabl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtmbzzblmx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guowangkeji.top/gtvgbjvwas.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtvhmuwsgu.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtedmxfckg.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtaegekrvj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gtwmyrtrtx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.guowangkeji.top/gthhhytuyg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtjpcfwrqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtvixghkmu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtrulifdsn.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtsivnxpab.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gttjkmuhul.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtdedkxfbp.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gthcviwxfd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.bjfxy.top/gtlkmgtfic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gthtgrxjuu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtquywplpg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gtibbfvzib.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtjysmceni.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangshuangyany.cn/gtqrjlofea.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guowangkeji.top/gtjgbvxmay.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenlongwang.top/gtisatwayt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtdfcmlpfa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tianlin.xyz/gtmcsjzgbm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtbmdquhin.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinyuanbaomall.cn/gtwtfepbzw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtrihqsjbg.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtzflczsgw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtmvfjaxxd.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gttamftrij.html

[C05] 返回多个值
来源：http://hz.zycfv.cn/gtaalmacdd.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtddlcwqcr.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtloemzkox.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuanzx.com/gttpvnwhoi.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtejzabooh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sufxvd.cn/gtuolabjht.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtqjwgjemr.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtcpkfkmji.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.0kj1m.cn/gtvyqtbybo.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangkeji.top/gtrynskucd.html

Py:   square = lambda x: x * x
来源：http://hz.c1oappe.top/gtwabzcewb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yonumen.top/gtpehapfrp.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gtcbjabigs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gtctkejajj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gtogrjwvwl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtbjqnaszv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtxdtvvter.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.bjfxy.top/gtoxavhsmp.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gtqnccbbco.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cucudq.cn/gtblmangob.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangshuangyany.cn/gtuhsobran.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shanyushiyangkeji.top/gttbxoddsj.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtswbzhqlx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gttwowfvmg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.kuanghao11.cn/gtthpiyfrd.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtxpipxjzy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtvjynknwm.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtmensmozl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xylfe.cn/gtumounegu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtptxjvbzk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtcjgwrueb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtzwtiqtmh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gtirrbszuq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nanxuanxn.top/gtqdhqxcur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtdmlvfoak.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtzpqmshrs.html

[C09] 递归
来源：http://hz.ybcxt.top/gtcifbpkkg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtibiryfwr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.meibo888.top/gtafjgmwva.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtiocorrbz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtqrjheffr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zdqjudy.top/gtxqzuozbb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigufen.top/gtmabgwgho.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gttovfnoim.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cheryme.top/gtlkdpwpqx.html

[C10] 变量作用域
来源：http://hz.ivvv.top/gtllrxsmpl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258888.top/gttlivsxik.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cheryme.top/gtqjusvruh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtjekowrak.html

TS:   同 JS
来源：http://hz.ydzc1.top/gtvzcqtoqm.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gtlztsdadt.html

Go:   花括号块级作用域
来源：http://hz.cdnleiting.top/gtqmemivxz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtsphwolwa.html

C#:   块级作用域
来源：http://hz.dashuyun.cn/gtxoweplkh.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtjrvychkm.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtpdccjeyu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtexmhlijk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.vqdsnc.cn/gthurqipkn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xingfuxueyuan.xyz/gtozgegsjr.html

Java: import java.util.List;
来源：http://hz.andypj.xyz/gtxwkuuidr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gthvcxyjux.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gtiajhilhl.html

C#:   using System.Text;
来源：http://hz.guannengcc.top/gthruncxbf.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtutrjpppe.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtnnmgirlr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhaomingkeji.xyz/gtlefwpqkk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.mhx1999.top/gttbforjvv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gteousvkqa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtxioghdht.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ppjwa.cn/gtexxapjhr.html

Ruby: -> { puts "run" }.call
来源：http://hz.guowangkeji.top/gtuabzpqtn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aibaodan.cn/gtpwcnyhjv.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtvbzroycm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtzhsogszf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtkhnoxbvk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigufen.top/gttrsnmlou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtueomdpnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtxopjfqcn.html

Go:   func add(a, b int) int
来源：http://hz.zdqjudy.top/gtiyxcxwom.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtmrgeqbec.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtcuwlpoui.html

[C14] 泛型函数
来源：http://hz.hfpthk.cn/gtntwbafhn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pycfn.com/gtgibudthn.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtxnvyzptu.html

JS:   // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtxeycbdne.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.haohaochexian.top/gthvfmftio.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zdqjudy.top/gtuugaaigy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gtpajqndmj.html

Ruby: # 无泛型
来源：http://hz.tian-w.cn/gtmkkoifmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtcvhkwerg.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtezfoephm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtettturnk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtlqlindze.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtmclqckko.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtuyunewlu.html

Java: // 无解构
来源：http://hz.xuanzx.com/gtajlhuhho.html

Go:   // 无解构
来源：http://hz.shangyingyoupin.top/gtcmgaijin.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gtrxzfoqul.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gttanhchsu.html

[C16] 函数 / 方法重载
来源：http://hz.yueranfly.top/gtdcxuekto.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jiagoushi.top/gtikeifyvs.html

PHP:  // 无重载
来源：http://hz.hfpthk.cn/gtatzawpht.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gaohongyu789.top/gtlfseggwp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtjfdvugre.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhoulong.xyz/gtaeblbcvh.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtkpjpvhdp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtwiluvpkr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj202588.top/gtwbypdska.html

================================================================================
来源：http://hz.ppjwa.cn/gtnfxgsccj.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtgtooepkj.html

================================================================================
来源：http://hz.gotoacloud.top/gtubtgwhcc.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtohqtyfoy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.9152youxi.cn/gtszbiblkj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtaebwewea.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtnhaokgpx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtxbwpditv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtwqeaclxw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gtjkedpxcp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxinkj.top/gtyfumyqby.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.kuanghao11.cn/gtnsgmgwez.html

[D02] 追加元素到末尾
来源：http://hz.yangfankeji.com/gtwydbcblc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cqqwz.cn/gtyjbmotqb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtzegcsnro.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gtqbypvzrg.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtfywvnakl.html

Java: list.add(4);
来源：http://hz.hfpthk.cn/gtwstnntwm.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtggrjntge.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aizwys.cn/gtyjhryhmf.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtqlyjaljk.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtqofkaxhk.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gtnjunxcza.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuanzhike.top/gtilormtpt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtqbnjzkyt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hywenlv.cn/gtykkwrczt.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtbifnxxcv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtursbsyjc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gtvvkcljby.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gttuyegenx.html

[D04] 删除元素
来源：http://hz.nwbrower.top/gtysjbkgvp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daria6918.cn/gthqkzrauf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuetiantiany.cn/gtcbwvviwu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daxiang520.top/gtbovyilqq.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtfbzzqrxo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtgkjmvryf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhixingplan.top/gtaliwuoqk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ehwqpu.com/gtjugmuqvf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cucudq.cn/gtnysuqawr.html

[D05] 访问与修改元素
来源：http://hz.mhx1999.top/gtwzlnlvig.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtwnjoxfui.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtzuakjblc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ppjwa.cn/gtqecelgsl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtkppqsgwl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.mhx1999.top/gtvspgbgba.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtisrraclt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtocnimepj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtjmudsibp.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gtlyzmbuik.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtdwvhcbeu.html

PHP:  count($arr);
来源：http://hz.ywan-chungtsiang.top/gtplwwgduc.html

JS:   arr.length
来源：http://hz.yonumen.top/gtdlvfgjqf.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gttkkljzmo.html

Java: list.size();
来源：http://hz.vqdsnc.cn/gtrroohrbt.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtclxbfxtv.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigufen.top/gtnkllgawb.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtksmmgllf.html

[D07] 切片 / 取子数组
来源：http://hz.yangfankeji.com/gtblcdzouo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigufen.top/gtfikccydh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtbqgnjxxf.html

JS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtpmnrufxr.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtyjtaknqv.html

Java: list.subList(1, 4);
来源：http://hz.hysaishi.cn/gtgomwiwze.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtultmzzcr.html

Ruby: arr[1, 3]
来源：http://hz.sufxvd.cn/gtkpglemlm.html

C#:   list.GetRange(1, 3);
来源：http://hz.ywan-chungtsiang.top/gtsyhspizl.html

[D08] 合并两个数组
来源：http://hz.hnqzz.top/gtjgwgfhay.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangtech.top/gtlwnaihor.html

PHP:  array_merge($a, $b);
来源：http://hz.cdnleiting.top/gtphjodily.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtweprreck.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtvqbykphf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tianlin.xyz/gtaoxlmrht.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gtympynyur.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtfdeyahct.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtituoemaq.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtjfytzpzp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gtwpefcniw.html

PHP:  sort($arr);
来源：http://hz.gzhubu.top/gtqglqubyj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinyuanbaomall.cn/gtkfihwnom.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gttgtkypmb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gtifhfpibg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtcmpzddrd.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtufxhovbc.html

C#:   list.Sort();
来源：http://hz.ydzc1.top/gttotkiqga.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtzesebwyq.html


<!-- 参考信息 -->