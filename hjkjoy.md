代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xylfe.cn/gtnglxgrkc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.fengsongda.top/gtxiholoqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtpqdqhanu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtkjuuqvue.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtcdsqwjwn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.316326.xyz/gtajzbwsvi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.smart0.xyz/gthzuwhtnz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtwrqhpyqx.html

[B13] 判断是否为数字
来源：http://hz.gzhubu.top/gtddqgudsp.html

Py:   isinstance(x, (int, float))
来源：http://hz.yonumen.top/gtcpdttzkt.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gttqdzqorh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtezilutjx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtnmuocxgh.html

Java: x instanceof Number
来源：http://hz.svipenyu.cn/gtpyusatyw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhengqikj.top/gtmbnferli.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tanke756.top/gtwlylwtqg.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtffaqpcma.html

[B14] 判断值是否在集合内
来源：http://hz.meibo888.top/gtgtrzvyiw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gtpkdtngwa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.smart0.xyz/gteqyhzkna.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtpftyqvzq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gthctinwzi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hywenlv.cn/gtitjowniz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gogol.net.cn/gtdeivhrrd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gthpyujxto.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtnjtxqpzc.html

[B15] 布尔运算与取反
来源：http://hz.jianghu66.top/gtxokjhnku.html

Py:   a and b or not c
来源：http://hz.hnqzz.top/gtbkawqltm.html

PHP:  $a && $b || !$c
来源：http://hz.gzhubu.top/gtlfglwohn.html

JS:   a && b || !c
来源：http://hz.jinqigufen.top/gtndjporai.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtsphgcmhj.html

Java: a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtrmcbcszk.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtkipgwdqv.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtmfirabad.html

C#:   a && b || !c
来源：http://hz.pycfn.com/gtycqehhft.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.pycfn.com/gtwetvhxhv.html

Py:   if not data: return
来源：http://hz.guowangkeji.top/gtxxytxjtn.html

PHP:  if (!$data) { return; }
来源：http://hz.yuxming.cn/gtpyubfwif.html

JS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtncfcuziv.html

TS:   if (!data) return;
来源：http://hz.jqgfzy.top/gtkjplsitq.html

Java: if (data == null) return;
来源：http://hz.xuanzx.com/gtipvmfmhd.html

Go:   if data == nil { return }
来源：http://hz.sufxvd.cn/gtjklstbql.html

Ruby: return if data.nil?
来源：http://hz.daxiang520.top/gtukuyijgm.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtsiqxarrm.html

================================================================================
来源：http://hz.zycfv.cn/gtliiecpqn.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtwefuktps.html

================================================================================
来源：http://hz.svipenyu.cn/gtxagykqjp.html

[C01] 定义函数
来源：http://hz.hnqzz.top/gtzfpxdkou.html

Py:   def add(a, b): return a + b
来源：http://hz.yvedp.cn/gtoksuworz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtiwnhkznx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gtwejhpmcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtobvgdhad.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gteeyywsok.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.birdmap.top/gtvcnmruxl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtwdvkravz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtcprwvnjm.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtujbmslkb.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxinkj.top/gtbnogpyhr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shangyingyoupin.top/gtkbieotnb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gotoacloud.top/gtfmsbrfzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shzxlz.cn/gtzjapiowm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cdnleiting.top/gtxzxaqrzf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtqpydjjwe.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtwszcdgxq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cqqwz.cn/gtrzyprtla.html

[C03] 可变参数
来源：http://hz.redwolf501.top/gtraxgpdwx.html

Py:   def total(*args): return sum(args)
来源：http://hz.sufxvd.cn/gtsexwmsye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtohucjpxe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtcofktada.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtwvvcaknj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yangfankeji.com/gtdirpcgra.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtbzxbosse.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.bjfxy.top/gtktdvsoyw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtwrhoncbb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.9152youxi.cn/gthopfikam.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dashuyun.cn/gtxnswujbl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtxccxlgva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtxhwgeffi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sxryk.cn/gtrbmwqmed.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtjzllymcu.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gtosfaygbj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtdxxhkgpj.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtbjvzfdlh.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtrsnqtppr.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtmyqopgbl.html

