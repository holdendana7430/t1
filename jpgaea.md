代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tanke756.top/gtpklornua.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhiwuduotai.top/gtpjakhtop.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cdnleiting.top/gtlbpjqyef.html

[B12] 跳出多层循环
来源：http://hz.jinghuilouyu.cn/gtxkcirbet.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtljqgmdlx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtempybssi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtuyjgljcz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtyjruhtob.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtbwjrqsyj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtvmdgsoyb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cucudq.cn/gtzviqtuoe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangdashe.top/gtkaismwie.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtrxzscjwn.html

Py:   isinstance(x, (int, float))
来源：http://hz.316326.xyz/gtwjtgrtrs.html

PHP:  is_numeric($x)
来源：http://hz.ybcxt.top/gtrwhesesd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtmcetpjex.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtptsscutn.html

Java: x instanceof Number
来源：http://hz.yj20258888.top/gtebiejhhv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuanzhike.top/gthgokmsjh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.guannengcc.top/gtdhcnpdyd.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtlxsztgmn.html

[B14] 判断值是否在集合内
来源：http://hz.dashuyun.cn/gtljdqekur.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tian-w.cn/gtvfmabdqz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtyattmrxw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtfqdnszeo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtygmoxbxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtagpvigiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj202588.top/gtqmdaixrb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuxming.cn/gtssimwrll.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ivvv.top/gtczjrqzww.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtfytypaxz.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtibkmjokl.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtiozhgxbr.html

JS:   a && b || !c
来源：http://hz.ivvv.top/gtvxmyueem.html

TS:   a && b || !c
来源：http://hz.zycfv.cn/gtitypbyft.html

Java: a && b || !c
来源：http://hz.aizwys.cn/gtdbtdrsfy.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gtbfrwhkvv.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gtkseyndgw.html

C#:   a && b || !c
来源：http://hz.svipenyu.cn/gtsxwgxykw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cucudq.cn/gtpqeptbov.html

Py:   if not data: return
来源：http://hz.ydzc1.top/gtmqoxomda.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtmszbisro.html

JS:   if (!data) return;
来源：http://hz.chenzaomai.com/gtseshqicl.html

TS:   if (!data) return;
来源：http://hz.iojbl.cn/gtlzzilegt.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtyrmdayzh.html

Go:   if data == nil { return }
来源：http://hz.guannengcc.top/gtzvordrta.html

Ruby: return if data.nil?
来源：http://hz.gotoacloud.top/gtwczmcndx.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtcplvmani.html

================================================================================
来源：http://hz.jiagoushi.top/gtmkvfiytv.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtzjiuveli.html

================================================================================
来源：http://hz.c1oappe.top/gtnmnxddrb.html

[C01] 定义函数
来源：http://hz.xuanzx.com/gtkaejinkm.html

Py:   def add(a, b): return a + b
来源：http://hz.zhijiandao.cn/gthlftbspe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtapgxeacg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtzrwzwjtw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtczjkwods.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtkjygfxcx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtheefymls.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj202588.top/gtnspbxjii.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gthntxjjxl.html

[C02] 默认参数
来源：http://hz.zdqjudy.top/gtzfdikywv.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gtnrnimgue.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtcgnrhivb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gttspkpnea.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtelfxhxkn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.0kj1m.cn/gtydxfofng.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.meibo888.top/gtraprzmpn.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtdgflssqi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtwqijhfee.html

[C03] 可变参数
来源：http://hz.tian-w.cn/gtotvlztte.html

Py:   def total(*args): return sum(args)
来源：http://hz.ppjwa.cn/gtugwafknj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.kuanghao11.cn/gtsunposys.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gteykwaqac.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gtadroohkw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtyptaniyv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtcdxazkld.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtdxswepbd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtyronrzeo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtgjlmduka.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtslxoovul.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.mhx1999.top/gtxvtevkmh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtqfpuqzpp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtylcoigol.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj202588.top/gtokppryyh.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtxdhrzkmj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtvqoakyud.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtvhxxlnvd.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gtnjbiedkm.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtbefvxtbq.html

PHP:  return [$a, $b];
来源：http://hz.vqdsnc.cn/gtokekjrip.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yangfankeji.com/gtsowoycxm.html

