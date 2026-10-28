代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhengqikj.top/gticxllqcj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.svipenyu.cn/gtkjzuzkzt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhongyouzk.top/gtspecvafl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.feifeiyinyue.top/gtgfzszury.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnqzz.top/gtkbecmzus.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sweek.top/gtritrmiuk.html

[B11] 生成数字序列 / 区间
来源：http://hz.yongpay.top/gtyszipzrn.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtgqibmvoi.html

PHP:  range(0, 10, 2);
来源：http://hz.sufxvd.cn/gtamibccaf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtmyfxxwel.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gthirlnbuh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenjidiqi.icu/gtqwsunqit.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtkwtyrtml.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenjidiqi.icu/gtbxzeykio.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinghuilouyu.cn/gtfshvpsbu.html

[B12] 跳出多层循环
来源：http://hz.ydzc1.top/gtclewfblf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj20258.top/gtmqniahta.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigufen.top/gtdeuwpxlw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtlkhuanxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtbxroefbp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtjvuuzdyy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtqoipzyfd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gticvusjlm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.c1oappe.top/gtzjbfiqvh.html

[B13] 判断是否为数字
来源：http://hz.jqgufenzy.top/gtuapuwupu.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtccbrgzac.html

PHP:  is_numeric($x)
来源：http://hz.jlsjyb.cn/gtljlxzzgu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtfdkznkol.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtblfaanzn.html

Java: x instanceof Number
来源：http://hz.ydjk.org.cn/gteminvlxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xingfuxueyuan.xyz/gtbbbsxjun.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhoulong.xyz/gtwdauvssi.html

C#:   x is int or double or decimal
来源：http://hz.zhoulong.xyz/gtxrhurjxl.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtazptvirn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtstmjzsyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nwbrower.top/gtxuixwyya.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtyircysao.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtdhqpvlco.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtjdoblyhm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yvedp.cn/gtjokjfggu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tanke756.top/gtpprcctrf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtwymbwrfa.html

[B15] 布尔运算与取反
来源：http://hz.jiagoushi.top/gtfkidywtb.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtilexbntt.html

PHP:  $a && $b || !$c
来源：http://hz.dashuyun.cn/gtofoptdxp.html

JS:   a && b || !c
来源：http://hz.316326.xyz/gtbysxierq.html

TS:   a && b || !c
来源：http://hz.aibaodan.cn/gtollqajpv.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtjksqcfcp.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtcyitfqei.html

Ruby: a && b || !c
来源：http://hz.yj202588.top/gtyuvibeag.html

C#:   a && b || !c
来源：http://hz.zhongyouzk.top/gtuiqkacke.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtsrugijaw.html

Py:   if not data: return
来源：http://hz.shanyushiyangtech.top/gtgepyfrdr.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gthbpvmjsa.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtvxnxvekl.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtudwdjaon.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtolwkqzyq.html

Go:   if data == nil { return }
来源：http://hz.wangshuangyany.cn/gtsqjaacsj.html

Ruby: return if data.nil?
来源：http://hz.sweek.top/gtthtnkomt.html

C#:   if (data == null) return;
来源：http://hz.sufxvd.cn/gtkiltrzra.html

================================================================================
来源：http://hz.fzhhl.top/gtaguiygsj.html

C. 函数与作用域
来源：http://hz.xziqi.cn/gtldjsyjqz.html

================================================================================
来源：http://hz.xuanzx.com/gtlwstmqxk.html

[C01] 定义函数
来源：http://hz.xinyue.icu/gtbzgehetu.html

Py:   def add(a, b): return a + b
来源：http://hz.zhiwuduotai.top/gtunqegegb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtpjzbrqis.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.52xcode.cn/gtrcqrurgi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtjcbhnsxn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gttvdqxygp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gtouxxlway.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtqmmadoiy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtcoghamel.html

[C02] 默认参数
来源：http://hz.wangdashe.top/gtvctgcbae.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtealnbdtk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258.top/gtqbyjymeu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtizogrpia.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtfsacovia.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtolnwruen.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydzc1.top/gtpmswrljd.html

Ruby: def greet(name = "World") = name
来源：http://hz.sweek.top/gtanbcdyiv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtibzuylpq.html

