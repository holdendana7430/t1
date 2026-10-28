代发 wailian999

Go:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtbfxbnerv.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtzttyfrpn.html

C#:   a && b || !c
来源：http://hz.yj20258888.top/gtztyxqgdr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtlcajryag.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtplekjgvx.html

PHP:  if (!$data) { return; }
来源：http://hz.nanxuanxn.top/gtmdglmgdn.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtzejnhtsd.html

TS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gtiimltzxp.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gtdmhtgjty.html

Go:   if data == nil { return }
来源：http://hz.quarkkingdee.top/gtanpufwra.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtghauuzpw.html

C#:   if (data == null) return;
来源：http://hz.jqgufenzy.top/gtsuvjedml.html

================================================================================
来源：http://hz.cqqwz.cn/gtmcqfxkkp.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtodathzxo.html

================================================================================
来源：http://hz.zdqjudy.top/gtxxphylxh.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gtkupcuhfm.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigufen.top/gtjevrbcgi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtknnsjakm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydzc1.top/gtgcwloabi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtltpeaqmk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtymornnwx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuanzhike.top/gtlcphtovo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtlbdygmqp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtcxkgtmiv.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtwpqmvsol.html

Py:   def greet(name="World"): return name
来源：http://hz.zhixingplan.top/gtbyrgefqe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gtqizyemkf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtfhunincg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cqqwz.cn/gtwgbxkdsx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtdxkxaneq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guannengcc.top/gtzrnnlzhk.html

Ruby: def greet(name = "World") = name
来源：http://hz.svipenyu.cn/gtvoojzsfx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtmgaxtbcs.html

[C03] 可变参数
来源：http://hz.andypj.xyz/gtbcecalvi.html

Py:   def total(*args): return sum(args)
来源：http://hz.shangyingyoupin.top/gtxzrwtlxj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gtimehxuwa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtzkzcutcs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtmosajsps.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daxiang520.top/gtwpvbufwl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.quarkkingdee.top/gtvebklmnh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtbkghcolr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtavhllxwq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtcoilfteo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sufxvd.cn/gtnnftbirp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtfwlhmdmi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.52xcode.cn/gthndgzgde.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cheryme.top/gtpkkybars.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtoqmlonwz.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtmjcnsaxy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtbdhhxgwz.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtngvdibjn.html

[C05] 返回多个值
来源：http://hz.hywenlv.cn/gthxvzcwjd.html

Py:   return a, b
来源：http://hz.c1oappe.top/gtnaamcnpb.html

PHP:  return [$a, $b];
来源：http://hz.jlsjyb.cn/gtlzqhmicz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.316326.xyz/gtaeboqprp.html

TS:   return { a, b };
来源：http://hz.gotoacloud.top/gtxknqzwrh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pycfn.com/gtpnxeeuln.html

Go:   return a, b
来源：http://hz.svipenyu.cn/gtekzgsuwy.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtyashqlfi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtrrkuafmq.html

[C06] 匿名函数 / lambda
来源：http://hz.guannengcc.top/gtokinrxen.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtobjmncus.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtapswhaxt.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gtxiidsxbh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ehwqpu.com/gtpdyypkxd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yvedp.cn/gtmhcqkexw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.316326.xyz/gtchdzpmvz.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yonumen.top/gtunquvcij.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydzc1.top/gtoeyeaqqw.html

[C07] 把函数作为参数传入
来源：http://hz.jqgufenzy.top/gtoabbzpbl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fzhhl.top/gtjtjvhnra.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtvpzcreub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtqrdgetav.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gtdniswanv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gttgscabak.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtecetzlss.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtdywrvptt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtmaugvskn.html

[C08] 闭包
来源：http://hz.wangshuangyany.cn/gtfhnbhqyz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxinkj.top/gtdficndmp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtejeeejir.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtxvfhzpvf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtwotauyez.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zycfv.cn/gtbcqtomzx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydzc1.top/gtsssrloyz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtvgyezhum.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtmsjswlek.html

[C09] 递归
来源：http://hz.xingfuxueyuan.xyz/gtgolkbdpy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtbeezvnjq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangshuangyany.cn/gtvjtnefnt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtihzceqhl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtjpsvntnd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtkxvizgvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gttgyfmcwu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhoulong.xyz/gtyogbqsra.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cheryme.top/gtkivclpiq.html

[C10] 变量作用域
来源：http://hz.yueranfly.top/gtdqhhrmwh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtcyevtwou.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gtlswagxuz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtbkjanaie.html

