代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtdbcdlinp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtxivmitxb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shzxlz.cn/gtxtdcdfyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtjorabcgs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtmzcknxdp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.birdmap.top/gtwegzmwaj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jlsjyb.cn/gtwfesfekq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtbniccnwp.html

[C02] 默认参数
来源：http://hz.wangshuangyany.cn/gtducttetd.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gteovxvvba.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenjidiqi.icu/gtaetbwysy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.316326.xyz/gtcaesztfv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.c1oappe.top/gtvrophdcu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtqviywgya.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.svipenyu.cn/gtilxnbfai.html

Ruby: def greet(name = "World") = name
来源：http://hz.shuidangran.top/gtlbxznomq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhongyouzk.top/gtnitjqcbg.html

[C03] 可变参数
来源：http://hz.316326.xyz/gtaotwtybc.html

Py:   def total(*args): return sum(args)
来源：http://hz.vqdsnc.cn/gtlimfwfjt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tianlin.xyz/gtwxdkhkaa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtjkanwvek.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtuboeatkr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gtynxssrkb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtdpbfvurv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xylfe.cn/gtbltydagf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtowxpztqq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxuanxn.top/gtfjbphrlj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydjk.org.cn/gtpwynxsqz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxuanxn.top/gtooeebjgp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtrlmjukid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtfxkxaqtw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tanke756.top/gtvhxjrnpj.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gteueqkpbu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtrzzovaev.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtpoktjmut.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gtcpxtqhis.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gtgbloppae.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtafcmmxlb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhoulong.xyz/gtjmdkaoyu.html

TS:   return { a, b };
来源：http://hz.cheryme.top/gtevzhhuaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtsutmgroe.html

Go:   return a, b
来源：http://hz.redwolf501.top/gtzbpzsbki.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtzojodhxo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtjokamjvy.html

[C06] 匿名函数 / lambda
来源：http://hz.ywan-chungtsiang.top/gtoohcfiny.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtalhszzkf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtfsvjlthi.html

JS:   const square = x => x * x;
来源：http://hz.wangdashe.top/gtmgdfvmew.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenzaomai.com/gtnvzjlrwb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenjidiqi.icu/gticcfldfi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtrehqiqjo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuetiantiany.cn/gttzvnwxna.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtpieizxhc.html

[C07] 把函数作为参数传入
来源：http://hz.0kj1m.cn/gtrlcyyiod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuanzhike.top/gtorcykwra.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.316326.xyz/gtbbnmupod.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtptnzqpiz.html

TS:   arr.map(String)
来源：http://hz.cdnleiting.top/gthhcxfdzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.havefunace.top/gtambfelpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gteqwucewn.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj202588.top/gthlzydyvj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cqqwz.cn/gtlkpmsbri.html

[C08] 闭包
来源：http://hz.aizwys.cn/gtrkhnnuyi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtqvemlhpj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtdoretoye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtvmpullew.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtlqjeulda.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.birdmap.top/gtmxlybzmi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jianghu66.top/gtaepxsrfu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.bjfxy.top/gtilehzkml.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtjhuewmpg.html

[C09] 递归
来源：http://hz.nanxuanxn.top/gtqgpejbuh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtzvwfxxri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.snrcjt.cn/gtuspsonga.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtcdgkzmcw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtqdpmrwjx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.snrcjt.cn/gtgttixsvj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cucudq.cn/gtofvvzxdq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jianghu66.top/gtnvlevfgq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pengpengdd.cyou/gtwfjkfafh.html

[C10] 变量作用域
来源：http://hz.chenzaomai.com/gtdjsliovf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gttucjcyyi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhaomingkeji.xyz/gtufaxzoqu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtseaygphe.html

TS:   同 JS
来源：http://hz.pengpengdd.cyou/gtrfiuncdj.html

Java: 方法内为块级作用域
来源：http://hz.chenjidiqi.icu/gtadmuibgj.html

Go:   花括号块级作用域
来源：http://hz.sysykeji.top/gtmbjtrdsx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.iojbl.cn/gtgirncsrw.html

C#:   块级作用域
来源：http://hz.zhijiandao.cn/gtjipyenri.html

[C11] 模块导入与导出
来源：http://hz.zhaomingkeji.xyz/gttipzbopq.html

