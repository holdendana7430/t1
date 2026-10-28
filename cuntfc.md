代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtfrnamont.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhijiandao.cn/gtsevmbuci.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.kuanghao11.cn/gtltnuyaze.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xinyue.icu/gtwdpxsotu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jiagoushi.top/gtlcsdwhum.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gzhubu.top/gtpkntfpbc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daria6918.cn/gtaedqmych.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtyvdfwreq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hnqzz.top/gtckckpjyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gtmvxbhwib.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtvfbnvwvq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtoewrmmip.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtfxllhjio.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hywenlv.cn/gtsbfmucds.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shangyingyoupin.top/gtmbnsssnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtywhxmovb.html

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gtxvgozkld.html

Py:   isinstance(x, (int, float))
来源：http://hz.quarkkingdee.top/gtxzbrvpgc.html

PHP:  is_numeric($x)
来源：http://hz.yj20258888.top/gtehhiqhln.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtkrjyytya.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangdashe.top/gtrxlbuvto.html

Java: x instanceof Number
来源：http://hz.daria6918.cn/gtbkevfczm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtjqcbfpht.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtvrfgvsux.html

C#:   x is int or double or decimal
来源：http://hz.ppjwa.cn/gtjxmcfxtn.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtorlqpoqg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuetiantiany.cn/gtygsexcis.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jyoumei.cn/gtimuolnug.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtptxwgohd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtrotjqgyc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhijiandao.cn/gtewyzgtfc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.quarkkingdee.top/gtgqvakkll.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.316326.xyz/gtzujzqdtu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtgpyzsgkq.html

[B15] 布尔运算与取反
来源：http://hz.zhongyouzk.top/gtghqmmama.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gthfbnebcw.html

PHP:  $a && $b || !$c
来源：http://hz.hfpthk.cn/gticqerlan.html

JS:   a && b || !c
来源：http://hz.tanke756.top/gtnhkvioyi.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtbnlbjqzz.html

Java: a && b || !c
来源：http://hz.cucudq.cn/gthprlcivz.html

Go:   a && b || !c
来源：http://hz.gogol.net.cn/gtjovufutf.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gtcshsotjo.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtgwmfagbx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtfvdrlqbp.html

Py:   if not data: return
来源：http://hz.meibo888.top/gtljtdgexh.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtdsdwzfwr.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtsaalcjzh.html

TS:   if (!data) return;
来源：http://hz.jqgfzy.top/gtoszjlkpv.html

Java: if (data == null) return;
来源：http://hz.zhoulong.xyz/gtdumkhisl.html

Go:   if data == nil { return }
来源：http://hz.vqdsnc.cn/gtgxgbugvt.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtkfjrfsug.html

C#:   if (data == null) return;
来源：http://hz.gaohongyu789.top/gtymunccvw.html

================================================================================
来源：http://hz.shuidangran.top/gtgfhfqlal.html

C. 函数与作用域
来源：http://hz.xuetiantiany.cn/gtgetmaptd.html

================================================================================
来源：http://hz.jiagoushi.top/gtuqhvnwkv.html

[C01] 定义函数
来源：http://hz.sweek.top/gtdgtnsqfu.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtvhimqowe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtxeaaeevn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtostfdvre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gttlzyyaya.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtdmesfqgy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangdashe.top/gtgwdbaoqy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.0kj1m.cn/gtgpwqibag.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gteyfcsmao.html

[C02] 默认参数
来源：http://hz.tian-w.cn/gtxeiglxdr.html

Py:   def greet(name="World"): return name
来源：http://hz.zhongyouzk.top/gtwwfteirg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shuidangran.top/gtzvwmcphu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ybcxt.top/gtbdmtllou.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sysykeji.top/gtnllqenqf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.meibo888.top/gtriccoyht.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yueranfly.top/gtztinzjis.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtujhqwdsw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtutrmqwuf.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtvjlrxtug.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtnnzbyddy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gttsszpqrq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtqbrgnsbw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtnycubdsg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtetuxcrnj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtwjmjlvfg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtjjjorrhj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigufen.top/gtupmpvxmv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtdczwtzzg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jyoumei.cn/gtkeydipvh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cheryme.top/gtwhixcuza.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gttoivtefm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtgoiqdjgn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtpvgzhrjo.html

Go:   // 无：用配置结构体参数
来源：http://hz.gogol.net.cn/gtdhytuzcp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtckhemsay.html

C#:   f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gthpyrhbvk.html

[C05] 返回多个值
来源：http://hz.9152youxi.cn/gtqkibcdch.html