TS:   return { a, b };
来源：http://hz.ehwqpu.com/gthxofhzqe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtgfgyadnc.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtchydievk.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtikzyxhok.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gtenijjpuv.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtxswfrygx.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtoagnelhz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinqigufen.top/gtkrlyrivx.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtharesgwi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtwwhandin.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cashguo.top/gtjgklkqcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yueranfly.top/gttvfyoxcw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtfxxwexza.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shuidangran.top/gtzltcuwge.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtkzvzyhqe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.9152youxi.cn/gtumzofeas.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sysykeji.top/gthztbtnfm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtxzcidsru.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtttwrmjjs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.vqdsnc.cn/gtwnrpgdbz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigfzy.top/gthzbxgtdp.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuxming.cn/gtusjjywhe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sysykeji.top/gtqhnizqpw.html

[C08] 闭包
来源：http://hz.dashuyun.cn/gtboalmjay.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtyepgijki.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtphlnalyf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtcopxesla.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtiowqsrzs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangshuangyany.cn/gtaxmfgxbm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gtysuenmrs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigufen.top/gtzzzamgqr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtwarzrgwu.html

[C09] 递归
来源：http://hz.ppjwa.cn/gtyagseoli.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtruxfwpdx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtexyhctiz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtllprpyuk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtrhlsnhiy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tianlin.xyz/gtebidzmlr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtrbuaszww.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtufzcabze.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuanzx.com/gtfhsjxenu.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gtfeubzrim.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jlsjyb.cn/gtcjfgiljk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydzc1.top/gttfhhkxzu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sxryk.cn/gtbbfxanot.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtirkyomfn.html

Java: 方法内为块级作用域
来源：http://hz.hfpthk.cn/gtkmcvbilm.html

Go:   花括号块级作用域
来源：http://hz.hongshengwenyu.top/gtdreezqou.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258.top/gtfdrboxca.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtbrdfgntg.html

[C11] 模块导入与导出
来源：http://hz.hnxiangtu.top/gtohenbdma.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtmggkhhgo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtjdrdmmgp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtwcnazbdm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtuqbygdjl.html

Java: import java.util.List;
来源：http://hz.zhiwuduotai.top/gtzcxocezm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.vqdsnc.cn/gtqhpscnqd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jiagoushi.top/gtecnajdug.html

C#:   using System.Text;
来源：http://hz.jinyuanbaomall.cn/gtcmaqqhhj.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigfzy.top/gtnvfxcghn.html

Py:   (lambda: print("run"))()
来源：http://hz.zhijiandao.cn/gtrwnagaur.html

PHP:  (function () { echo "run"; })();
来源：http://hz.andypj.xyz/gtzbkuwppu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gthxphthgq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtzfaxnyel.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gtarxiqyjn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gtlbmtvjra.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtgmbbdzeo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtkebrjxup.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gtaevtrexq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtaxdacpyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtodsjegsh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.meibo888.top/gtbtyieivc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtkwvxehmv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gterlbszyn.html

Go:   func add(a, b int) int
来源：http://hz.mhx1999.top/gtkzkzpboa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xinyue.icu/gtljshpuah.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhongyouzk.top/gtwdajuuxq.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtxkhgsatm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.0kj1m.cn/gthezchend.html

PHP:  // 无泛型
来源：http://hz.iojbl.cn/gtkxmwgatk.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gtpvaqfrpn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yvedp.cn/gthstulfrs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtrdwoiktz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gtnmdfzyqr.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtcbqmwfqv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuetiantiany.cn/gtcbgzisub.html

[C15] 解构 / 展开参数
来源：http://hz.cdnleiting.top/gttfvoxdtx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yueranfly.top/gtgctpmzmx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtxqfvnfki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtqeidppse.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtttiekiwo.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtkkofbhox.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtvbgxuexq.html

Ruby: a, b = pair
来源：http://hz.zhoulong.xyz/gtcszanugx.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gthgsououf.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtxncvegiv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtgjgotwsn.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtuykmihdx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtpkisfkbg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtxjdsvqwm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gtmbnbbdxt.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtdoorooao.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhongyouzk.top/gtgdbmsyth.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tianlin.xyz/gthpqskuzy.html

================================================================================
来源：http://hz.pycfn.com/gtskuquamb.html

D. 数组 / 列表 / 集合
来源：http://hz.hammf.cn/gtuxbenlgf.html

================================================================================
来源：http://hz.yueranfly.top/gtinrvgyph.html

