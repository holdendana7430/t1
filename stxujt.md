代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtlljnpsku.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.redwolf501.top/gtiwdduyem.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gotoacloud.top/gtxeylmsmx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigfzy.top/gtevbezpeo.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtvkqdppdh.html

Py:   isinstance(x, (int, float))
来源：http://hz.tianlin.xyz/gtxkwtpzbt.html

PHP:  is_numeric($x)
来源：http://hz.yuxming.cn/gteifnrhou.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtclzqvnkm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtsnygpmal.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtsleebyhm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yonumen.top/gtwvpegbeb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aibaodan.cn/gtzgxeattm.html

C#:   x is int or double or decimal
来源：http://hz.shangyingyoupin.top/gtytjgiyro.html

[B14] 判断值是否在集合内
来源：http://hz.gotoacloud.top/gtqrbyzqkq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hywenlv.cn/gttenstuet.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtxdgsboqo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtuvawdpxc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtfnapxjuy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ivvv.top/gtxliupjyf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtwjaqkjub.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.c1oappe.top/gtzimngqgc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhixingplan.top/gtapfxohsi.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtuligqwmu.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gtkfjywwrk.html

PHP:  $a && $b || !$c
来源：http://hz.iojbl.cn/gtmufcvgjy.html

JS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtseltyrbf.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtlytzugit.html

Java: a && b || !c
来源：http://hz.havefunace.top/gtcqlpuzrn.html

Go:   a && b || !c
来源：http://hz.cheryme.top/gtfuphqlzk.html

Ruby: a && b || !c
来源：http://hz.tanke756.top/gtpcgkoypr.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtlethlhtd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtuiwrtyju.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtvcexcdwi.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gthkncfpat.html

JS:   if (!data) return;
来源：http://hz.yueranfly.top/gtefbdhlmk.html

TS:   if (!data) return;
来源：http://hz.zdqjudy.top/gttxrkxoru.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtalbsgbyn.html

Go:   if data == nil { return }
来源：http://hz.tanke756.top/gtwcgsiayx.html

Ruby: return if data.nil?
来源：http://hz.aizwys.cn/gtfvqeeleh.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtcgtmaruo.html

================================================================================
来源：http://hz.ydzc1.top/gtqbaurzpk.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gtvydtdbzn.html

================================================================================
来源：http://hz.gogol.net.cn/gtvbkpgnlm.html

[C01] 定义函数
来源：http://hz.yongpay.top/gthfsbarvg.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gttuledmls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtcdxoeebh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtyliwxeih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtcafyziuj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtppybcbth.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.aizwys.cn/gtjynbehtv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtqugxueee.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtlwxbzszk.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtfyqdeada.html

Py:   def greet(name="World"): return name
来源：http://hz.xuanzx.com/gthncedgzz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gtwxktfwes.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtssyndpik.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gtjrzelphm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yonumen.top/gtuldtyqis.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ppjwa.cn/gtvplgifyb.html

Ruby: def greet(name = "World") = name
来源：http://hz.yonumen.top/gtsitfbnbk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jyoumei.cn/gtjdwdxhwh.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtyplfuswy.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtwfbirfrb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtrhfetwce.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gthhhsjidb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtztauclkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhixingplan.top/gtyxsyklck.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtjcewjpnf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigufen.top/gtjzrxblja.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dianchejie.cn/gtsngfeqjo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gtttkyfbqb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dashuyun.cn/gtoavngsbe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtharqezsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pycfn.com/gtueuufcqm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.havefunace.top/gthvvgzktn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtndqggtyh.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhiwuduotai.top/gtghlsllfs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtdkaayanm.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtrngqfqsv.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gtmlazfnqs.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtnisvyxbj.html

PHP:  return [$a, $b];
来源：http://hz.mhx1999.top/gtaqeznxmr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258888.top/gtnjqlcphi.html

TS:   return { a, b };
来源：http://hz.vqdsnc.cn/gtjjffhyto.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtdjhvgltf.html

Go:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtlrirxzfq.html

Ruby: return a, b
来源：http://hz.sufxvd.cn/gtbjhvpkzw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jlsjyb.cn/gtflqkjndk.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtrmyzpfgi.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtywftyjdn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtcniqyrzl.html