Py:   return a, b
来源：http://hz.cdnleiting.top/gtjwjcernv.html

PHP:  return [$a, $b];
来源：http://hz.yvedp.cn/gtmaxvfwsa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fzhhl.top/gtadlohqct.html

TS:   return { a, b };
来源：http://hz.cucudq.cn/gtuuyildrg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtlcqvwmdn.html

Go:   return a, b
来源：http://hz.birdmap.top/gtuukucumd.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gtnfabsphy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtdqawbipv.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtbwtzvpeq.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gtxierwrht.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenzaomai.com/gtwikgtxtj.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtdphrdqut.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jlsjyb.cn/gtkllicqen.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sufxvd.cn/gtydmdhafx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gteoebrald.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ybcxt.top/gttlslzwzl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtlpipaein.html

[C07] 把函数作为参数传入
来源：http://hz.yangfankeji.com/gtpjcdvjjm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hongshengwenyu.top/gtxhstxoky.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cucudq.cn/gtqdyzutoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zycfv.cn/gtgzenqnew.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtmvxmnapd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.kuanghao11.cn/gthtefsazm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtpotmcbju.html

Ruby: arr.map(&:upcase)
来源：http://hz.c1oappe.top/gtjrbfvdxz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuanzx.com/gtbcdbpzrg.html

[C08] 闭包
来源：http://hz.dianchejie.cn/gttjvouxos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gttrhmzqpt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuanzhike.top/gtmvgopcgr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtjthdpzmk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtihrozuxd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj202588.top/gtrgweycvw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xinyue.icu/gtajdhivld.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtgdwkzgyk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtzqaxqdhi.html

[C09] 递归
来源：http://hz.yongpay.top/gtlrbwwrab.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sxryk.cn/gtxlprwtkb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.iojbl.cn/gtrsyjlwgf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ybcxt.top/gtdbxjdzcy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtwccdhtwt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gtakuiczng.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gttjlqesxk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zdqjudy.top/gthyailesn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gtdmlsdtwx.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gthjpuzcei.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtzaexehfc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuetiantiany.cn/gtbtnjglyl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cheryme.top/gtipfvzypd.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtsjnsaroj.html

Java: 方法内为块级作用域
来源：http://hz.sweek.top/gtwekromdf.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtxodjlayr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtbluqzskk.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtvxgkojmi.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gtazjpugjz.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtmgqnhwgw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cdnleiting.top/gthdyjjppa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sxryk.cn/gtjzqswvlu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guowangkeji.top/gtazkxzjxv.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtpwtwlojk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hywenlv.cn/gtflpyadpe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hysaishi.cn/gtvmgoaprm.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtcftsfcjh.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenlongwang.top/gtrljbxmzz.html

Py:   (lambda: print("run"))()
来源：http://hz.meibo888.top/gtqzlphmoo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xylfe.cn/gtjvrdvmeb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtgixynpbz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtmpzobuna.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtihzzaryo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gttptoodjl.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtbmqerdlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cheryme.top/gtryyvsmse.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtieowkfqs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhixingplan.top/gtyvhoygal.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtueutsckc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtalkckqgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtwfjdoikv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtrosrzdrz.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtukbajbgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guannengcc.top/gtlyagcwbg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gthumurhpt.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtksgrgiqa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtwfegfvoi.html

PHP:  // 无泛型
来源：http://hz.yvedp.cn/gtufgvwuyh.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtzzelhyas.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuxming.cn/gtyixfskxh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nwbrower.top/gtktdpubhw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.svipenyu.cn/gtlezrgvme.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtvyvwlhmr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtkporjopt.html

[C15] 解构 / 展开参数
来源：http://hz.gzhubu.top/gtiyqjknat.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jianghu66.top/gtbvdqbbdr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtnpifentw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtxctqfykw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtwrxghzil.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtwthkmmdr.html

Go:   // 无解构
来源：http://hz.chenzaomai.com/gtwfckqnpx.html

Ruby: a, b = pair
来源：http://hz.shangyingyoupin.top/gtjcwsgylb.html

C#:   var (a, b) = pair;
来源：http://hz.dianchejie.cn/gtgjbgzblt.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258888.top/gtwlovtpks.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtkjqionfy.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtzjhhlipj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtlhxedyai.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gogol.net.cn/gtezxttahe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shanyushiyangtech.top/gtapkyjggx.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtjyncxqfo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenjidiqi.icu/gtknldcbno.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtthvqzkpl.html