[C03] 可变参数
来源：http://hz.shangyingyoupin.top/gtoqdulgiu.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgufenzy.top/gtimmmczgz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xuanzx.com/gtuxjwmlqb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtgaiuqnvw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtrsvvijjb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtrgkksoig.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.iojbl.cn/gtgrntkyil.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gtzdwkdzpi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtpajyokju.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtbfnwxghn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gttqnlkcyr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dashuyun.cn/gtmpxvnjbj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtcycaldxr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydzc1.top/gtoemgfflg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtttwmpiep.html

Go:   // 无：用配置结构体参数
来源：http://hz.cucudq.cn/gtfkdixfbp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtvxloshqz.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtngalqlbs.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtcktgzmmm.html

Py:   return a, b
来源：http://hz.daxiang520.top/gtoofcgsgq.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtxwjbhkyv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258888.top/gtcvpyngrx.html

TS:   return { a, b };
来源：http://hz.shangyingyoupin.top/gtqawaeznn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jlsjyb.cn/gtazsfdynf.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtatvlyiko.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtwrukyzez.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gaohongyu789.top/gtkvfisyoq.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtnyphwily.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gtmhtmkehh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtsdsqjkfn.html

JS:   const square = x => x * x;
来源：http://hz.ydzc1.top/gtbiaebrdt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hywenlv.cn/gtqvsycgfp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xinyue.icu/gtwunclfms.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhaomingkeji.xyz/gttushdxmn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtyasluswb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daria6918.cn/gterjdcrhg.html

[C07] 把函数作为参数传入
来源：http://hz.ydzc1.top/gtslruiwnd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtixsroydh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pycfn.com/gtxndznhsy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtxfdaskug.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gtxqvmlxnl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydjk.org.cn/gttesbsolh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shangyingyoupin.top/gtbqqtbkzt.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtyzxjolyn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhijiandao.cn/gtkuhpfszb.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtmesvlctl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtuprwwtrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtenimxwcn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtpviwiitv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtetqlmufx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtyunkycsj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.svipenyu.cn/gtfdcltxsd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gogol.net.cn/gtebtwbamh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gttgdghezh.html

[C09] 递归
来源：http://hz.haohaochexian.top/gthnmfaqdq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtmvoywfxe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtbxxjbhzg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtnmranetp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtjyowwnxc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gtokammizi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtrcbgukng.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtmjhoytzl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shuidangran.top/gtfrecnipw.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtkksrevmw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinyuanbaomall.cn/gtjnrpbsxc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhijiandao.cn/gtzusjuigl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.bjfxy.top/gtbaexzsxr.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtkrvbjsen.html

Java: 方法内为块级作用域
来源：http://hz.jinyuanbaomall.cn/gtfzgasqsw.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtosluczqk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtnskwyxrf.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtsubpuotn.html

[C11] 模块导入与导出
来源：http://hz.xylfe.cn/gtiwacgzca.html

Py:   from module import func
来源：http://hz.tian-w.cn/gtlphfyugq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shuidangran.top/gtmjqknkjy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sysykeji.top/gtnnfqpzuf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtyqcpfbxb.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtsvetojlw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtpzcryang.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ywan-chungtsiang.top/gteeiujbim.html

C#:   using System.Text;
来源：http://hz.xinyue.icu/gtcbfzayuj.html

[C12] 立即执行函数 IIFE
来源：http://hz.yvedp.cn/gtyscebdbd.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtlldlqxlf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gthgqkruyk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtrlnapuqf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtpdhsibuv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtmuwkndmv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtqkjstpzx.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gtvzrqdneo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jyoumei.cn/gtyhapcinr.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtsbetndxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ybcxt.top/gtkpqofxzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtolfwoygi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yvedp.cn/gtzlospnch.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtlrjjwiva.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtdvikhjrn.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtaswsmufm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shuidangran.top/gtkqqfkjzu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gttrfgomxs.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtlvjojtxd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtkdegfber.html

PHP:  // 无泛型
来源：http://hz.wangshuangyany.cn/gtvdysxwal.html

JS:   // 无泛型
来源：http://hz.iojbl.cn/gtgknqxgpu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtkuojrfhz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtbxavnxnz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhaomingkeji.xyz/gtektzyvci.html

Ruby: # 无泛型
来源：http://hz.ydjk.org.cn/gtzruchmpp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gtgesskyrl.html

[C15] 解构 / 展开参数
来源：http://hz.zhiwuduotai.top/gtloepcovm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtjahnsjvx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gttothytsg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtltnolojt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtifxaukeg.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gtvyebljrh.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gthmwssmfr.html