[D01] 创建数组 / 列表
来源：http://hz.quarkkingdee.top/gtujlwvdcz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtdggayqno.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuanzx.com/gthhlfxsps.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtdnbvxtfi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gtqnbjmmya.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtwkyuqdsj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtrifajkik.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhaomingkeji.xyz/gtlmvlkilp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtuwdkbhyx.html

[D02] 追加元素到末尾
来源：http://hz.jinghuilouyu.cn/gtotgyquxa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.vqdsnc.cn/gtizouhydy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtcujammnc.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtqqfvucjm.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtajahzuiz.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gtmvsdxrpf.html

Go:   arr = append(arr, 4)
来源：http://hz.ybcxt.top/gtnaeupgmj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtntarbivb.html

C#:   list.Add(4);
来源：http://hz.xuetiantiany.cn/gtgtxninlz.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtuenbrxrf.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtkdxrtqvp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinyuanbaomall.cn/gtnhqrcqij.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigufen.top/gtgberuatr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtcqgrxpso.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gthovbhwtv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuetiantiany.cn/gtirgetlll.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xingfuxueyuan.xyz/gtpujjbaov.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gtxltknttj.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtfgjevutn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nwbrower.top/gtkgxudryi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydjk.org.cn/gtczjqoycd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtullxdezp.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtrimcqyql.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtokorqygi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtcrwitfny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtqqcmyxnf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtljvlcpxs.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gthdwbxbnq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtysepduka.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtgwiqidse.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daria6918.cn/gtwftgxtwy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gthzmrzmam.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtzkxhbjqk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtemuvjomm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtszgofwxm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnxiangtu.top/gtnirmbcrv.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtqagwsdqq.html

Py:   len(arr)
来源：http://hz.0kj1m.cn/gtszhapgvd.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtmxdkebcq.html

JS:   arr.length
来源：http://hz.nwbrower.top/gtpqhjpvxu.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtibtnqejk.html

Java: list.size();
来源：http://hz.chenzaomai.com/gtyapgjliu.html

Go:   len(arr)
来源：http://hz.jqgufenzy.top/gttibdumnk.html

Ruby: arr.length; arr.size
来源：http://hz.cashguo.top/gtsezvhhmx.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtozfupsjn.html

[D07] 切片 / 取子数组
来源：http://hz.sxryk.cn/gtxpqseibm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sxryk.cn/gtecndnvfj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtpnczbehg.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtbcswqgyn.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtcebjrlqv.html

Java: list.subList(1, 4);
来源：http://hz.sysykeji.top/gtpaswwxdm.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtsoaysyyz.html

Ruby: arr[1, 3]
来源：http://hz.yangfankeji.com/gttfkmpzth.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtsfslkpvg.html

[D08] 合并两个数组
来源：http://hz.yanxiufei.cn/gtqyqkheyy.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnxiangtu.top/gtqhqwewgq.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtdqninehs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtsofeyrma.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtgumzglba.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guannengcc.top/gtewrrhqnz.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtoojigrix.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtfufcdtqm.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtjymlnnmj.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtbxcqxeiw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtsdckyydo.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtwrrhptiy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtpebrybev.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sysykeji.top/gtwcsnxbxs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtpwvidhri.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.316326.xyz/gtsunxmfza.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtgqnnpbms.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gtkaspqchm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guannengcc.top/gtlskyiitb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xziqi.cn/gttlmxesxa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtdgyrlush.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtvpgsrxgl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtxblshzvg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hywenlv.cn/gtfrfcghki.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.daria6918.cn/gtotekqilj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gaohongyu789.top/gtpqyfrepe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydzc1.top/gtwaopwary.html

[D11] 反转数组
来源：http://hz.yangfankeji.com/gttjchdhmm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.bjfxy.top/gttgkxmfdf.html

PHP:  array_reverse($arr);
来源：http://hz.tanke756.top/gthsgblmui.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtamiwxpzs.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtrmvvykiw.html

Java: Collections.reverse(list);
来源：http://hz.cashguo.top/gtrwzrkdtw.html

Go:   slices.Reverse(arr)
来源：http://hz.cdnleiting.top/gtpcyetdwx.html

Ruby: arr.reverse
来源：http://hz.zhiwuduotai.top/gtauyrfwvy.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtsltdrezq.html

[D12] 查找元素下标
来源：http://hz.hfpthk.cn/gthyfotyas.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gteuxufmzu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtpkomkspq.html


<!-- 参考信息 -->