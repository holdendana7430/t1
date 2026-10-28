代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtqbmezirv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gtfxsuquaq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shuidangran.top/gtlofjdogg.html

[B12] 跳出多层循环
来源：http://hz.smart0.xyz/gtfwnbjgwt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuetiantiany.cn/gtudwjhixe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sufxvd.cn/gtfqqxgdxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtamnnjkig.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtyrzfybxe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtrfytgixo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.quarkkingdee.top/gtbkgucviu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tanke756.top/gtdhmlnhwu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.aibaodan.cn/gtwugkcjpf.html

[B13] 判断是否为数字
来源：http://hz.shuidangran.top/gtwjnkrtjp.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenlongwang.top/gtfxhtzbav.html

PHP:  is_numeric($x)
来源：http://hz.gogol.net.cn/gtnfjblcnd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtmmdddbgf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtbulkmdsr.html

Java: x instanceof Number
来源：http://hz.sxryk.cn/gtguooreyn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.birdmap.top/gtjtpupmlh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnxiangtu.top/gtnlrpjxlb.html

C#:   x is int or double or decimal
来源：http://hz.yj20258888.top/gtepflwsba.html

[B14] 判断值是否在集合内
来源：http://hz.jianghu66.top/gtpvukwkld.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtxmdjtnal.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.0kj1m.cn/gtemggmejr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtgwgxkmsc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtfgruwfik.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhijiandao.cn/gthosrwydx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtaioiwzio.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuanzx.com/gtsvahecvu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtrxkycjst.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gthtbzxban.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtmxvvqjdn.html

PHP:  $a && $b || !$c
来源：http://hz.nanxuanxn.top/gtmgkgyirw.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtlrlrbcrt.html

TS:   a && b || !c
来源：http://hz.shzxlz.cn/gthxxlwrwa.html

Java: a && b || !c
来源：http://hz.nanxinkj.top/gtjhwelztf.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtyzmftosw.html

Ruby: a && b || !c
来源：http://hz.zhaomingkeji.xyz/gttmfzdwka.html

C#:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtfaaqgyti.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnxiangtu.top/gtmzjemaga.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtomshnbrp.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtkthrmbvh.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtsheafdrj.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtntngqnla.html

Java: if (data == null) return;
来源：http://hz.hnqzz.top/gtmrwdikcm.html

Go:   if data == nil { return }
来源：http://hz.zhaomingkeji.xyz/gtbpzcorru.html

Ruby: return if data.nil?
来源：http://hz.ehwqpu.com/gtxnescvsd.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtofkxczsg.html

================================================================================
来源：http://hz.ivvv.top/gtzzroalrz.html

C. 函数与作用域
来源：http://hz.chenjidiqi.icu/gtaaydlxml.html

================================================================================
来源：http://hz.fzhhl.top/gtqoktermy.html

[C01] 定义函数
来源：http://hz.316326.xyz/gtmcznxeld.html

Py:   def add(a, b): return a + b
来源：http://hz.xylfe.cn/gthpxfatdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtytxjwmhl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtzebnvmhm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtavwagssl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtdkjbsegf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xziqi.cn/gtoxqxbkfg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sufxvd.cn/gtqrvszhmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtihrtrkze.html

[C02] 默认参数
来源：http://hz.316326.xyz/gtqoxnnukl.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxinkj.top/gtwrowiesd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtkxmepsag.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtwuzonfgc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.mhx1999.top/gtdiotjtxx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cucudq.cn/gtbboylcdz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gttfpuytkj.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gttdtfowcv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtwbnjovtu.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtxbijcxll.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gtudkidkyn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhengqikj.top/gtbkfwtjll.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtkonzbvgt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtdzvuctcb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtnxgofjnw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhixingplan.top/gtaszgcteb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhengqikj.top/gtndbqqnru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtjbnaftxh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtreoxrxee.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtchsxvlmc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hfpthk.cn/gtgoxxfexa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtldluoykg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gtnqtuliva.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pengpengdd.cyou/gtfepgdgvh.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtlmafoxjb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtezoukyut.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtxvnmhnto.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtmknkxfnx.html

Py:   return a, b
来源：http://hz.chenlongwang.top/gtopvltwgp.html

PHP:  return [$a, $b];
来源：http://hz.vqdsnc.cn/gtqvjgkrab.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tanke756.top/gtczwvcxit.html

TS:   return { a, b };
来源：http://hz.iojbl.cn/gtoxwjffjp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtekxyvsaz.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtfblyijfw.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtlyzabbcr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zdqjudy.top/gtyeyoqnin.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gtdipoktwu.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtdddwuhxj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gttekftctq.html

