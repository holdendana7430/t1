代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gteeursroi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yonumen.top/gtvbpmqvqt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xylfe.cn/gtpapwnzkk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yanxiufei.cn/gtqagirfjg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.316326.xyz/gtukvdrgxh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cucudq.cn/gthvollvof.html

[B11] 生成数字序列 / 区间
来源：http://hz.andypj.xyz/gtsjqrbvbc.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gthblxdlzy.html

PHP:  range(0, 10, 2);
来源：http://hz.zhongyouzk.top/gtlwtpqhef.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtnsthqwmc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtpmvphbrk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtvfmxxpqw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnqzz.top/gtdwgkxvps.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtvztfmhdj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhengqikj.top/gtdzqrxfek.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gttjxwmkpe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ivvv.top/gtoibisisg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.vqdsnc.cn/gtthfrncrw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtyvemebio.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtlhenowfl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtcmgqjoek.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtdvzyksga.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258.top/gttaccuoqm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yvedp.cn/gtdhvcwghp.html

[B13] 判断是否为数字
来源：http://hz.zhijiandao.cn/gtjzgpydum.html

Py:   isinstance(x, (int, float))
来源：http://hz.tanke756.top/gtxinwfkiy.html

PHP:  is_numeric($x)
来源：http://hz.aizwys.cn/gtrqevtsxz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtvyouivmn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtmonnxvts.html

Java: x instanceof Number
来源：http://hz.zhoulong.xyz/gtacdhmfnj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yongpay.top/gtujfmvbag.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtjgunrvnt.html

C#:   x is int or double or decimal
来源：http://hz.gaohongyu789.top/gtrkyjvcjs.html

[B14] 判断值是否在集合内
来源：http://hz.fzhhl.top/gtegtbecca.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenjidiqi.icu/gtoeecszia.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.quarkkingdee.top/gtahxgkfgt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hysaishi.cn/gtfvroidvo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtnbhfulom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.kuanghao11.cn/gtvllhewlb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.pengpengdd.cyou/gtasbfcatq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ehwqpu.com/gtftwydkbs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtngtmpbmh.html

[B15] 布尔运算与取反
来源：http://hz.daxiang520.top/gtbujtweck.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtxlsxrjkt.html

PHP:  $a && $b || !$c
来源：http://hz.shanyushiyangkeji.top/gtiymkylfp.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtgxbzsvri.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtyidwvubh.html

Java: a && b || !c
来源：http://hz.xinyue.icu/gtluklejqx.html

Go:   a && b || !c
来源：http://hz.cashguo.top/gtcgjpremm.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtpuzdmctc.html

C#:   a && b || !c
来源：http://hz.jqgufenzy.top/gtioxeqmrt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.meibo888.top/gtfenqkqno.html

Py:   if not data: return
来源：http://hz.daria6918.cn/gteaiojlcr.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtzphhzdcb.html

JS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtwwhqazso.html

TS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtgcsgbvew.html

Java: if (data == null) return;
来源：http://hz.wangshuangyany.cn/gthviexmbm.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtqkpjamhb.html

Ruby: return if data.nil?
来源：http://hz.gotoacloud.top/gtinevgofd.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtrdfnkxrd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbtmgltyk.html

C. 函数与作用域
来源：http://hz.jinqigufen.top/gtgelkykcy.html

================================================================================
来源：http://hz.9152youxi.cn/gtbkbtvcio.html

[C01] 定义函数
来源：http://hz.hongshengwenyu.top/gtaakswmpw.html

Py:   def add(a, b): return a + b
来源：http://hz.yj20258.top/gthfzxgbzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtnlrefcwb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pycfn.com/gtuldfrqja.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtdhoqcmaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtrqobiuag.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtrlkanhjz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sweek.top/gtgoguvofz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtgqrnyimb.html

[C02] 默认参数
来源：http://hz.jyoumei.cn/gtpyonteqc.html

Py:   def greet(name="World"): return name
来源：http://hz.jiagoushi.top/gtwdosltiq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtzdwscneg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtkzgruelo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtandnxjnp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gtgnlkzmla.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guannengcc.top/gteszlcfdo.html

Ruby: def greet(name = "World") = name
来源：http://hz.fzhhl.top/gtiqhhmjhn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pycfn.com/gtepwfadoc.html

[C03] 可变参数
来源：http://hz.ybcxt.top/gtzhugzcip.html

