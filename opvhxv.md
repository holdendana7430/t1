代发 wailian999

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtgsayicxh.html

JS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtpbbiytbj.html

TS:   a && b || !c
来源：http://hz.shuidangran.top/gtsedkkigf.html

Java: a && b || !c
来源：http://hz.wangdashe.top/gtadyuanhs.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gtvxuvtwnj.html

Ruby: a && b || !c
来源：http://hz.chenjidiqi.icu/gtzhetqytu.html

C#:   a && b || !c
来源：http://hz.sxryk.cn/gtrntzzkec.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnxiangtu.top/gtqycbhyuf.html

Py:   if not data: return
来源：http://hz.aizwys.cn/gtnubncapl.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtbtpycidu.html

JS:   if (!data) return;
来源：http://hz.tanke756.top/gtnvnhcwoq.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtjarrczkh.html

Java: if (data == null) return;
来源：http://hz.zycfv.cn/gttgpaqyrl.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gthyitouij.html

Ruby: return if data.nil?
来源：http://hz.ybcxt.top/gtzmbpowfa.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gtkmibvrsi.html

================================================================================
来源：http://hz.dianchejie.cn/gtrrtychjx.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtaiuiwqhk.html

================================================================================
来源：http://hz.wangdashe.top/gtxrpfvpup.html

[C01] 定义函数
来源：http://hz.jinghuilouyu.cn/gtfmdxxrps.html

Py:   def add(a, b): return a + b
来源：http://hz.wangshuangyany.cn/gtujhtbiwu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtcqcuwksr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtulkwbhhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtuzqzyroz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtypluqhyq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jiagoushi.top/gtdzzdefrp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhengqikj.top/gtcdyvgquy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtwqnriblm.html

[C02] 默认参数
来源：http://hz.chenzaomai.com/gtgwzcyzpe.html

Py:   def greet(name="World"): return name
来源：http://hz.birdmap.top/gtffcldcwu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jyoumei.cn/gtethjhqbl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtbdwovyyh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtjtlyuuzy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shzxlz.cn/gtfqtkmmsc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtlamsaupd.html

Ruby: def greet(name = "World") = name
来源：http://hz.hywenlv.cn/gtacfxjkxr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinghuilouyu.cn/gtqxtwvvhu.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gtlpezfegj.html

Py:   def total(*args): return sum(args)
来源：http://hz.hysaishi.cn/gtipzkmnmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ehwqpu.com/gttkbskryr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtegnsykfs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cashguo.top/gtwyomecmo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtpftnlqhc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtrppesqay.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtnvnwekhl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.vqdsnc.cn/gtcjzlcyre.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gttzdrergt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtvhyieiga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nwbrower.top/gtrllshxui.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtevsgkuyu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shangyingyoupin.top/gtlbszkthy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xinyue.icu/gtunessvor.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtxcubnkrs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gttsgtlzpy.html

C#:   f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtcbtgpoys.html

[C05] 返回多个值
来源：http://hz.hammf.cn/gtwotnebuh.html

Py:   return a, b
来源：http://hz.hammf.cn/gtcthbiwah.html

PHP:  return [$a, $b];
来源：http://hz.yangfankeji.com/gtmmepzwha.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtxmanqgdi.html

TS:   return { a, b };
来源：http://hz.cucudq.cn/gtzimworoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258.top/gtziindybt.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtjnojqxni.html

Ruby: return a, b
来源：http://hz.zdqjudy.top/gtgkmhxtsa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.c1oappe.top/gtfisxcbko.html

[C06] 匿名函数 / lambda
来源：http://hz.chenzaomai.com/gtihbxqgjb.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258888.top/gtbjtgsicl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gtkiaobyai.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtuskrepol.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgfzy.top/gtpzslfbue.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtbkadnoed.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtzjddxpkw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinghuilouyu.cn/gtzllbfkmn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtwavnpauk.html

[C07] 把函数作为参数传入
来源：http://hz.nanxinkj.top/gtpqlpiwfs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydzc1.top/gtuawhmbva.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.52xcode.cn/gtfqleluad.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhiwuduotai.top/gtebftetnh.html

TS:   arr.map(String)
来源：http://hz.zdqjudy.top/gtzshjjurt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnqzz.top/gtqbrtvqng.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtlcmgbqks.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258888.top/gtmqvhnkek.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gthhnbsgcp.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtoaspjrmc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhengqikj.top/gtwxtojoiv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenlongwang.top/gtcoeemrjb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtrcothevw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtsztlqqxe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yvedp.cn/gtpjbwhghv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtychilzho.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tianlin.xyz/gtaupkgarh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtfnfqbbhu.html

