代发 wailian999

Java: if (data == null) return;
来源：http://hz.snrcjt.cn/gtnrkjxpsq.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtkpndwxws.html

Ruby: return if data.nil?
来源：http://hz.guowangkeji.top/gtfyrimttr.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtrliojlgc.html

================================================================================
来源：http://hz.guowangkeji.top/gtrfkgbkqa.html

C. 函数与作用域
来源：http://hz.ybcxt.top/gtoucijrxh.html

================================================================================
来源：http://hz.wangdashe.top/gteqqsaref.html

[C01] 定义函数
来源：http://hz.sufxvd.cn/gtdanufkll.html

Py:   def add(a, b): return a + b
来源：http://hz.zhaomingkeji.xyz/gtytkypwwf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtcrwftxqv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.iojbl.cn/gtnaeptlcn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gteijgbaws.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtcjwalovo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gttwjgmotx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtdrmuzehx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gthmroalgv.html

[C02] 默认参数
来源：http://hz.xingfuxueyuan.xyz/gtzypnemcn.html

Py:   def greet(name="World"): return name
来源：http://hz.gzhubu.top/gtyhvtyxbi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtbeijsbsv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yongpay.top/gtciwncgwm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtftvzlqvv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sxryk.cn/gtxkeguqxd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtdppoivrj.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtwodifnur.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gogol.net.cn/gtgettrigs.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gttgvenkso.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258888.top/gttugbmsrn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gttbyllbqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtfpduwmrq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtgwybhbpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenlongwang.top/gtowfxixss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hywenlv.cn/gtdovnuiop.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gthgmrdopf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtfrxtdyqo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shzxlz.cn/gtbyoadmcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gtevlletur.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtxqltdqth.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtykzcjohy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gzhubu.top/gtpugacxrr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cqqwz.cn/gtshtfudwc.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gtfmjpokgg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtahwrzgea.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtrfuwyjln.html

[C05] 返回多个值
来源：http://hz.hongshengwenyu.top/gtivnkblvq.html

Py:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtxibyzcys.html

PHP:  return [$a, $b];
来源：http://hz.c1oappe.top/gtynsmqmmg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtkqrgcjxm.html

TS:   return { a, b };
来源：http://hz.zhiwuduotai.top/gtrfcypqir.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hammf.cn/gtfshilbgp.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtprlhtfcp.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtfcjxglov.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.fengsongda.top/gtzeulcggh.html

[C06] 匿名函数 / lambda
来源：http://hz.ehwqpu.com/gtczrvpncv.html

Py:   square = lambda x: x * x
来源：http://hz.daxiang520.top/gtlldrasgj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gttjldkmhb.html

JS:   const square = x => x * x;
来源：http://hz.havefunace.top/gtrtjxgxeh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cashguo.top/gtwtygpvrl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigfzy.top/gtcdukxxjt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtupbirtbz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gtbgrdlhos.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xylfe.cn/gtbdbzkrvv.html

[C07] 把函数作为参数传入
来源：http://hz.zhixingplan.top/gtgxwygkmv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtydnfkesc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jiagoushi.top/gtwyrnftwx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhiwuduotai.top/gtdgamqfut.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtgsihrsuy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nwbrower.top/gtidsgvnnn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxuanxn.top/gtmcpjquld.html

Ruby: arr.map(&:upcase)
来源：http://hz.guowangkeji.top/gteccxssvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangdashe.top/gtclyysdwo.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtfjbnnccd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jqgfzy.top/gtnnmsqatx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gtmnpkuiqh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtezzikzir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtkrshswsd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtgdtygdmu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.0kj1m.cn/gtutmvtyvf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtkustalez.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtldsirrjl.html

[C09] 递归
来源：http://hz.xinyue.icu/gtfrvbqjst.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtmlosnjqo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xinyue.icu/gtrvcwaufn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtlxzdincp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtftixoshj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gtqjgmwavd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shangyingyoupin.top/gtvrwuxacx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jqgfzy.top/gteknxgeny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gthfigbjty.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtegqhlrlm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtdthokwjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigufen.top/gtpznwflbr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtlmgkezfn.html

TS:   同 JS
来源：http://hz.ivvv.top/gtfajxvkiy.html

Java: 方法内为块级作用域
来源：http://hz.c1oappe.top/gtavpgyavy.html

