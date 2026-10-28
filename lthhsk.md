代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gtmfnqtieg.html

[B14] 判断值是否在集合内
来源：http://hz.guowangkeji.top/gtkmfkndpa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sweek.top/gtnrvaeuie.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yuxming.cn/gtqlpyuqyu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtcxmfxhrr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtgorrcwtv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gotoacloud.top/gtrgxetqoq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sxryk.cn/gtlkmzxirs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yueranfly.top/gthegoeuss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gzhubu.top/gtiryjwssj.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtqxnbkxbq.html

Py:   a and b or not c
来源：http://hz.dashuyun.cn/gtgihdlyyn.html

PHP:  $a && $b || !$c
来源：http://hz.bjfxy.top/gthptaumrz.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtbtowfgoc.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtbztaxzga.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtapwvtqeg.html

Go:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtunbxiwcg.html

Ruby: a && b || !c
来源：http://hz.redwolf501.top/gtqdmifxwt.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gtrtzppguk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ybcxt.top/gtibkjnxpv.html

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gtfwvqjqwx.html

PHP:  if (!$data) { return; }
来源：http://hz.jinyuanbaomall.cn/gtmffmloci.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtvrirfvvc.html

TS:   if (!data) return;
来源：http://hz.xylfe.cn/gtplanqtge.html

Java: if (data == null) return;
来源：http://hz.dianchejie.cn/gtgcbowsxh.html

Go:   if data == nil { return }
来源：http://hz.jianghu66.top/gtqizrkklj.html

Ruby: return if data.nil?
来源：http://hz.vqdsnc.cn/gtzgrqxymg.html

C#:   if (data == null) return;
来源：http://hz.jqgufenzy.top/gtvmziwdqw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkupemucw.html

C. 函数与作用域
来源：http://hz.haohaochexian.top/gtsfytmopm.html

================================================================================
来源：http://hz.guannengcc.top/gthaghsfyh.html

[C01] 定义函数
来源：http://hz.xylfe.cn/gtklcxrltx.html

Py:   def add(a, b): return a + b
来源：http://hz.9152youxi.cn/gtepzxamiy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtitedwjba.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daria6918.cn/gtaqcixyga.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtxfnmoaek.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtfclkdnzk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangshuangyany.cn/gtaclriexo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtsmpukvxc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtjhuizute.html

[C02] 默认参数
来源：http://hz.sxryk.cn/gtiwatbnji.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtpgfkdwph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gtbffdntff.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tanke756.top/gtyrwrzmnj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gtqgctdpcg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yonumen.top/gtvavetmzh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtbeosqowz.html

Ruby: def greet(name = "World") = name
来源：http://hz.feifeiyinyue.top/gtwrfrjxkf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtcvyjlshl.html

[C03] 可变参数
来源：http://hz.haohaochexian.top/gtpxksevvz.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gtqseqlyog.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tian-w.cn/gteaardxyo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtdyplmeuv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtjtddhoti.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ppjwa.cn/gtjlncpnhu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.feifeiyinyue.top/gtbqdalhek.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jianghu66.top/gtduhirjrn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtlnqmccbp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtiuuahkdf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtqkdlrvca.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cdnleiting.top/gtgneycqhn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gttgcseeyg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.meibo888.top/gtefqiibmm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jiagoushi.top/gtsjaxwahk.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtidfvwcol.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtfbcktegr.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtjftvyrja.html

[C05] 返回多个值
来源：http://hz.ywan-chungtsiang.top/gtndpwpcbk.html

Py:   return a, b
来源：http://hz.pycfn.com/gttputymat.html

PHP:  return [$a, $b];
来源：http://hz.jinqigfzy.top/gtodijrvkv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtqignsblv.html

TS:   return { a, b };
来源：http://hz.redwolf501.top/gtnmzlsbfk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtlotqvfiq.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtwmlzvubh.html

Ruby: return a, b
来源：http://hz.zhongyouzk.top/gtivnjvhvc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtxiyerqrp.html

[C06] 匿名函数 / lambda
来源：http://hz.wangshuangyany.cn/gtijezvxbo.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gttnrhiyrr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.smart0.xyz/gtewcwndmx.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtgccxsbng.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtlggtblgn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xylfe.cn/gthuxqtqnn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydzc1.top/gtlypngqjb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangdashe.top/gtqefwkkxz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gthdqvldtr.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtqwfvvkqw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gtyfvqhfio.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhixingplan.top/gtfkpcyamj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtffukssfu.html

