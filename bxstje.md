代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gthumnhxan.html

[B10] 遍历同时拿索引
来源：http://hz.meibo888.top/gtdnnrhhkq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guowangkeji.top/gtcpzdeegs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258.top/gttjcbyjje.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xziqi.cn/gtunzrdbds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yangfankeji.com/gtaqkwqydc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.redwolf501.top/gtxwewgbjk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.fengsongda.top/gtrnyglbta.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.9152youxi.cn/gtydfajuiv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinyuanbaomall.cn/gtuncmzjdz.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gtjpuotrgp.html

Py:   list(range(0, 10, 2))
来源：http://hz.jyoumei.cn/gtjnbiwzap.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigfzy.top/gtkqdjbdab.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinyuanbaomall.cn/gtviertmjg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtxhwwjzzj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtkjqnxwsy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fzhhl.top/gtxxeadrui.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuanzhike.top/gtootwlslr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aizwys.cn/gtajkgohwr.html

[B12] 跳出多层循环
来源：http://hz.52xcode.cn/gtvqymbuzb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.wangdashe.top/gtnfltskmv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daxiang520.top/gtlexhlrjf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtbdzlyzal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtbfgkchpw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtrgzblqfx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dianchejie.cn/gtdfykcvco.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gtvftgjcgf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtomwgxcet.html

[B13] 判断是否为数字
来源：http://hz.daria6918.cn/gtffmekvqe.html

Py:   isinstance(x, (int, float))
来源：http://hz.cqqwz.cn/gtrndzmsqg.html

PHP:  is_numeric($x)
来源：http://hz.haohaochexian.top/gtxsxkwaru.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtloiuhqtp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtiajnqpyb.html

Java: x instanceof Number
来源：http://hz.fengsongda.top/gtbunikmki.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cheryme.top/gthspxlvyt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tianlin.xyz/gtpxdfhqof.html

C#:   x is int or double or decimal
来源：http://hz.yuanzhike.top/gtqvbzuzti.html

[B14] 判断值是否在集合内
来源：http://hz.fzhhl.top/gtkgqdttcz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ehwqpu.com/gtgymyhngf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yanxiufei.cn/gtojfgcuvs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtudszcntg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtxdlawnok.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gogol.net.cn/gteuouzciu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtwkykndgj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtkmglhupn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.bjfxy.top/gtpxpkknsl.html

[B15] 布尔运算与取反
来源：http://hz.mhx1999.top/gtdltpntjd.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtnamxtxvl.html

PHP:  $a && $b || !$c
来源：http://hz.zhixingplan.top/gtdxcdndlf.html

JS:   a && b || !c
来源：http://hz.mhx1999.top/gtnrvkkgln.html

TS:   a && b || !c
来源：http://hz.cqqwz.cn/gtjaithbzj.html

Java: a && b || !c
来源：http://hz.zycfv.cn/gtokvfkomk.html

Go:   a && b || !c
来源：http://hz.fengsongda.top/gtqqodqzvo.html

Ruby: a && b || !c
来源：http://hz.jiagoushi.top/gtftgmijtf.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtayiyptvq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yvedp.cn/gtnvbfzipd.html

Py:   if not data: return
来源：http://hz.cheryme.top/gteonylxbd.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtisaplsxw.html

JS:   if (!data) return;
来源：http://hz.zhixingplan.top/gtodujogaq.html

TS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtyzmichpu.html

Java: if (data == null) return;
来源：http://hz.havefunace.top/gtlokesybe.html

Go:   if data == nil { return }
来源：http://hz.vqdsnc.cn/gtcixhlfvv.html

Ruby: return if data.nil?
来源：http://hz.yonumen.top/gtlxgiuiep.html

C#:   if (data == null) return;
来源：http://hz.wangshuangyany.cn/gtibwvbdly.html

================================================================================
来源：http://hz.zdqjudy.top/gtuorfrzal.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtrlqhemdn.html

================================================================================
来源：http://hz.xziqi.cn/gtjrefggbg.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtwtyqnjxh.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtldsgerpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtqdoqclyr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gthgitvtxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtozjdgayb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtzzsxuzcw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cdnleiting.top/gtgtheajuq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.birdmap.top/gtblxexgcn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtywyyqmjl.html

[C02] 默认参数
来源：http://hz.wangshuangyany.cn/gttuwtpfdl.html

Py:   def greet(name="World"): return name
来源：http://hz.hammf.cn/gtjwfvseiv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shangyingyoupin.top/gtskmsiuvn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtbvejnuah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtyedxzlor.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.svipenyu.cn/gtzxdsgerr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hammf.cn/gtpikftghh.html