Py:   def total(*args): return sum(args)
来源：http://hz.kuanghao11.cn/gteafeicuj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gteqkidyec.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtamnficwv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtgkxbwqgq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yanxiufei.cn/gtsomrrjul.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hfpthk.cn/gtqxkfxvfj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtwdkyxtuu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.bjfxy.top/gtcsalkqrt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yangfankeji.com/gthmlpyduy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxinkj.top/gtwfldgjxu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydjk.org.cn/gtfvctqxry.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtgpkdqaxv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtvklhoehn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gthwmharal.html

Go:   // 无：用配置结构体参数
来源：http://hz.redwolf501.top/gtskqejfiu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtcqsrcejx.html

C#:   f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtlmwddmmj.html

[C05] 返回多个值
来源：http://hz.yongpay.top/gtkenjfqiz.html

Py:   return a, b
来源：http://hz.ydzc1.top/gtoeivjsch.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtictklbdw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yonumen.top/gtetiivnlp.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtltvkmcep.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtvrpnosop.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtlfwmlyug.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtfrfrfept.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tanke756.top/gteweccyuc.html

[C06] 匿名函数 / lambda
来源：http://hz.pengpengdd.cyou/gtpkgoqdkd.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtnxxnlghq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gttiubbdwt.html

JS:   const square = x => x * x;
来源：http://hz.ehwqpu.com/gtcksizvwm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gtsuhtgcsg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shzxlz.cn/gtaanqbocx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtezakwsnw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtmhrzbfmm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.vqdsnc.cn/gtucqgyuyx.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gthkoafuis.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pengpengdd.cyou/gtmtnxqjxv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shuidangran.top/gtmjydalsg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtjdqavclk.html

TS:   arr.map(String)
来源：http://hz.ehwqpu.com/gthwxalkzs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gthdprelli.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhiwuduotai.top/gtfhqrmrpq.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydjk.org.cn/gthnhabjsp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtxxepebfv.html

[C08] 闭包
来源：http://hz.quarkkingdee.top/gtowguqusn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtxtmachvu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gtsrdzmyqb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtvrvyzrkm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtdyvrvpdz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtlhaqdabo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sufxvd.cn/gtlusiecdz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gthmciphvt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtcnzkbezm.html

[C09] 递归
来源：http://hz.yvedp.cn/gtcdtkgimf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.smart0.xyz/gtzgvubmri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.quarkkingdee.top/gtuhisazfo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtbsadknam.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtrqievrhw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxinkj.top/gtkavqxbij.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gtzekvcitz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xziqi.cn/gtczxbwgai.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.kuanghao11.cn/gtukovitnv.html

[C10] 变量作用域
来源：http://hz.chenlongwang.top/gtvaodfqvp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yonumen.top/gtxxyzlast.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.9152youxi.cn/gtyhdwokex.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.smart0.xyz/gthwlyetgm.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtohvgzcmi.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gthllkjcyj.html

Go:   花括号块级作用域
来源：http://hz.pengpengdd.cyou/gtgzjiblzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gtgnubaedr.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtmlxwsccf.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtzmdzuipg.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtncjhtalx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtpttbgnzt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nanxinkj.top/gtelsvqbkl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hongshengwenyu.top/gtdujoywgz.html

Java: import java.util.List;
来源：http://hz.snrcjt.cn/gtaajnywsv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.0kj1m.cn/gtbuiaxpdu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jianghu66.top/gtxizhgjyx.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtexcpewci.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gtanjshrsv.html

Py:   (lambda: print("run"))()
来源：http://hz.hnqzz.top/gtvggjffqo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dashuyun.cn/gtrbasdmrr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtyoysgzdw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtoksufdaq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sxryk.cn/gtlfnjcrch.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtrzadzhip.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gthslfsxmk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtytsahdbv.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuanzx.com/gtynxymthb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gotoacloud.top/gtwbihgjjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtsiszvotp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.meibo888.top/gtcqnzsowa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtlairlcii.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtavgylivb.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtgijlqwzh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dianchejie.cn/gtkdrfekbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gtidmkkshm.html

[C14] 泛型函数
来源：http://hz.jinyuanbaomall.cn/gtqeysfhzy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangdashe.top/gtxiodecan.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtbrljzfya.html

JS:   // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtbfxzqxss.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.haohaochexian.top/gtujnxwdvt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxuanxn.top/gttflfnqjz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxinkj.top/gtwqresguo.html