================================================================================
来源：http://hz.tian-w.cn/gtsneqxqcv.html

D. 数组 / 列表 / 集合
来源：http://hz.9152youxi.cn/gtgosbcxtf.html

================================================================================
来源：http://hz.jinqigfzy.top/gteqfustja.html

[D01] 创建数组 / 列表
来源：http://hz.jqgufenzy.top/gtzrsyccoo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.iojbl.cn/gtaebvcdam.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gttnnivhrj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtlxlnivpl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtrrsjqmhx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.52xcode.cn/gtetgmgqzb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtcrjkbjzy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtgcbdjhvz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.mhx1999.top/gtatsjlaeb.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtkgwsttza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtzbtdthfq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.smart0.xyz/gtuehpsmni.html

JS:   arr.push(4);
来源：http://hz.xinyue.icu/gtajfoeros.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtrmvzqzoi.html

Java: list.add(4);
来源：http://hz.xuanzx.com/gtvpjoqyke.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtiroscyws.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinyuanbaomall.cn/gtdmnicntw.html

C#:   list.Add(4);
来源：http://hz.quarkkingdee.top/gtwijzywnb.html

[D03] 在指定位置插入元素
来源：http://hz.andypj.xyz/gtnjoypsza.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtbhjvpdrg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xziqi.cn/gtcqmgorgl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gthzcvwdpu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nwbrower.top/gtbvjjrrep.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gthnrwpppw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtngeqallx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxinkj.top/gthriqsmck.html

C#:   list.Insert(0, 0);
来源：http://hz.andypj.xyz/gtzrnpsrqw.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtsxsujwuj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtwdclxhbi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gzhubu.top/gtxwwtuass.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuxming.cn/gtbiwmbbnj.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gttxdoheqf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtcjwneeai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtjgvbmbxs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pycfn.com/gtovdgtidj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenzaomai.com/gthwevozmb.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtqugdthhm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtahzivdqf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.316326.xyz/gtgkhuwgds.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtogoqkybx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gtsyyweqdz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xingfuxueyuan.xyz/gtfgltwkgi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.pycfn.com/gtmuzvdzsk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtsmfdecat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dashuyun.cn/gtrdzjgjvc.html

[D06] 数组长度
来源：http://hz.hnqzz.top/gtexaqywuc.html

Py:   len(arr)
来源：http://hz.fzhhl.top/gtfnfjkgqh.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtevuteeqj.html

JS:   arr.length
来源：http://hz.yongpay.top/gtdnajgabu.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtzpgwdwoa.html

Java: list.size();
来源：http://hz.smart0.xyz/gtzclwcvlk.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gtpqzdbgxx.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtgwnhlnlb.html

C#:   list.Count;
来源：http://hz.jlsjyb.cn/gtiqldgmxf.html

[D07] 切片 / 取子数组
来源：http://hz.sufxvd.cn/gtymziagix.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gttrvylrfy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtplwffnek.html

JS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtdsxfritm.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtfwihphei.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gthvpbjxcl.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtncnypvdd.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtljcnadxw.html

C#:   list.GetRange(1, 3);
来源：http://hz.daxiang520.top/gtofphkfqj.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtghaeniqz.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gteuhrddie.html

PHP:  array_merge($a, $b);
来源：http://hz.gotoacloud.top/gtapxixfax.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nwbrower.top/gtratcsrfb.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtbjlzcdat.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.vqdsnc.cn/gtmqjprdde.html

Go:   append(a, b...)
来源：http://hz.svipenyu.cn/gtvpecybrl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtorobeksa.html

C#:   a.Concat(b).ToList()
来源：http://hz.zdqjudy.top/gtgtysmdui.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gtlguwfsgm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtqaarwswu.html

PHP:  sort($arr);
来源：http://hz.zhaomingkeji.xyz/gtrzvtgntq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gtvivznxrq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.0kj1m.cn/gtimkwtsbb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.meibo888.top/gtojmkfckf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtlgpxfldy.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtuikerzih.html

C#:   list.Sort();
来源：http://hz.birdmap.top/gtqffgurce.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtlngsdlgm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tanke756.top/gtrpfsiopd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtemntoruy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtjcdkjxsu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtreddtwkb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gticchdett.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgufenzy.top/gtsrdjrbau.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gteoqmjvoh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtjftqkbtz.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtnkwdwhgf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daxiang520.top/gtomybyhga.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtrquozhve.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtvgeitcjz.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gttehjlceq.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gtubkkxlhs.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtidbwpnnt.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtqmxwokak.html


<!-- 参考信息 -->