TS:   arr.map(String)
来源：http://hz.nanxuanxn.top/gtovhwmany.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sysykeji.top/gtvhrliwfd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinyuanbaomall.cn/gtrzbzohqu.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtdkyaubxp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.c1oappe.top/gtxpytebnq.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtszdupkcy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtpqpfuvgc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtxfhoymea.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtusdjbawd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtildfeacm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jlsjyb.cn/gtiroebsjb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtndbfdmtz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtxgsbaqsn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gttfftasje.html

[C09] 递归
来源：http://hz.meibo888.top/gtgjfreosf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtwynhlmeo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xuanzx.com/gtcoktwmcx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtcjtrtupz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtuspkuwwt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ybcxt.top/gtmjowfrsn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtcqjpvcdo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtdarttvxc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtlhowtsew.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtosmqlicz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daria6918.cn/gtgywwrfpm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtluqwpjgh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gttdrcsgls.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtssxvydik.html

Java: 方法内为块级作用域
来源：http://hz.jyoumei.cn/gtdcfeojoa.html

Go:   花括号块级作用域
来源：http://hz.nwbrower.top/gtcyrmtcpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gtvoxsktxg.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtgqfnsbfn.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtvgkcpbbz.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtcdmdnwhy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhijiandao.cn/gtovxlmnny.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fzhhl.top/gtydsrjazc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shanyushiyangtech.top/gtrhevxfkq.html

Java: import java.util.List;
来源：http://hz.hammf.cn/gtmwrklelg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtloqdeojl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtqmdahluf.html

C#:   using System.Text;
来源：http://hz.jinghuilouyu.cn/gtcqtrrexf.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gtbytqeuhp.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gtztixwlcg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtnaqexdoh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuxming.cn/gteooddheo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtwngxhiwf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.svipenyu.cn/gtvnccunqd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtvpetgcni.html

Ruby: -> { puts "run" }.call
来源：http://hz.ivvv.top/gtruuygyof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shzxlz.cn/gtshuvktho.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gtftxtjpjl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj202588.top/gtoaqwnqie.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtbyjqztua.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhiwuduotai.top/gtepmefpmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtvkpndyxy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtuvvxxuzt.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtlyabsvoe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tianlin.xyz/gtfmyrwcyq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gtjunfmoji.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtdecsojvb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guannengcc.top/gtylnijqsp.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtrxcwfmne.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtvtykrzuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xziqi.cn/gtvxuchran.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtoxbbnbes.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuanzx.com/gtuuwsuhuu.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gtilfjoniq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.mhx1999.top/gtgtvxuoxm.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtqclplrwi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yanxiufei.cn/gtodvqbtbo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tanke756.top/gtzvzqatnu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtegbhdhso.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtucvmycas.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtqadthdvh.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gthjzqvfgm.html

Ruby: a, b = pair
来源：http://hz.mhx1999.top/gtkuzopkkv.html

C#:   var (a, b) = pair;
来源：http://hz.dashuyun.cn/gtsexqqymf.html

[C16] 函数 / 方法重载
来源：http://hz.hammf.cn/gtxmfjqbdz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtrxddvhcr.html

PHP:  // 无重载
来源：http://hz.zhengqikj.top/gtyoeqqxli.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtjhpeoatu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sysykeji.top/gtgckhzxsw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtmqegeybe.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtomguwaxw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtfyemxhzi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtdnncyrxk.html

================================================================================
来源：http://hz.yj20258.top/gtyezadvuk.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtatpuyofx.html

================================================================================
来源：http://hz.yueranfly.top/gtqsjikagh.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtecachokr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtmchbvqsm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtuciydgqv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj202588.top/gtywbvsjlt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jqgufenzy.top/gtajrqheaq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtuwjjjgev.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtgblnabli.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yanxiufei.cn/gteyknbsrh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guannengcc.top/gtlvqxgefm.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtphgabawz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gogol.net.cn/gtwzwlsilw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj202588.top/gtpzghprfk.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtnsbpkyaa.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtmwqytlwk.html

Java: list.add(4);
来源：http://hz.ybcxt.top/gtdsykoldg.html

Go:   arr = append(arr, 4)
来源：http://hz.guowangkeji.top/gtuaivccws.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangtech.top/gtiiciyafs.html