Ruby: def greet(name = "World") = name
来源：http://hz.yanxiufei.cn/gtruaaikms.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cqqwz.cn/gtikgdyzjn.html

[C03] 可变参数
来源：http://hz.9152youxi.cn/gtugdcsfld.html

Py:   def total(*args): return sum(args)
来源：http://hz.tanke756.top/gtwbsplaxu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtstkjdenr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gthdwnhdin.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gttdjhtafn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hnxiangtu.top/gtowtjuudl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtqbtscety.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.redwolf501.top/gttlaikonm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xylfe.cn/gtakyenzdb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtzrtnuvud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.redwolf501.top/gtnsnhykqf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hongshengwenyu.top/gtedntplov.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtekrouuip.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tanke756.top/gtbcpbwxkd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.52xcode.cn/gtaajbpnxn.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtxqrpgpoa.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtrkzjygwv.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtegfnbjpz.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtlmpcjtlq.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtstjqsabu.html

PHP:  return [$a, $b];
来源：http://hz.yanxiufei.cn/gtkpqdtxuh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daria6918.cn/gtyuphkcje.html

TS:   return { a, b };
来源：http://hz.jlsjyb.cn/gtqztleybp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.haohaochexian.top/gtetkelhit.html

Go:   return a, b
来源：http://hz.hysaishi.cn/gtpvkjmrwa.html

Ruby: return a, b
来源：http://hz.9152youxi.cn/gtkuwwoyga.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sufxvd.cn/gtsruvvfxw.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtgknmndqj.html

Py:   square = lambda x: x * x
来源：http://hz.haohaochexian.top/gtxnysuvqw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gtuqcfsizb.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtzhrbeils.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gtgkivclbo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hywenlv.cn/gterikhher.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtvbwvxfcm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtetnbpfoq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gtyxppdwpu.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtlinvkoww.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtdjrgulgk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xylfe.cn/gtqazzzdoc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuanzhike.top/gtwvoaqfdv.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtaeyvuwbp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhaomingkeji.xyz/gtsomyjmei.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.52xcode.cn/gtbrefnsen.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuanzx.com/gtzluojxor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shangyingyoupin.top/gtztmlodsv.html

[C08] 闭包
来源：http://hz.jqgufenzy.top/gtaaowpsfe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ywan-chungtsiang.top/gtwemvldif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhoulong.xyz/gtcjqfhueu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gthwnjimcz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gthpvqykqh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sweek.top/gtfcwhsdwv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ehwqpu.com/gtolwmfhiy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtzruspcku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtqqixeylz.html

[C09] 递归
来源：http://hz.cashguo.top/gtzwckxbjw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtcxssntiz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tian-w.cn/gtmhgpfhea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtzjmczfol.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtkoejyoon.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtbptbtrbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtphnwtrec.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtmwwpihik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fzhhl.top/gtgmvquont.html

[C10] 变量作用域
来源：http://hz.zhoulong.xyz/gtqwdaneje.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtbngmoltc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtmfydxyha.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangdashe.top/gttmnywfud.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtdhntbqph.html

Java: 方法内为块级作用域
来源：http://hz.hnxiangtu.top/gtkbgqxobe.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gtoiqkbcew.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guowangkeji.top/gtutscvovd.html

C#:   块级作用域
来源：http://hz.52xcode.cn/gtgkhbpajc.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtioaucivq.html

Py:   from module import func
来源：http://hz.wangshuangyany.cn/gtjluifqhn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.redwolf501.top/gtomgiqdbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtembkkxef.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cashguo.top/gtrwrqteuw.html

Java: import java.util.List;
来源：http://hz.daxiang520.top/gtogxpkurm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.smart0.xyz/gtqungtivm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtoumbwlpq.html

C#:   using System.Text;
来源：http://hz.yueranfly.top/gtwcrtqzdc.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtjhqpemvx.html

Py:   (lambda: print("run"))()
来源：http://hz.chenzaomai.com/gtcotjjryv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangkeji.top/gtsrjedorr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtpozhxvpk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtbcpvegja.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tian-w.cn/gtywocdsvk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtjbjioxua.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtdumiabwg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gteoqwzctn.html

[C13] 类型声明 / 类型注解
来源：http://hz.xingfuxueyuan.xyz/gtjmtryorr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuanzhike.top/gtwkfmilcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtoaeibqgi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtqikwdezk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtskcudgsd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtdkdzrjcq.html

Go:   func add(a, b int) int
来源：http://hz.cucudq.cn/gtucvosnjw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtflpsqclo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtewrbenak.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtkqpbuegq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnqzz.top/gtfvgjefqe.html