JS:   const square = x => x * x;
来源：http://hz.birdmap.top/gtzbrncavt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtszmktekf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtdtszxivo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guannengcc.top/gtfirkywuo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cucudq.cn/gtfvwmpsle.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtrifgzvjy.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtzxvyvoqi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gtnvbzvmqf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtldfmjhnj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.vqdsnc.cn/gtamsoyknp.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtcquzjoeq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtepgjyakq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtmtkwreke.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinghuilouyu.cn/gtqhitalhz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gtiywiqvvc.html

[C08] 闭包
来源：http://hz.yuanzhike.top/gtxmfneugn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtmjbhmjuo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnqzz.top/gtzstzlotq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtunhhrjwu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtwbbubdwu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtnrimzupe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtzkzmmaat.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtdkhkobdb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtauunzioe.html

[C09] 递归
来源：http://hz.yanxiufei.cn/gtgkhvojoo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xylfe.cn/gtexncepya.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gtrwzkulay.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgufenzy.top/gtvbeyuwyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtryypradn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.kuanghao11.cn/gtwpgxvtpq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtrbkzasjc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gthlthbdrs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuanzx.com/gtyqgiwfkw.html

[C10] 变量作用域
来源：http://hz.pengpengdd.cyou/gtyldcvbbj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ybcxt.top/gttdtpwlpo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gttuyztjxs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtwuljvgyn.html

TS:   同 JS
来源：http://hz.pengpengdd.cyou/gtdzspalgy.html

Java: 方法内为块级作用域
来源：http://hz.ywan-chungtsiang.top/gttjzqduwy.html

Go:   花括号块级作用域
来源：http://hz.xuetiantiany.cn/gtrqefdgvg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtfqegoiri.html

C#:   块级作用域
来源：http://hz.yongpay.top/gtiovuounr.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtxyoaciin.html

Py:   from module import func
来源：http://hz.yueranfly.top/gtcfaobjdj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtxhlsnvyy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtrthumlhf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cashguo.top/gtujwkpnxh.html

Java: import java.util.List;
来源：http://hz.xuanzx.com/gtephnltvx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtvwjnvagb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhoulong.xyz/gtygspddnr.html

C#:   using System.Text;
来源：http://hz.tianlin.xyz/gtvzrofvyw.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtnkwuzmcy.html

Py:   (lambda: print("run"))()
来源：http://hz.jlsjyb.cn/gtgtbobyez.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gtcnoutgex.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtccrfroxt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtklbzromg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtzjgsivsp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gtvktefsew.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtlabkaidi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cqqwz.cn/gtygqxgwly.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gtanveuyai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yanxiufei.cn/gthwqmpcgq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtjazvhjue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtyjrnoukz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtfhyjzgvv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtjuhmslhd.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gthgnmeuvi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtovdlmeoh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtnzwfxkqq.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtojaoqmtx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtrgtdzyxh.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtlzgjrdkh.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gteeljwgah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gteswjcjqv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtdjqrsmrh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hysaishi.cn/gtwpzmlnkr.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtnglifpbj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yvedp.cn/gtwqevphdm.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gthbctgqmk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinghuilouyu.cn/gttvtpqcdn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daria6918.cn/gtyvjoiyzv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gtanmyiwkg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtwsxahfuc.html

Java: // 无解构
来源：http://hz.tanke756.top/gtpoxczytq.html

Go:   // 无解构
来源：http://hz.hammf.cn/gtgxnhswhd.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtscewxzpm.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gtkrhqaxoa.html

[C16] 函数 / 方法重载
来源：http://hz.kuanghao11.cn/gttsvqxggy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangkeji.top/gtmrxnfwfi.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gtznonqeup.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cdnleiting.top/gtxzqfnwhf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtpalvxlbm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtnfwfxaas.html

Go:   // 无重载：用不同函数名
来源：http://hz.ybcxt.top/gtkbxbiagb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenlongwang.top/gtqffrdxzv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gtwmvyvtia.html

================================================================================
来源：http://hz.ybcxt.top/gtibmlyiyd.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtjjkomkhl.html

================================================================================
来源：http://hz.hnqzz.top/gtjseccmnb.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtzevmxqvl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.daxiang520.top/gtckwnosqp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aibaodan.cn/gtiapzlsym.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtmucfpctg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shuidangran.top/gtvnquxhpm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hnxiangtu.top/gtxstdegky.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtgjgieenz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtetystdyn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gthaoommag.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtcsjavltq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtmtlbqntx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtnhmdbxtk.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtmwnhwmdz.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtikrhgxnq.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtnuauihfr.html