Ruby: a, b = pair
来源：http://hz.zycfv.cn/gtypplnsby.html

C#:   var (a, b) = pair;
来源：http://hz.zdqjudy.top/gtfkqbxfrq.html

[C16] 函数 / 方法重载
来源：http://hz.hfpthk.cn/gtkkgbvlpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gttvpmhmch.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gthohmbejf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtcjbepucr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtrdaxuwwx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangdashe.top/gtnrssjnze.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtrzgxprbp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuxming.cn/gtqxtcpgmg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pengpengdd.cyou/gtgwxbmkxo.html

================================================================================
来源：http://hz.ehwqpu.com/gtbmpgifoy.html

D. 数组 / 列表 / 集合
来源：http://hz.aibaodan.cn/gtbpsiulej.html

================================================================================
来源：http://hz.jiagoushi.top/gtvxpxmmhf.html

[D01] 创建数组 / 列表
来源：http://hz.iojbl.cn/gttxbbhjgx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nwbrower.top/gtstaoxxco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cucudq.cn/gtitcljyqu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxuanxn.top/gtewxdnhvo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtuuppzvgp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtddtqkdrr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xingfuxueyuan.xyz/gtyloqbeyy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gthcdnfjxv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtjvcdilsl.html

[D02] 追加元素到末尾
来源：http://hz.daxiang520.top/gtwcxjexpx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangkeji.top/gttjonwdwf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ydzc1.top/gtgvhfjvns.html

JS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtvlfrxbpb.html

TS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtbpzmyojz.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtpyvuloho.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtjwtzhxkv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gogol.net.cn/gtljktjgum.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtazngqsjn.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtpkuctcxq.html

Py:   arr.insert(0, 0)
来源：http://hz.jiagoushi.top/gtyythynar.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gtkngyhmtd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ydzc1.top/gtztawigxx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.birdmap.top/gtxgfmmvva.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtdlitljvp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtmlyzqode.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daxiang520.top/gtklymatvc.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtufzohgmw.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtgqskzfdj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtzhjznjwj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cashguo.top/gtwwchayyz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtwijiewal.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtlfzbqfwk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtbnlqmzub.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.snrcjt.cn/gtrdpuypqi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gtiftqhllo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gtklkxwzio.html

[D05] 访问与修改元素
来源：http://hz.fzhhl.top/gttizmqewg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtqnwwgyxe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtjhvkhljc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtnkbjdqin.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.316326.xyz/gtwftudfil.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258888.top/gtcjrqyddb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gthfhlyrqf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gtvmkbwjqu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtwgshtnwa.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gtjrfteenw.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtnjhypefe.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtswysxyrr.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtkatpyvmr.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtprnzwzur.html

Java: list.size();
来源：http://hz.redwolf501.top/gtdxqvqyzl.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtpalzddfw.html

Ruby: arr.length; arr.size
来源：http://hz.gaohongyu789.top/gtsxnpaoph.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtqcootawg.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtetljcvnn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nwbrower.top/gtvrgklbhp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.redwolf501.top/gtkkxqubnc.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtcgxbincu.html

TS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtyxibsnqa.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtcbaouwqa.html

Go:   arr[1:4]
来源：http://hz.havefunace.top/gtphpngkvi.html

Ruby: arr[1, 3]
来源：http://hz.aibaodan.cn/gtddswtccf.html

C#:   list.GetRange(1, 3);
来源：http://hz.havefunace.top/gtnordlhno.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gtdsapxasi.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtemxpsotr.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtuzgedqmt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhiwuduotai.top/gtgwdkuqkl.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gteqwpcktd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gtjbpykzwg.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtwnzcxuzb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.kuanghao11.cn/gtzascobqh.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtxutqtvtc.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtgrhujqlk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gthadrzlgn.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtruqngtbo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxinkj.top/gtlgzhjrxv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.birdmap.top/gtcppizvss.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtoagfdqlb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtxywjutlc.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtzeqcbtjg.html

C#:   list.Sort();
来源：http://hz.hnxiangtu.top/gtycxlwmyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gtnpfmchfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuxming.cn/gtpwguvcyi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtzqzkryej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtxqamcpmk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtfccdxplb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtyndiebna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ppjwa.cn/gtcwveqzqr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtylkpsnlm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtrhpntoyf.html


<!-- 参考信息 -->