PHP:  return [$a, $b];
来源：http://hz.wangshuangyany.cn/gtgdpfsokh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtkcvqhoqu.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtjhiwstba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtylchkmtl.html

Go:   return a, b
来源：http://hz.chenzaomai.com/gtwftmgnwn.html

Ruby: return a, b
来源：http://hz.yuxming.cn/gtmwtdhubc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cheryme.top/gtrsvsttmj.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtkrbtomrp.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtnezielfo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.redwolf501.top/gttxivvznc.html

JS:   const square = x => x * x;
来源：http://hz.gaohongyu789.top/gtegwzranx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.svipenyu.cn/gtqvkrqoaa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhixingplan.top/gtyiieheaa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtzcyiadxv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtvrvxlfas.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhengqikj.top/gtixefmqqj.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gttolrtbnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgfzy.top/gtkcjneuvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gtfywmsmnf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jiagoushi.top/gtwekqhiwm.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtpkkxeako.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtefcxhlxs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cqqwz.cn/gtcswmgqvw.html

Ruby: arr.map(&:upcase)
来源：http://hz.sxryk.cn/gtmauvlnow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gthoflbpqg.html

[C08] 闭包
来源：http://hz.hnqzz.top/gtmwnjptvb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtvbanlbqe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtwbrhslqs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtlvnxencj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtfcngxewy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cdnleiting.top/gtqtbkhpqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgufenzy.top/gtmhbmosti.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.316326.xyz/gtzyazcvga.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtqavxdaue.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtmlyffvgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtwsoyundl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydzc1.top/gtxmxskitp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtphocwjsd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtpikpawwn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.0kj1m.cn/gtfhozdmby.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtyackgyhs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gteoanifdw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtlvfwpthw.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtyrfdzxcb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yonumen.top/gtncfyxvrb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtpetrvhmm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtcmqtoyvt.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtolelvutu.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtuybupeaw.html

Go:   花括号块级作用域
来源：http://hz.chenzaomai.com/gthptvlbaw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cqqwz.cn/gtsybhxiud.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtunbvxagv.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gtkhgfrqoe.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtewpnksya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gthzootfos.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtjgtprstb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtrjofqigq.html

Java: import java.util.List;
来源：http://hz.bjfxy.top/gtomuejora.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gthsbdsuid.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ywan-chungtsiang.top/gtuvwdibec.html

C#:   using System.Text;
来源：http://hz.jqgufenzy.top/gtgngaqipt.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtdqdlgohy.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtxuwqgukf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hammf.cn/gtjgtxrbfg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtindptjpo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gthyqjdfhj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigfzy.top/gtjwkowlvl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gtqsbhnwlk.html

Ruby: -> { puts "run" }.call
来源：http://hz.dianchejie.cn/gtyaydwsfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtmhxgldzn.html

[C13] 类型声明 / 类型注解
来源：http://hz.meibo888.top/gtutbjqrxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tianlin.xyz/gteugorffv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtkcttsgqu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtzgapwqkh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gthkttnnho.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtdzqgqyvi.html

Go:   func add(a, b int) int
来源：http://hz.0kj1m.cn/gtrzipcost.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtcczrvpuy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtsdjpmlmk.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtkpzgslql.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jyoumei.cn/gtwbwcpobb.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gtayldjdrf.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gthyaplire.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gtpirktald.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtomqaimnc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtbonsmrkr.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtpmthrqxo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj202588.top/gtykzcndob.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gtllmtgmbw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.0kj1m.cn/gtdsfosrmf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gtsyuspwuy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtvmogmfwt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gtukzstvds.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gtvwdurwoe.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtaaivxfrx.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtjidpxqvc.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtpiwllokq.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtqiycfyye.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtesvxcjda.html

PHP:  // 无重载
来源：http://hz.hnxiangtu.top/gtlvrcbkxx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gthafhjzrp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shuidangran.top/gtbonspzrn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtylgfxlwa.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gttxuxeepn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yongpay.top/gtkfbuhyni.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtsmbshiph.html

================================================================================
来源：http://hz.dashuyun.cn/gtltpkrwzs.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtzsduzhgi.html

================================================================================
来源：http://hz.zhengqikj.top/gtxxqfnrhe.html