Go:   花括号块级作用域
来源：http://hz.jinyuanbaomall.cn/gttntaxkac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.havefunace.top/gtptxjmzbb.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtvoslctnb.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtgzjweiav.html

Py:   from module import func
来源：http://hz.xuetiantiany.cn/gtruhrdgwk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtyydxbmsj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtbrlhdhlt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gogol.net.cn/gtozpfcgyc.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gtxwibdyyz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtzdqksaad.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtjagojlmv.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gttyncjiap.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtjuymoney.html

Py:   (lambda: print("run"))()
来源：http://hz.zhijiandao.cn/gtitmkldcg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jyoumei.cn/gtbqpovfxm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtykyhzqtd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtwgbtvmkx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtfpqdooxd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtlkyyauag.html

Ruby: -> { puts "run" }.call
来源：http://hz.nwbrower.top/gtkcqjmovy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ybcxt.top/gttjaltphb.html

[C13] 类型声明 / 类型注解
来源：http://hz.redwolf501.top/gtieudupyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtfhinuanx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtnftwawda.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtcevckjlw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.redwolf501.top/gtzlxrdkkr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtdmcfocfw.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gttuiancuh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtpruhmmuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuanzhike.top/gtrishsetv.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtmoplynup.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtbihgikme.html

PHP:  // 无泛型
来源：http://hz.aizwys.cn/gtmuftyaio.html

JS:   // 无泛型
来源：http://hz.zhongyouzk.top/gtgbhxjdwg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guannengcc.top/gtcqcnzowa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtnpgeegpq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxinkj.top/gtogqzmbit.html

Ruby: # 无泛型
来源：http://hz.0kj1m.cn/gtcdweccnj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydzc1.top/gtgjnllaok.html

[C15] 解构 / 展开参数
来源：http://hz.guannengcc.top/gtpidyqyhf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtbllkyvsf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtvswgfejg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtmdoyopap.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.9152youxi.cn/gtbctppqap.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtdgljfhzt.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtsljceips.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gthlvhjken.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtnxuefupp.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtylkhktkk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gogol.net.cn/gtojrdonot.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtlogcfllq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cqqwz.cn/gtxqbsshpe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gttyzvyhsp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtyczhacld.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydzc1.top/gtayhmzkvm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.havefunace.top/gtovhezooz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gthnlghpqi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtynyieeyx.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gtbczvlsgu.html

================================================================================
来源：http://hz.gotoacloud.top/gtvxfftihs.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtdjsanoqg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.c1oappe.top/gtzuyxzaqv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhijiandao.cn/gtjpqnubce.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtggqsxrxv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtqbkdzlqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtpxawajys.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dianchejie.cn/gtmppbdlej.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tanke756.top/gtqydwaief.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtsqcnbpzz.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtvofhbahw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jyoumei.cn/gtksoubirq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtcrglbiiw.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtvkcetoey.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtdswbjnrh.html

Java: list.add(4);
来源：http://hz.cucudq.cn/gtoqymmnam.html

Go:   arr = append(arr, 4)
来源：http://hz.chenlongwang.top/gtctosflgy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtjyjylpzu.html

C#:   list.Add(4);
来源：http://hz.zycfv.cn/gtybxreixx.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtytsdrojh.html

Py:   arr.insert(0, 0)
来源：http://hz.nwbrower.top/gtdzjgsxiu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tian-w.cn/gtqcvmgjox.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtshzahusq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtgdxckvkg.html

Java: list.add(0, 0);
来源：http://hz.zhixingplan.top/gtlngbxbse.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.tianlin.xyz/gtntcxkqft.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtdraumekd.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtutwqhaeu.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtqwuhezgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtqdbhmxaz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtwfsdtier.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daria6918.cn/gtsiwdrklh.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtiazjkgtu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtxprbjslc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxuanxn.top/gtruwzlezi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yanxiufei.cn/gtmtwdfjou.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.iojbl.cn/gtjmfymtwy.html

[D05] 访问与修改元素
来源：http://hz.hywenlv.cn/gtnfafuclt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtfvcywjpp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.bjfxy.top/gttjhfxqhq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtrjscdfsb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtnmfzbwke.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtwykahbnj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtmubhglnr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtajtmlvmx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtgkfizttu.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtludefuvg.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtybertbwi.html