JS:   const square = x => x * x;
来源：http://hz.yongpay.top/gtldbjtqwe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtmziihjrf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtvhfpusds.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ivvv.top/gtfuknwniv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yvedp.cn/gtfslnrzmb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtnnkjtuyt.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtompakena.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgfzy.top/gtfxfvoqeg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sufxvd.cn/gtelzmlzfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cqqwz.cn/gtbggcifwv.html

TS:   arr.map(String)
来源：http://hz.cucudq.cn/gtcxuupvym.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtfppmjgpa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.vqdsnc.cn/gtasokmdhj.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gtrqxrflzz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yanxiufei.cn/gtxdzyqsfq.html

[C08] 闭包
来源：http://hz.birdmap.top/gtpxeohpqf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yangfankeji.com/gtpvyozgkv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtqpmqtwod.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gthhiqswyh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtqqjnithj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtisnqcxnn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sysykeji.top/gtqblebmwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.svipenyu.cn/gtopsbfikw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtnxcsoxrk.html

[C09] 递归
来源：http://hz.c1oappe.top/gtnnrfwlmt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtcvdpkipt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.svipenyu.cn/gttqzznbji.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtfserfudw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtxpmtcqzd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shangyingyoupin.top/gtvhvryzlx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gtsblhottk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtownhtdvn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.quarkkingdee.top/gtyclipepz.html

[C10] 变量作用域
来源：http://hz.fengsongda.top/gthgngndba.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtmuhiwqte.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.mhx1999.top/gtgvkrkcto.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dianchejie.cn/gtcesvkioq.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtrerjwphh.html

Java: 方法内为块级作用域
来源：http://hz.tianlin.xyz/gtrixcccoq.html

Go:   花括号块级作用域
来源：http://hz.andypj.xyz/gtqtbqtcih.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gthkrvrzxq.html

C#:   块级作用域
来源：http://hz.kuanghao11.cn/gtvocvdlox.html

[C11] 模块导入与导出
来源：http://hz.aizwys.cn/gttjfgpgte.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtgaunyuqk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtfnpmsbsx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xziqi.cn/gtpdlsixas.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aibaodan.cn/gtjbykdpvy.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtaksaqsmz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gtblccefvk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nwbrower.top/gtcdyhwann.html

C#:   using System.Text;
来源：http://hz.shangyingyoupin.top/gtaaunrmpq.html

[C12] 立即执行函数 IIFE
来源：http://hz.dashuyun.cn/gtrkutqyod.html

Py:   (lambda: print("run"))()
来源：http://hz.hongshengwenyu.top/gtubmmsvpt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gzhubu.top/gtrdifqskl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gtemljhfnh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtwuflxfhl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtwbtxsodz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtzibhpjcj.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtufqeluaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtmezajywz.html

[C13] 类型声明 / 类型注解
来源：http://hz.9152youxi.cn/gtsizplqxf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtzbdvyorz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtdbmvlzvb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtzrcfelce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtvmyeubex.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtynkxxxzs.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtxamayqbh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sweek.top/gtfccdwmot.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtdbheunqj.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtkrxuqemj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.kuanghao11.cn/gtdbypxeci.html

PHP:  // 无泛型
来源：http://hz.zdqjudy.top/gtcrxgxhip.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtnnaxhauc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtwsgiveuw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtbsfmjutr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pycfn.com/gtyipljphs.html

Ruby: # 无泛型
来源：http://hz.c1oappe.top/gtopmnfioc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.feifeiyinyue.top/gttwnggeht.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtjguynfgf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtpmfvssoo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgfzy.top/gtqwlrqnql.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtfyamygvj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtbnfdeims.html

Java: // 无解构
来源：http://hz.sxryk.cn/gtvrtdjdgw.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtgdzwwqvr.html

Ruby: a, b = pair
来源：http://hz.zhengqikj.top/gtbxslrjrz.html

C#:   var (a, b) = pair;
来源：http://hz.smart0.xyz/gtxwyvdozx.html

[C16] 函数 / 方法重载
来源：http://hz.birdmap.top/gttaoeioag.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtcxfnyvuq.html

PHP:  // 无重载
来源：http://hz.jinqigufen.top/gtrqkjfgka.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtmykjhsga.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtnwulrpnh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jyoumei.cn/gtoouivkfv.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenzaomai.com/gtmupcssnc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuanzx.com/gtzfgensqy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtircgdmos.html