Ruby: # 无泛型
来源：http://hz.yangfankeji.com/gtnktvoktv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.vqdsnc.cn/gtrgzeqxqr.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gthccwczdk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtbpdlowil.html

PHP:  [$a, $b] = $pair;
来源：http://hz.0kj1m.cn/gtlhfqlikn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtdwfphnrd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtboxjware.html

Java: // 无解构
来源：http://hz.yanxiufei.cn/gtdwopmhzq.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtlheiuipb.html

Ruby: a, b = pair
来源：http://hz.zhongyouzk.top/gtfzmymjfw.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtpctqdckr.html

[C16] 函数 / 方法重载
来源：http://hz.jyoumei.cn/gtokgoqtqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtfggemivl.html

PHP:  // 无重载
来源：http://hz.cucudq.cn/gtkzmkuavt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhongyouzk.top/gtxmijnmfl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnxiangtu.top/gtgzwtozql.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fengsongda.top/gtoehtgket.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenzaomai.com/gtwwyknmoy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtwsovquri.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtvdevauir.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtxkivpthv.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gtvujkyvjj.html

================================================================================
来源：http://hz.316326.xyz/gtveaaiifo.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtwsllrykr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.daria6918.cn/gtadxwbtqm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zdqjudy.top/gthredayoe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ppjwa.cn/gtutlrxvpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtrlmovyul.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gturzdwyrm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.vqdsnc.cn/gtcyehcszh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ehwqpu.com/gtkttysjdt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtjkxicmtw.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtbxafmfuy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gttaitofcx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtqibwbrcr.html

JS:   arr.push(4);
来源：http://hz.yangfankeji.com/gtvwfrhpjr.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtzugfyzbu.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtpbwnusya.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gtoqyfqkmm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtlorkoadu.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtnlgcgwtt.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtajtrnlre.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtpwkilzpr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gtiueabejr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtmdxwkzbm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.redwolf501.top/gtffidtnuh.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gtiuvyhyig.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinyuanbaomall.cn/gtcsbamgic.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cucudq.cn/gtmcocuorf.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gtxwwjufpp.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gtvyjqmckn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cheryme.top/gtioucxjkw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.mhx1999.top/gtlwnjiszh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gtsmmohljy.html

TS:   arr.splice(0, 1);
来源：http://hz.ydzc1.top/gtbgbkudgh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtovbvaxxs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhoulong.xyz/gtxogvepqz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gtwmvyzsce.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xinyue.icu/gtnbzcoivh.html

[D05] 访问与修改元素
来源：http://hz.yuanzhike.top/gttwpljret.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtzwhpnibg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtmdtwnawo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuanzx.com/gtyhrkfsst.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtmxxupymn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zycfv.cn/gtvzgkezju.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtsvjbfnyn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtzmhffnga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtlwywnrha.html

[D06] 数组长度
来源：http://hz.0kj1m.cn/gtmwrskjnd.html

Py:   len(arr)
来源：http://hz.sufxvd.cn/gttbjilocx.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtaninhrig.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtoglazydd.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtyesohwij.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtdyxczbed.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtmkjymnsk.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gtzhmrupeu.html

C#:   list.Count;
来源：http://hz.birdmap.top/gtmzxznjvp.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtczmkadxk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.snrcjt.cn/gtbjrtjbuh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtxaiqamnk.html

JS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtizrgdlcp.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtxovrcmhy.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtdyeecnvl.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtfrcrkhyv.html

Ruby: arr[1, 3]
来源：http://hz.feifeiyinyue.top/gtbamhffup.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtqlhokpnl.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gtziexhvmp.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtggkzydxe.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigfzy.top/gteqjnjwmg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.haohaochexian.top/gtddgditfg.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtbccudyfi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sufxvd.cn/gtszufmpcc.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtgtqlqkxm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtwytbgojz.html

C#:   a.Concat(b).ToList()
来源：http://hz.gzhubu.top/gtyljgqfmn.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtxinqrfcc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtfseltscr.html

PHP:  sort($arr);
来源：http://hz.shuidangran.top/gtcqzkpqzm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxinkj.top/gtikjpvpye.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.vqdsnc.cn/gtxlklstjg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtkfakheji.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtocqvehan.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtdmozjnsc.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtlgvbfmfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.aibaodan.cn/gtanbwgsva.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtexkbxeym.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gttmtyatfv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gthhblqguc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtzzyjvtnx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.andypj.xyz/gteotqfkga.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtttdtydcq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtlwybpjka.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtbhjygzla.html


<!-- 参考信息 -->