Py:   from module import func
来源：http://hz.9152youxi.cn/gtjlhpynpl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenzaomai.com/gtvynzvode.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtsyoyuxft.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtqakhxjgo.html

Java: import java.util.List;
来源：http://hz.guowangkeji.top/gtjrbfnxql.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gogol.net.cn/gtjfqjcskq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sysykeji.top/gtpdrblkvo.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtprxpadae.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gthidnktco.html

Py:   (lambda: print("run"))()
来源：http://hz.andypj.xyz/gthdenmalz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yongpay.top/gttdxybtng.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtztasobuf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtxjkwzgrm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ywan-chungtsiang.top/gtqlqpxbhf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtglrjseha.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtkfcowmgk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gtwgfdzlig.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtgnzssjrb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtoszumbye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtliazvulw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fengsongda.top/gtuljmozrn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtzzycjhev.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtgqlbetxq.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gtyiiyrckn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtrwwuguba.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtivhwmemr.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtooxseyqe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sufxvd.cn/gtguyfznfy.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gtwteeuwji.html

JS:   // 无泛型
来源：http://hz.yj20258888.top/gtjafoygpn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtvirbkqxr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtcpnddtzm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtnkhzjcrt.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtrrxkolqm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtpijqivkg.html

[C15] 解构 / 展开参数
来源：http://hz.yongpay.top/gtymlfrzjt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.bjfxy.top/gtnofmvxqp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtoapftgru.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.52xcode.cn/gtlmkkeprq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtnfvfcgup.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtwcwositm.html

Go:   // 无解构
来源：http://hz.aibaodan.cn/gtxibxhwhs.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtzelvfnpy.html

C#:   var (a, b) = pair;
来源：http://hz.hnqzz.top/gtwrcwlchh.html

[C16] 函数 / 方法重载
来源：http://hz.zhongyouzk.top/gtdwsrepwy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fzhhl.top/gtmhphdipj.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtcnngaifo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtpasuitld.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtvvpjfzcg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yangfankeji.com/gtdvfjhyyt.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtbknndgyz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhoulong.xyz/gtsnkwmezb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gthgyjmkyx.html

================================================================================
来源：http://hz.wangdashe.top/gtfupgkmot.html

D. 数组 / 列表 / 集合
来源：http://hz.fengsongda.top/gtpvyjwdzb.html

================================================================================
来源：http://hz.ydzc1.top/gtjmuobvwv.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtmdizbhcy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jqgfzy.top/gtvtlqukwu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gttygfeqqv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtygwtshnx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtkmonrndy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dianchejie.cn/gtiejsgbiy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yongpay.top/gtuwcanfff.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtxabdnqrb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtbbfgpwyq.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtsyvqfsrd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtktatuvfn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtimkcikzg.html

JS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtygjztirv.html

TS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtxcaovnsm.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtmmsrtoze.html

Go:   arr = append(arr, 4)
来源：http://hz.redwolf501.top/gttfiljvot.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtvrwjwile.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gtgvglmygr.html

[D03] 在指定位置插入元素
来源：http://hz.ybcxt.top/gtaywifszj.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtkskmavzw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtyojrchlg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yangfankeji.com/gtdcahnaye.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtbwcijwtt.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtmgnrpphm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtusbjgpmy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.andypj.xyz/gteapeapjr.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtrojshnge.html

[D04] 删除元素
来源：http://hz.smart0.xyz/gtmvfhhtjr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtyidxukmr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuanzhike.top/gtrlxagpis.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtyhfzzgkq.html

TS:   arr.splice(0, 1);
来源：http://hz.ivvv.top/gtiagsblpu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtzsngfvln.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.kuanghao11.cn/gteorpdmeq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sufxvd.cn/gtinlbafnu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtrtvfzfty.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtsogzlzai.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gthsorfqzn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtbnadmbsl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtizljqdrz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fengsongda.top/gtgobivuoa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtxmvwjiau.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtmijfwwnr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gturnduhpn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtalqcwcmz.html

[D06] 数组长度
来源：http://hz.ivvv.top/gtetifgihe.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtmnzjwlxw.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtbyecvnfx.html

JS:   arr.length
来源：http://hz.sweek.top/gtqypmgvzb.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtqahgezfs.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtscubjpmp.html