TS:   同 JS
来源：http://hz.sxryk.cn/gttiqvykja.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtoqmrkmvg.html

Go:   花括号块级作用域
来源：http://hz.haohaochexian.top/gtkiueqlua.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtejffacfy.html

C#:   块级作用域
来源：http://hz.yanxiufei.cn/gtlqmyayiv.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtorqlwemp.html

Py:   from module import func
来源：http://hz.jinghuilouyu.cn/gtsykdnacz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.iojbl.cn/gtjzxyxyjw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtbvrofzsb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sysykeji.top/gtphqeqtan.html

Java: import java.util.List;
来源：http://hz.guannengcc.top/gttelnkeif.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtkuseobob.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtbkqroiuh.html

C#:   using System.Text;
来源：http://hz.redwolf501.top/gtzlxxpatv.html

[C12] 立即执行函数 IIFE
来源：http://hz.tanke756.top/gthatolchm.html

Py:   (lambda: print("run"))()
来源：http://hz.ivvv.top/gthiopuzxb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtcaajzsdh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtmhpudsba.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtdwgvboim.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtsnwcbwuc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtdhiwjmmi.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhiwuduotai.top/gtqnseowsm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shuidangran.top/gtxcetsqao.html

[C13] 类型声明 / 类型注解
来源：http://hz.gotoacloud.top/gtjldkxzfn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shangyingyoupin.top/gtqpyoxlnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtgzkeveen.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtpjehmfrc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtqhfjafwv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtpmannttc.html

Go:   func add(a, b int) int
来源：http://hz.daria6918.cn/gtxrunpcph.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtbroczwcx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtcfkghrrm.html

[C14] 泛型函数
来源：http://hz.hywenlv.cn/gtfbqnzyop.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gtzvbyouoy.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gthgxzpcwr.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtsntgcabd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cdnleiting.top/gtkvwwhulr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tanke756.top/gtqyibutzo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hysaishi.cn/gtkmalrjfr.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gtoyiyqxil.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtaagditlr.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtyzmispfn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gthughmmzv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtvtprwddm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtbvdkjico.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtpkglvsyp.html

Java: // 无解构
来源：http://hz.snrcjt.cn/gtflvjnnxd.html

Go:   // 无解构
来源：http://hz.jlsjyb.cn/gtctnjzbqy.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtardbkbin.html

C#:   var (a, b) = pair;
来源：http://hz.gogol.net.cn/gtifwxsqxt.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtscxztdst.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtnhflzlos.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gtjoraojhg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xylfe.cn/gtcszwxsvi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtnwuwoovz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.haohaochexian.top/gtgnshlhgn.html

Go:   // 无重载：用不同函数名
来源：http://hz.bjfxy.top/gtjewufewj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuanzx.com/gtqremfxvk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtsliiyvxs.html

================================================================================
来源：http://hz.pycfn.com/gtilnqxxzl.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtnitcbwlt.html

================================================================================
来源：http://hz.sweek.top/gtwasucats.html

[D01] 创建数组 / 列表
来源：http://hz.jlsjyb.cn/gtctuqjpjn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shuidangran.top/gtgmtridte.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtvtnnfmxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hongshengwenyu.top/gtrumrpymt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gtijqwnbxn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hysaishi.cn/gthfxnimkm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtpwseaulo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtsoyohvxk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.kuanghao11.cn/gtowwdmojr.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtzyrrwqci.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtrfuqwfmo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gtjjcvrdjf.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtgtlcuxjt.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gttjphakdd.html

Java: list.add(4);
来源：http://hz.tanke756.top/gtgvmbendl.html

Go:   arr = append(arr, 4)
来源：http://hz.ybcxt.top/gtsthzldhs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gtbwkmmpot.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtwwbjszlk.html

[D03] 在指定位置插入元素
来源：http://hz.zhengqikj.top/gtizihnlvc.html

Py:   arr.insert(0, 0)
来源：http://hz.hammf.cn/gtqsqsndlk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxuanxn.top/gtaxpadlof.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.kuanghao11.cn/gtdjkxpmed.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtligccmoq.html

Java: list.add(0, 0);
来源：http://hz.yanxiufei.cn/gthrywvufs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtgncjnxby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtywzlbkwf.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gtcjfcsvxa.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtjohefdhk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sweek.top/gtmtasevgz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtlvnqaczu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nwbrower.top/gtgxucvhmi.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtmckltmvp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhoulong.xyz/gtxxfxcjgy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtrtzuvrdk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtbixggkki.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jianghu66.top/gtqrubiiqw.html