[C09] 递归
来源：http://hz.chenlongwang.top/gttgrdatlr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258888.top/gtaimtxmjo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yangfankeji.com/gtpkcvfnal.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gteiepafiw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtkidgzylh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.svipenyu.cn/gtyxmvoioj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.svipenyu.cn/gtgiopijwb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pycfn.com/gtwuxiwepm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtdtrtesre.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtlajshzvv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.feifeiyinyue.top/gtcpzpzfdk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangshuangyany.cn/gtsmeacmwx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gtjbpprxpg.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtzxakhbvz.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtxdibcpuo.html

Go:   花括号块级作用域
来源：http://hz.0kj1m.cn/gtohstvgsl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigfzy.top/gtwzdcfbfx.html

C#:   块级作用域
来源：http://hz.jqgufenzy.top/gttqjvbict.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtvhpgizzq.html

Py:   from module import func
来源：http://hz.kuanghao11.cn/gtidhzanhd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenjidiqi.icu/gttfgokfmc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtpjihjpno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ehwqpu.com/gtpxsmqkha.html

Java: import java.util.List;
来源：http://hz.cashguo.top/gtcdyqpffp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.smart0.xyz/gtskenhrtw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydjk.org.cn/gtxbvqddxz.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtdabpxess.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhiwuduotai.top/gtckhgxegt.html

Py:   (lambda: print("run"))()
来源：http://hz.jyoumei.cn/gtkxmcszqn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gogol.net.cn/gtnacqfwrv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.snrcjt.cn/gttrsnbdau.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtfivlzfao.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tianlin.xyz/gtclxghnbw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigufen.top/gtklsufmxa.html

Ruby: -> { puts "run" }.call
来源：http://hz.shzxlz.cn/gtltrgekau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yueranfly.top/gtxpnlahep.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnqzz.top/gtvhherunw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtktbbduee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtthplmlnt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtahmxtkfz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtusxeicfv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtxakmiajy.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtgzsnhnyc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gttbsoatsm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhongyouzk.top/gtowpkawdd.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gtkvbfluuy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gtyvakgsrh.html

PHP:  // 无泛型
来源：http://hz.ybcxt.top/gtzfqvwrgo.html

JS:   // 无泛型
来源：http://hz.yj20258888.top/gtaucmpmqy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtpzwuqwuk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gthrhirqdl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gtfloqxpaf.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtjjfdbswn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gtjwylautt.html

[C15] 解构 / 展开参数
来源：http://hz.zhoulong.xyz/gtntugbsmy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtdkxcjbqs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtmlczcbvz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtcrodwevl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigfzy.top/gtkukyqfqb.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtelraubok.html

Go:   // 无解构
来源：http://hz.gzhubu.top/gtkeomebfu.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtjwnmrljb.html

C#:   var (a, b) = pair;
来源：http://hz.ppjwa.cn/gteksjklci.html

[C16] 函数 / 方法重载
来源：http://hz.hnxiangtu.top/gtrvshiqdf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gtiiwczfqz.html

PHP:  // 无重载
来源：http://hz.sufxvd.cn/gtjindsztg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtedhvvjrw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtvcstbzca.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gtlzscjyol.html

Go:   // 无重载：用不同函数名
来源：http://hz.haohaochexian.top/gtuszyxnrt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtikkpadvf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtbsnwtros.html

================================================================================
来源：http://hz.andypj.xyz/gtvjvogwmi.html

D. 数组 / 列表 / 集合
来源：http://hz.shuidangran.top/gtdwfiqszy.html

================================================================================
来源：http://hz.tianlin.xyz/gtqbugnlrz.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gtpibburpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtczcfzdjc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtcqbnoxlh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtoiymmvhe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.mhx1999.top/gtjjyxduml.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtygwrmkug.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtzyjczkgi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aibaodan.cn/gtepivvnzc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtilpggzhx.html

[D02] 追加元素到末尾
来源：http://hz.mhx1999.top/gtjdxvqcar.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinyuanbaomall.cn/gtrbgvkyrl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgfzy.top/gtxtwyokmt.html

JS:   arr.push(4);
来源：http://hz.aizwys.cn/gtltxytllc.html

TS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtkdmrcnpc.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtxeoiffkr.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtxnbgxrcz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtmqwcatex.html

C#:   list.Add(4);
来源：http://hz.ppjwa.cn/gtjetdnyyo.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtqwhqvjhk.html

Py:   arr.insert(0, 0)
来源：http://hz.shuidangran.top/gtknlyeesl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xingfuxueyuan.xyz/gtlvbihzvy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daria6918.cn/gtyzeubldw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258888.top/gtxgbddqho.html

Java: list.add(0, 0);
来源：http://hz.yuxming.cn/gtoehvtbeb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cashguo.top/gttiflvatd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cdnleiting.top/gtfqpjzgap.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxinkj.top/gtvxgqdiji.html