PHP:  // 无泛型
来源：http://hz.zycfv.cn/gthedgdiyv.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtwggihoms.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtlbgpjhml.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gteekctupl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yueranfly.top/gtytipiqps.html

Ruby: # 无泛型
来源：http://hz.52xcode.cn/gtiirpkymn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtvvitivyu.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gthbpopggb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtsrxhqqzo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xylfe.cn/gtfdkufabc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtsmjaefti.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtlrqffgla.html

Java: // 无解构
来源：http://hz.316326.xyz/gtqferygvq.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gtwhxtdagr.html

Ruby: a, b = pair
来源：http://hz.chenzaomai.com/gtmvwtmcvu.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtlwwyxiiz.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtsauguhok.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtfsmtqkug.html

PHP:  // 无重载
来源：http://hz.snrcjt.cn/gtyswjxkfy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.mhx1999.top/gtqwbjllnr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtwyavfyaf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtqaaqwkeu.html

Go:   // 无重载：用不同函数名
来源：http://hz.zycfv.cn/gtmruwilto.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhengqikj.top/gticprzdln.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tanke756.top/gttkkwbinu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtzrhqftap.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtarhegiqz.html

================================================================================
来源：http://hz.52xcode.cn/gtpvqvgwur.html

[D01] 创建数组 / 列表
来源：http://hz.sweek.top/gtnfqgdavq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnqzz.top/gthlfdcajo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtrzebwukh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gthkbmkbgh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.316326.xyz/gtnxxluukh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.316326.xyz/gteywozbbh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtlwlcchgz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtghiljugb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sysykeji.top/gtwffnkkxd.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtxfblmhvh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtdxbpighn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtenhkdkmk.html

JS:   arr.push(4);
来源：http://hz.yuxming.cn/gtnglxcbwc.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtzoghpyps.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtsznmotaj.html

Go:   arr = append(arr, 4)
来源：http://hz.daxiang520.top/gtfyxkazro.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtvqnkmzhv.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gtbuqolmhb.html

[D03] 在指定位置插入元素
来源：http://hz.yj202588.top/gtvgtymehq.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtpclkddet.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtormobkac.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258888.top/gtuxwzefls.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtrveyjhtr.html

Java: list.add(0, 0);
来源：http://hz.shzxlz.cn/gtxahcwkod.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtffqnqbqb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gtxialfhme.html

C#:   list.Insert(0, 0);
来源：http://hz.yvedp.cn/gtxkpapxyn.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtdiywlqmm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhiwuduotai.top/gtonjbvgth.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenjidiqi.icu/gtfqymamob.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtczuhieep.html

TS:   arr.splice(0, 1);
来源：http://hz.shzxlz.cn/gtfzbqgxvi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jianghu66.top/gthxpsknqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fengsongda.top/gtagxteynr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtseokifgi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sxryk.cn/gtcdfbjxzr.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtfsmfkwiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtikirrdtf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtcndxizhj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtqvorrfat.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtajuycshv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtptibkfky.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zycfv.cn/gtksrupfsb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gthkggihrq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtjcsulkpa.html

[D06] 数组长度
来源：http://hz.pycfn.com/gthpltbydz.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtpffewton.html

PHP:  count($arr);
来源：http://hz.kuanghao11.cn/gtzuimttes.html

JS:   arr.length
来源：http://hz.gogol.net.cn/gtkbouyafk.html

TS:   arr.length
来源：http://hz.c1oappe.top/gtseagaisz.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtcuwzlswo.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtjyftnqec.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gtpokgtigg.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gteytabjjn.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gthedeyywz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtoyjpousg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtgwpmahet.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtpjqkxjnw.html

TS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtlcbycuor.html

Java: list.subList(1, 4);
来源：http://hz.ehwqpu.com/gtqbwdsrve.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gtwyqsxmjg.html

Ruby: arr[1, 3]
来源：http://hz.nanxuanxn.top/gtrtjkkigs.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtcehrrvzs.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtbwacabxl.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtulgvdvzd.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtgymwzujb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.meibo888.top/gtukejyygg.html

TS:   [...a, ...b];
来源：http://hz.smart0.xyz/gtloppncyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jiagoushi.top/gtjgubmufn.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtdvrffdkw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gtsxhohkyy.html

C#:   a.Concat(b).ToList()
来源：http://hz.ppjwa.cn/gtyeasucbt.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtcwawiyhc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtcaoyjqos.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtjrsamtpu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtgzhaiyjr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gthcouxgnm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtqdgvsord.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtarwakrek.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtzlmfxnys.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtuufbyjdf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtlftkjnwv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenzaomai.com/gtxjmiblka.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtldwcwztl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtzkmnopgv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtypkiujio.html


<!-- 参考信息 -->