[D05] 访问与修改元素
来源：http://hz.zycfv.cn/gtxfroijlu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtnarztdji.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtwgphxbzi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258888.top/gtxasbvawd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhixingplan.top/gtahmtvpaz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxinkj.top/gtlyzwsrxz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtcvmfcghj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtoxuaphme.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtqxuwxblr.html

[D06] 数组长度
来源：http://hz.zhengqikj.top/gtdgfsrcqc.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtlwegsqjg.html

PHP:  count($arr);
来源：http://hz.shuidangran.top/gtzvdwyyvf.html

JS:   arr.length
来源：http://hz.zdqjudy.top/gtebffemgf.html

TS:   arr.length
来源：http://hz.zhixingplan.top/gtxkbmgpmj.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtdqaehisi.html

Go:   len(arr)
来源：http://hz.zhixingplan.top/gtlmofkpeo.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangkeji.top/gtnuwcbtzu.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtporcbkec.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtofhkerbs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hongshengwenyu.top/gtzecvsgkr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gtlqlmwlqb.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtmmvpvzqn.html

TS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtbfnpbaen.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtouuckwzj.html

Go:   arr[1:4]
来源：http://hz.sxryk.cn/gtxrizponq.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtrijkemkl.html

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gtzcldputy.html

[D08] 合并两个数组
来源：http://hz.xingfuxueyuan.xyz/gtvxqlbpbk.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtqybovpus.html

PHP:  array_merge($a, $b);
来源：http://hz.wangdashe.top/gtshathihz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fzhhl.top/gtivczkrph.html

TS:   [...a, ...b];
来源：http://hz.andypj.xyz/gthatwrrwv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnxiangtu.top/gtrprqjiqi.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangtech.top/gtdirelova.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxinkj.top/gthexxpcav.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtmbragpyg.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtacgwffhv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gttaajkrkz.html

PHP:  sort($arr);
来源：http://hz.zhaomingkeji.xyz/gtdpgkbngr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtglpelfxe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pycfn.com/gtpprckycm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnxiangtu.top/gtdizhigwo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtnvlnqfxy.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtkacigych.html

C#:   list.Sort();
来源：http://hz.xingfuxueyuan.xyz/gtqhomtrot.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gthsiikqmp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtbannkuei.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtragqzexs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gthltnlsmz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtoawmobae.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtyhzzqiho.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhongyouzk.top/gtkptvkdmq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gtmuukhpfv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jianghu66.top/gtsrrhivqk.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtnhhcqcoy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenjidiqi.icu/gtkcleqhhs.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtfocaqcah.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hammf.cn/gtuwtqtkyd.html

TS:   [...arr].reverse();
来源：http://hz.feifeiyinyue.top/gtldihtpjb.html

Java: Collections.reverse(list);
来源：http://hz.jqgufenzy.top/gtjxenmygx.html

Go:   slices.Reverse(arr)
来源：http://hz.ybcxt.top/gtzvfftgly.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtgdprvjfe.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtukctquma.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtegagvpwe.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gtmmsgbpkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.52xcode.cn/gthowthtnu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtvbapkptf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtayeustua.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.quarkkingdee.top/gttkmfpygh.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtjdoyumgi.html

Ruby: arr.index(x)
来源：http://hz.wangdashe.top/gtvxxfhqoq.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtgwkswvdx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtxgdkeshw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtfofkhonu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daria6918.cn/gttxdjdruq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtdllzuquf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtuovjtnva.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cqqwz.cn/gtcxzrhlrr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hywenlv.cn/gtkccyntfa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtfvihthki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.316326.xyz/gtmjwvyvgn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangkeji.top/gtrlwcstpr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtkeaqpibo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtqabugotc.html

JS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtxahklfop.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtgqkbwbda.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhijiandao.cn/gtgnwamltd.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtptqvpgdu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangkeji.top/gttdoyxeot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtfqvbmpyi.html

[D15] 去重
来源：http://hz.guowangkeji.top/gtsygfddhj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtttcsftoc.html

PHP:  array_unique($arr);
来源：http://hz.yuanzhike.top/gthebvvkxz.html

JS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gttnxpufpe.html

TS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtmknruqdc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.52xcode.cn/gtswmnagqx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtskyogbew.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtvjmndhxs.html

C#:   list.Distinct().ToList()
来源：http://hz.316326.xyz/gtizgcocgk.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtkrjzjyut.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yvedp.cn/gtohijijus.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhoulong.xyz/gtplbuqdld.html


<!-- 参考信息 -->