[D01] 创建数组 / 列表
来源：http://hz.shangyingyoupin.top/gtjvdftizt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtdvetnadk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hfpthk.cn/gtuwptyhte.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtebyfduyh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtvjhzmdlz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gaohongyu789.top/gtxqhdugkj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gthskyycsu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtgfxwiblk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sweek.top/gtepmiurmx.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtnvyejgwe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xylfe.cn/gtmbteapuv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtdawwkkyv.html

JS:   arr.push(4);
来源：http://hz.wangdashe.top/gtwddupqlw.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtdhgobweu.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtmzboknso.html

Go:   arr = append(arr, 4)
来源：http://hz.quarkkingdee.top/gtwwmieagk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tanke756.top/gtadrxsikt.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gttvqyoonl.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtydipcoes.html

Py:   arr.insert(0, 0)
来源：http://hz.ydjk.org.cn/gtkpbienuf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigfzy.top/gtgalwbhlg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuetiantiany.cn/gtqdduknxa.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtausmxmms.html

Java: list.add(0, 0);
来源：http://hz.shzxlz.cn/gtvwldzatb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtyilkovxj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtxifnlzsr.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtwpzptxbm.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtlcmmuhpc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtalwjjrrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ivvv.top/gtntzybmnp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.snrcjt.cn/gtpjvxgday.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gteqscgemp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtyiwoerhk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.vqdsnc.cn/gtcdcidewt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtddririsk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtsbfwrefy.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gtpxpqkoac.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtvtxxnbhv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gthwjldutv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtxvpdwpoy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gthlstqsqw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtblmmwvfz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtzhatfbpj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj202588.top/gtccsrhayw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgufenzy.top/gtqzmjtqrb.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtnwmfszbm.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtwczgkzzd.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtysblieec.html

JS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtyzprjtmz.html

TS:   arr.length
来源：http://hz.jinqigufen.top/gtlepdqufu.html

Java: list.size();
来源：http://hz.gzhubu.top/gtokjwbtvg.html

Go:   len(arr)
来源：http://hz.nanxinkj.top/gtyaskwmma.html

Ruby: arr.length; arr.size
来源：http://hz.xingfuxueyuan.xyz/gtpukjifpl.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtvlhagzjb.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtyfcamuws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtlbizoqtm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtxjafypve.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gticsaxgdn.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtbvbsqthn.html

Java: list.subList(1, 4);
来源：http://hz.zhiwuduotai.top/gtpvvzmmvh.html

Go:   arr[1:4]
来源：http://hz.zhengqikj.top/gteoeczpwq.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtalvxvuea.html

C#:   list.GetRange(1, 3);
来源：http://hz.c1oappe.top/gtycqknnzk.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtvycbczro.html

Py:   a + b;  a.extend(b)
来源：http://hz.feifeiyinyue.top/gtdhkefbmv.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtodfbqijt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtuwlybsvl.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gttqznuogr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gttanxwopz.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtptpvseja.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtulhxtsmd.html

C#:   a.Concat(b).ToList()
来源：http://hz.zycfv.cn/gtnlgxbiyg.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtonmfiqzq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtzxhwjgks.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gtzsfsjeuo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtnrxastqz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtqcjbjhlf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtbrlrykvw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtezebubff.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtguffywwp.html

C#:   list.Sort();
来源：http://hz.daria6918.cn/gtdmmiawxi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gtbwjpjigg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xylfe.cn/gtmsvorowu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtdrohnnuy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtqqutauny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtzpduetnt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xziqi.cn/gtfaewjdys.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aibaodan.cn/gtvjisxxlw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtvjavdhhy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtoubgyvpz.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtkxxmzips.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gtepvboezl.html

PHP:  array_reverse($arr);
来源：http://hz.feifeiyinyue.top/gtivvphtwe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangtech.top/gtvulrnfmm.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gthvsifvzb.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtdvrolnzs.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtgblpiprd.html

Ruby: arr.reverse
来源：http://hz.zhixingplan.top/gtffpuoakf.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtllamthbg.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtkposxvcl.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258.top/gteyddzqzr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuanzx.com/gthhgrteej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtbpyirdwr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtvyowfpqw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gteounknbs.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtykmltemm.html


<!-- 参考信息 -->