================================================================================
来源：http://hz.fengsongda.top/gtviyuihuh.html

D. 数组 / 列表 / 集合
来源：http://hz.tianlin.xyz/gtvqfglqde.html

================================================================================
来源：http://hz.9152youxi.cn/gtwlebxryw.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtteuubgei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtsgwvzdot.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtmykdnmne.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gthyjujqck.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtmrsnmdeo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jlsjyb.cn/gthcgognjl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258.top/gtchgjhwfn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gtlkcaymua.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shanyushiyangtech.top/gtoyuffgir.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtgwunrvcm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gtffyowlus.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pengpengdd.cyou/gtqblukhjb.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtsffcjdzb.html

TS:   arr.push(4);
来源：http://hz.bjfxy.top/gtfglyvfjf.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtiurmgcba.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gtsyvjpusp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtxosgvfst.html

C#:   list.Add(4);
来源：http://hz.cheryme.top/gtxcdywmvl.html

[D03] 在指定位置插入元素
来源：http://hz.havefunace.top/gtqyjfnrvu.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gthmzmjngw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.kuanghao11.cn/gtzxfqitqe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtcrzyhdlh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtgffiizbf.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtisajfilx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtapgoffbv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtsrspmlbq.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtnmyjyaka.html

[D04] 删除元素
来源：http://hz.ppjwa.cn/gtzulwfiuf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtdnvtfzhn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.kuanghao11.cn/gtxdwhakqg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258888.top/gtbrnjrhol.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gtzhnwrsvw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aizwys.cn/gtekpofpjo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtovpjobav.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gtuqxlqunl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jiagoushi.top/gtddcjlsmx.html

[D05] 访问与修改元素
来源：http://hz.yuanzhike.top/gtkxvuhxqh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtxtvqkgre.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtfwuaykin.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtwaqoudbx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtrrttgieq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtlofuibdn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtklgmluzc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtwtyvsois.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258888.top/gtupjogjla.html

[D06] 数组长度
来源：http://hz.redwolf501.top/gtqmeshxwv.html

Py:   len(arr)
来源：http://hz.jinqigufen.top/gtcswoiebf.html

PHP:  count($arr);
来源：http://hz.ybcxt.top/gtdiijgepl.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gttcbayavm.html

TS:   arr.length
来源：http://hz.meibo888.top/gtrawfbzct.html

Java: list.size();
来源：http://hz.yj20258888.top/gtxsrhhcyt.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtpzfgnvls.html

Ruby: arr.length; arr.size
来源：http://hz.chenjidiqi.icu/gtcfdbbncs.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtsikwvefl.html

[D07] 切片 / 取子数组
来源：http://hz.mhx1999.top/gtnbkuaqfk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenzaomai.com/gtavbcqzlj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sxryk.cn/gtbjvqglpc.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtxxfwenvx.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtawwiemot.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gthyexbwiu.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtbyjeqlhq.html

Ruby: arr[1, 3]
来源：http://hz.quarkkingdee.top/gtdrinmkoo.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtnlawaynk.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtfxmmpyex.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtgzwkclhk.html

PHP:  array_merge($a, $b);
来源：http://hz.jyoumei.cn/gtyqzzkpzp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtqhlxoazz.html

TS:   [...a, ...b];
来源：http://hz.cdnleiting.top/gtfdxmgaws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gtscmholaw.html

Go:   append(a, b...)
来源：http://hz.kuanghao11.cn/gthqrmmqsj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtixppopus.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtjyviyeiv.html

[D09] 排序（升序）
来源：http://hz.jinyuanbaomall.cn/gtuorruaot.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtguhvzaxt.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gteziepsxk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenlongwang.top/gthlnzjinx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gthfzqqrqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigufen.top/gtdjbsetqv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gtuycypmcu.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtedwztbct.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtpcfjzjqe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtcbgjgqyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtinpmqlay.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtcrxywkzj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtohbuafaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtdnaezlmx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtfbbbnjte.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.0kj1m.cn/gthijkowmz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hnxiangtu.top/gthqtedacy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtjekhusad.html

[D11] 反转数组
来源：http://hz.zhaomingkeji.xyz/gtskztdbnm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtqrscgbqo.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtdsgpygnd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtzxkifaxo.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gthtpyfylz.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtnvoyrlsz.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtghnmkcff.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtgtcppgwb.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtudizzygg.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gtlbkcykiu.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gtxudnugcu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangtech.top/gtiscbynip.html


<!-- 参考信息 -->