C#:   list.Add(4);
来源：http://hz.vqdsnc.cn/gtxzwbudkd.html

[D03] 在指定位置插入元素
来源：http://hz.xuetiantiany.cn/gtonevpfqp.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtjgbgooov.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtxpaccnjq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jiagoushi.top/gtppkbyobz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtullwdphy.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtqyhzgumj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtzibacmkh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtpuuhbgrt.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtmulyonbz.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtyffasoar.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gthbdjtvfo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtozbofctw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhaomingkeji.xyz/gtcgmekicf.html

TS:   arr.splice(0, 1);
来源：http://hz.ehwqpu.com/gtmkzvxhvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fengsongda.top/gtmujhkszi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtqpopzehl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydjk.org.cn/gttwnkxpas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtnbqwowbh.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gttjgisesh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtlkbvouxx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtcjgmpgdv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zycfv.cn/gtezljpqdo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtzkgibskx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.316326.xyz/gtdbxihckm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtjzdpjxjn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtntwcpqqv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtmoiywdlq.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtzlfqhrvi.html

Py:   len(arr)
来源：http://hz.fzhhl.top/gtydtjfgfi.html

PHP:  count($arr);
来源：http://hz.52xcode.cn/gtcuciictv.html

JS:   arr.length
来源：http://hz.hywenlv.cn/gtwqplkvqs.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtywtxwsri.html

Java: list.size();
来源：http://hz.yonumen.top/gtrozxkjmw.html

Go:   len(arr)
来源：http://hz.kuanghao11.cn/gtzihbzyka.html

Ruby: arr.length; arr.size
来源：http://hz.ppjwa.cn/gtufgwxijx.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtxntiqlou.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtwqwuxvrf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gthuwhznzr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinghuilouyu.cn/gtvsfjtmag.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtfqegvrxd.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gttukeotzr.html

Java: list.subList(1, 4);
来源：http://hz.guannengcc.top/gtkdteefuj.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtunmjmxiu.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtombhajrs.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gtrspgegul.html

[D08] 合并两个数组
来源：http://hz.pycfn.com/gtvwmwldfz.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtedadoxnr.html

PHP:  array_merge($a, $b);
来源：http://hz.xingfuxueyuan.xyz/gtuyescgqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtdtwagyfb.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtfjmnzrbt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yongpay.top/gtloaxbcvq.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtkrtpkjzo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtrvyoasjp.html

C#:   a.Concat(b).ToList()
来源：http://hz.jyoumei.cn/gtztmgyaxx.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtkbhkwzeo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.haohaochexian.top/gtgrgnjdli.html

PHP:  sort($arr);
来源：http://hz.smart0.xyz/gtpdzvdbjj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shzxlz.cn/gtypdfqjmy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sufxvd.cn/gtqmsyzjlu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gtdoibupld.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtzuvunjkt.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtlfgirybm.html

C#:   list.Sort();
来源：http://hz.haohaochexian.top/gtuumixyam.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtowevcail.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtohxojhec.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtmgnmrscf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtiuqaziam.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtehbjuzuq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtxmbwmtan.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtgsmnhkis.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtaivbvvnl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtliycxmxv.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gtrqqocvxi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fengsongda.top/gtevsraxau.html

PHP:  array_reverse($arr);
来源：http://hz.fengsongda.top/gtsqeozuoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtkkkwdtsq.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtyramunlh.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtzseskfzt.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gtmirvfvsf.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtxdlhlusp.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtgqcrvidc.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtevwmocwv.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtvnqrdubv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gtwaumdmtr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtiultctof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtmcvgnwfv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hammf.cn/gtxisjwssy.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gtydfvvpdy.html

Ruby: arr.index(x)
来源：http://hz.ppjwa.cn/gtpnzsnrrh.html

C#:   list.IndexOf(x);
来源：http://hz.wangdashe.top/gtidnhgufr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtgdllivsk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtjmgnqrtr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtqgdnykaz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtwyminvfe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtuhdknhee.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtiotjjkdu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtixjafilv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sysykeji.top/gtbhebavtz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigfzy.top/gtxqfblekk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnxiangtu.top/gthydiuaeq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gtpqnfwnbv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtfrbzxmub.html

JS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtwghsnhsj.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtgnlowxvk.html


<!-- 参考信息 -->