Go:   len(arr)
来源：http://hz.hongshengwenyu.top/gtfbcguhsm.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtchjgnbay.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtkkkrzygl.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gttzzygctf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gtqkzxrkkr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtckrrzrls.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gturacvyoa.html

TS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtdtdsbggn.html

Java: list.subList(1, 4);
来源：http://hz.jlsjyb.cn/gtctnptgna.html

Go:   arr[1:4]
来源：http://hz.aizwys.cn/gtxubalzfa.html

Ruby: arr[1, 3]
来源：http://hz.ydzc1.top/gtmadybeyk.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtzvbunoxt.html

[D08] 合并两个数组
来源：http://hz.zdqjudy.top/gtlpgfrrjm.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtzvnxzrlo.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtjpuxrafi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtnxduzwyn.html

TS:   [...a, ...b];
来源：http://hz.316326.xyz/gtfydlxkvo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtwkxekoxs.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtpzffoptp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gtakudfovb.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtaysmmkxt.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtyisfyrxp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtecsusrhp.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtbscmnhqf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtjaewxjyd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtepflmnus.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yueranfly.top/gtbplwfnvi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.316326.xyz/gtjxzupsed.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtxhtttiix.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtysrlhjgs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tianlin.xyz/gtszewoxae.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtqibpedzf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gthgxkbifv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtykdfxcep.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gthirridww.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.0kj1m.cn/gttttfjkww.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtrjdoejiw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtyvpgcztl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtdcjrjqqh.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtjjakhang.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gtcktwntgy.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtkdwntnlo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtodrgxeln.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtwbaxawob.html

Java: Collections.reverse(list);
来源：http://hz.gaohongyu789.top/gthmrvepkk.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtuvthxnrl.html

Ruby: arr.reverse
来源：http://hz.gogol.net.cn/gtkdhjojdf.html

C#:   list.Reverse();
来源：http://hz.yj20258888.top/gtfbrbgxgg.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangkeji.top/gtqxjgkfak.html

Py:   arr.index(x);  x in arr
来源：http://hz.quarkkingdee.top/gtjgnnxtrx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.52xcode.cn/gtmrrzgjmw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuetiantiany.cn/gtmilfthaj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gttjkgjyzp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtbookhogt.html

Go:   slices.Index(arr, x)
来源：http://hz.vqdsnc.cn/gtnzhyodyq.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtymkycrst.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtbztlhbda.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuetiantiany.cn/gtfayitbix.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtdvyuhisn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gthsuzsdbn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gthugqysml.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtxjhjjxla.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtwzxjwjfs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gtrzmsosag.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cdnleiting.top/gtfymeawgt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtgqnsrvcj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sufxvd.cn/gtbcauwctc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aibaodan.cn/gtwhfqpfsi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtptwiovbq.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtggjsynyi.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtnnjnrgeq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.quarkkingdee.top/gtjapylwun.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtbifxwszc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtuoauofvx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shzxlz.cn/gtbnyagrzz.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtxlvjttpo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gtmoqlcfkb.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtmqmakxcs.html

JS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtimuephib.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtdsashgjh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cheryme.top/gtutrjpdzx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.0kj1m.cn/gtqhtboprk.html

Ruby: arr.uniq
来源：http://hz.jinqigfzy.top/gtgyecgjhb.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gtdohthpyc.html

[D16] 求和与平均值
来源：http://hz.zhaomingkeji.xyz/gtssnfsjqt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtqwkiupze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtvbnhdgiq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtkzwpkbbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtfehfwxle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gthgotbzll.html

Go:   // 手写循环累加
来源：http://hz.xuanzx.com/gtlsxgaovw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yvedp.cn/gtgzfjpkhj.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtighgknsu.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtpxvlwhqa.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtkilouzbq.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtgpxbkazu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtqpklzbqb.html

TS:   Math.max(...arr);
来源：http://hz.tian-w.cn/gtwyjfdhzo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yangfankeji.com/gtzbmmuuid.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtabczqfyc.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtmjcpeokm.html

C#:   list.Max();  list.Min()
来源：http://hz.jlsjyb.cn/gtoairryng.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gtxtbofqmf.html


<!-- 参考信息 -->