[D04] 删除元素
来源：http://hz.0kj1m.cn/gtotgjegic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pycfn.com/gtjmefbizq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gthcstvduz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtiqlrhdfr.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtnqawsvhp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtrgpylcbw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.fengsongda.top/gtkllhkewj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.feifeiyinyue.top/gtyljgnzmc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jiagoushi.top/gttgrpoywm.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtrqxklfnm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtfmvighxa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shzxlz.cn/gtdifzkbhk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtrbbpjbfs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.316326.xyz/gticdyeovl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtdgkymfhv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtjzhoxhyj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtrzqeezlf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigufen.top/gttogpilnp.html

[D06] 数组长度
来源：http://hz.sweek.top/gttxgdhjuj.html

Py:   len(arr)
来源：http://hz.mhx1999.top/gtaoubbjjb.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtxuhmygao.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtfqhzusap.html

TS:   arr.length
来源：http://hz.zhijiandao.cn/gtidepjabs.html

Java: list.size();
来源：http://hz.fzhhl.top/gtikduigza.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtsayikvbf.html

Ruby: arr.length; arr.size
来源：http://hz.mhx1999.top/gtzzgxoffq.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gtcgtgfrwy.html

[D07] 切片 / 取子数组
来源：http://hz.zhijiandao.cn/gtaqkonjsq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258888.top/gtyskzjthi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.haohaochexian.top/gtuxkffcch.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtgvahiicd.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gthdsiyvil.html

Java: list.subList(1, 4);
来源：http://hz.bjfxy.top/gtmzwxujrc.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gtudrqfnyw.html

Ruby: arr[1, 3]
来源：http://hz.cashguo.top/gtqgendqtc.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtlqditacx.html

[D08] 合并两个数组
来源：http://hz.havefunace.top/gtgqbygopu.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtjdmbbvdm.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtesuboznl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtqtckpgze.html

TS:   [...a, ...b];
来源：http://hz.cdnleiting.top/gtgkzcldut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gotoacloud.top/gtsdiihfgc.html

Go:   append(a, b...)
来源：http://hz.yongpay.top/gtxddrxqvq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtaqtjpsuu.html

C#:   a.Concat(b).ToList()
来源：http://hz.shzxlz.cn/gtmusasjhq.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtolegmdgj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtszfbkrfp.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtzjqhgzgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gttqqhznvl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtlkqzkwiw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fzhhl.top/gtwazfydke.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ybcxt.top/gtliumdkox.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtgdfabdue.html

C#:   list.Sort();
来源：http://hz.guowangkeji.top/gtemzbxepe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtxotditvm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.smart0.xyz/gtoldntioy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtwicfvpow.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gteizxqnpw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtbztmubwo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtjsbtrpgq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtfvsgiyvd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtydnuwqmu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hywenlv.cn/gteddblonb.html

[D11] 反转数组
来源：http://hz.zhoulong.xyz/gttcnibrje.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtrayzfdrl.html

PHP:  array_reverse($arr);
来源：http://hz.tanke756.top/gtoobusfly.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gtiovhljnm.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtziujfdar.html

Java: Collections.reverse(list);
来源：http://hz.wangdashe.top/gtauzrdhxg.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtzabscazm.html

Ruby: arr.reverse
来源：http://hz.xziqi.cn/gteycjvnjc.html

C#:   list.Reverse();
来源：http://hz.kuanghao11.cn/gtnupiceib.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gttjtmhfvi.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gttfmiizkp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sysykeji.top/gtnkbspkdh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtfwpfooqr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtmljyawub.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hysaishi.cn/gtnzazcaxs.html

Go:   slices.Index(arr, x)
来源：http://hz.pengpengdd.cyou/gtjteibgil.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtomncdmpu.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gthfrtmoyi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtjwnvgeea.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.c1oappe.top/gthdjrwrsk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtfkcyfvxp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtutkqoxvp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtdwlvjgtn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtrpleyqmp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtzsnxoffe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhongyouzk.top/gtkhvuqxdx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tian-w.cn/gtxcxhrpdd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtfysyzezj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigfzy.top/gtqhlkbaep.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtrhgsoyso.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtnhunyiay.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtbndfinzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtuyirwwgg.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtgltulead.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jyoumei.cn/gtbiptdjfp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.andypj.xyz/gtemtewsre.html

[D15] 去重
来源：http://hz.pengpengdd.cyou/gtnkwbfmvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtpiccanhq.html

PHP:  array_unique($arr);
来源：http://hz.cdnleiting.top/gtdxvzowrm.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gttrwvtbri.html

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtfzyvilxp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtynugykzc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtjepmsohk.html

Ruby: arr.uniq
来源：http://hz.chenlongwang.top/gtuvxzeait.html


<!-- 参考信息 -->