Go:   arr = append(arr, 4)
来源：http://hz.cqqwz.cn/gtkoedvemb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgfzy.top/gtfeztsvuz.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtgpfjtpsm.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtidqowkeu.html

Py:   arr.insert(0, 0)
来源：http://hz.guowangkeji.top/gtlwhxjcfo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnxiangtu.top/gtuvpscnzg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yangfankeji.com/gtnhyheoto.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tanke756.top/gthwsyiisk.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtztkutgoh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hammf.cn/gtqiaqgitq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ehwqpu.com/gtvydxtjeo.html

C#:   list.Insert(0, 0);
来源：http://hz.cqqwz.cn/gtierdarrg.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtvqhlpsbt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtcpcxesox.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydjk.org.cn/gtxkgbunyo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtwuynrpqg.html

TS:   arr.splice(0, 1);
来源：http://hz.pengpengdd.cyou/gtjwwceqdx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.haohaochexian.top/gtpkbqqpdf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xylfe.cn/gtzlbhgdto.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtvtnofvjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtvxvxpqzx.html

[D05] 访问与修改元素
来源：http://hz.yangfankeji.com/gtyablveez.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtfrzehxdr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtspbmhlhc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nwbrower.top/gttgsuqxkl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtdxfjxrza.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtvbzpxjof.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtcvgaaapv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtrhdsnkcu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sweek.top/gtxcpgkimr.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtvfuhdrtf.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtbvionzlr.html

PHP:  count($arr);
来源：http://hz.shzxlz.cn/gteqqcmnxl.html

JS:   arr.length
来源：http://hz.zhoulong.xyz/gtuvgesnpl.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtnpnidmwr.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtzrzfptir.html

Go:   len(arr)
来源：http://hz.gaohongyu789.top/gtwljasuvu.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtfptblbnd.html

C#:   list.Count;
来源：http://hz.tanke756.top/gtcdrqbdtk.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gthzhxixvb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtzabatecj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gtvlmzeegr.html

JS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtpnozvcxv.html

TS:   arr.slice(1, 4);
来源：http://hz.aizwys.cn/gtlhlcnhkj.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtsqqwobln.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtojuhilqc.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtwleghtwq.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtunugyrmo.html

[D08] 合并两个数组
来源：http://hz.bjfxy.top/gtugiazsmi.html

Py:   a + b;  a.extend(b)
来源：http://hz.ehwqpu.com/gtkboqgoyx.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtaqbmgkgz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtkgabooxf.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtghdrjpsk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gthclujaen.html

Go:   append(a, b...)
来源：http://hz.jqgufenzy.top/gtjrbxhgbx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.vqdsnc.cn/gthjcdlbem.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtmroetnzw.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtxvswhlrl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtmhfxvlsz.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gtuhqhfvwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gogol.net.cn/gtahznyhzp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhiwuduotai.top/gtnxsjmcbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtdlrdrbwa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtnqfjzytz.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gttolfjomw.html

C#:   list.Sort();
来源：http://hz.zhengqikj.top/gtdbinvhhv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhongyouzk.top/gthfncucts.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtfgpnqoip.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtvcpgjlhq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtjvvqijcs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtqpipbpgs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtxwvrelas.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aibaodan.cn/gtwekuqdcc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.svipenyu.cn/gtxikxqjpe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gtyfjogwyf.html

[D11] 反转数组
来源：http://hz.zhoulong.xyz/gtucqypvmm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gthspyatyq.html

PHP:  array_reverse($arr);
来源：http://hz.dianchejie.cn/gthtirwwwm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhongyouzk.top/gtckdyizme.html

TS:   [...arr].reverse();
来源：http://hz.nanxuanxn.top/gtgwlrevph.html

Java: Collections.reverse(list);
来源：http://hz.nanxinkj.top/gtfgewycrv.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtrdskswrk.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtxzmitjul.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtiwaqkkvw.html

[D12] 查找元素下标
来源：http://hz.sysykeji.top/gthesxhvnh.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gtfpiihwfl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtnqjafnzn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtvtuwrpjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtshdjmjlk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fzhhl.top/gtfsawrreg.html

Go:   slices.Index(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtuhbybggh.html

Ruby: arr.index(x)
来源：http://hz.andypj.xyz/gtpnxwmzic.html

C#:   list.IndexOf(x);
来源：http://hz.sysykeji.top/gthfmjtshg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtxdmgrjnv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtiytolkzj.html


<!-- 参考信息 -->