PHP:  count($arr);
来源：http://hz.yuxming.cn/gtckouigqb.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtadiycybk.html

TS:   arr.length
来源：http://hz.cqqwz.cn/gtmrbxasfp.html

Java: list.size();
来源：http://hz.ydzc1.top/gtammjhrse.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtswfukwoh.html

Ruby: arr.length; arr.size
来源：http://hz.snrcjt.cn/gtxtfmxhvt.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gtxbskihri.html

[D07] 切片 / 取子数组
来源：http://hz.vqdsnc.cn/gtmbbzkrfi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtwumtuczj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.kuanghao11.cn/gtuqstewhb.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gthmzjonsu.html

TS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtaqdjmahn.html

Java: list.subList(1, 4);
来源：http://hz.hnqzz.top/gtkvloloei.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtpisrqtgn.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtkjovprao.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhiwuduotai.top/gteugunpok.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gtmdudphfz.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtknosruyc.html

PHP:  array_merge($a, $b);
来源：http://hz.zhiwuduotai.top/gtzfzlqikz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnxiangtu.top/gtwvzxanrm.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtsdcmhmlp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtcyqnnzhh.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtvuwludes.html

Ruby: a + b;  a.concat(b)
来源：http://hz.c1oappe.top/gtfqcdsbnj.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtjmisahre.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtughrbafq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtwzszbwct.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gtolmyqkuc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtbscohojb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hammf.cn/gtstwzexle.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtsdjtwyma.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtebjqoeqa.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtmbxkihjd.html

C#:   list.Sort();
来源：http://hz.jqgfzy.top/gtcofwnwor.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtlqehynfk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtctxpaqbc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtdnisljao.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtajetnprc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gttvsiwgoa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jiagoushi.top/gtcleezzad.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gtxemmvyuy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sxryk.cn/gtriahween.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.feifeiyinyue.top/gtculcsnhg.html

[D11] 反转数组
来源：http://hz.ppjwa.cn/gtpodrjjnu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ppjwa.cn/gtrokemqdk.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gthekhgpsk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gteuorvfkf.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtgwagghkm.html

Java: Collections.reverse(list);
来源：http://hz.chenzaomai.com/gtsskqvfqh.html

Go:   slices.Reverse(arr)
来源：http://hz.yongpay.top/gtqzitlttj.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gticwiyesr.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtixmbrxrh.html

[D12] 查找元素下标
来源：http://hz.nanxinkj.top/gtkfunazgf.html

Py:   arr.index(x);  x in arr
来源：http://hz.sxryk.cn/gtjxzjlocz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhijiandao.cn/gthfxpwtqs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtwspvsjdg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gteyafsbtz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydjk.org.cn/gtmqtbzcvn.html

Go:   slices.Index(arr, x)
来源：http://hz.yangfankeji.com/gtsfvuguhn.html

Ruby: arr.index(x)
来源：http://hz.gogol.net.cn/gtgqawymzj.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258.top/gtstlsrxuf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtasshbdrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yuxming.cn/gtwgqxfzsq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtdaaxwxkx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtksqefaqm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtibcobbgm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gtsubmhodb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtmvrjezts.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.0kj1m.cn/gtuyvxaamf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hywenlv.cn/gtcyiatwtu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtnfnalcxa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gttxdpepmu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtzbtktbuy.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtbiiongcm.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtqgmrdify.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhixingplan.top/gtpnurwxys.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtyghcntov.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtshbvrmah.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gaohongyu789.top/gtvplvrube.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtvxhtavla.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtvqnbuynd.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gtcmzscqsb.html

JS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtzfgnqibm.html

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtsnunhmtr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtfhqceqaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangkeji.top/gtqlexybdh.html

Ruby: arr.uniq
来源：http://hz.shangyingyoupin.top/gtetsedbou.html

C#:   list.Distinct().ToList()
来源：http://hz.quarkkingdee.top/gttbtceybb.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gtnkukeuma.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guannengcc.top/gtnbzdmxhx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtgsgjlywq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtuypvbjmu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtindzehqu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gtscjjpeay.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtiogfnlot.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtvutpmxjc.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtctobbndm.html

[D17] 最大值与最小值
来源：http://hz.gogol.net.cn/gtkudfzugf.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigufen.top/gtdmnfthhl.html


<!-- 参考信息 -->