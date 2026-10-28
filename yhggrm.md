代发 wailian999

================================================================================
来源：http://hz.shzxlz.cn/gtqdbdmfsj.html

C. 函数与作用域
来源：http://hz.quarkkingdee.top/gtozunhbsc.html

================================================================================
来源：http://hz.daxiang520.top/gtpuevqzvx.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtqzwkdanm.html

Py:   def add(a, b): return a + b
来源：http://hz.tianlin.xyz/gtbmemhcfp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtytgvdhwd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.guowangkeji.top/gtyjemlznl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtqkgwcqju.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtfdlebkib.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtzylcgdpj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtpanlwfnn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtablyjxkc.html

[C02] 默认参数
来源：http://hz.jinqigfzy.top/gtqambncjs.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxinkj.top/gtqaeldlaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtgkxmqvla.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.birdmap.top/gtwkvjlcsi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gzhubu.top/gtiugyxdnt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtxgnvyyvu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.9152youxi.cn/gtntzomkpb.html

Ruby: def greet(name = "World") = name
来源：http://hz.haohaochexian.top/gtiwlleptf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtinqktmzy.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtkbbzcbmr.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gtbnndqwqo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shzxlz.cn/gtrjqymopo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nwbrower.top/gtcmbaqukg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gteizpkgze.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtiasxtqmx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhaomingkeji.xyz/gtjgidrzja.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtdnxfqkma.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtqkbbacmx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gtrllotqfm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hysaishi.cn/gtvfmetaab.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigfzy.top/gtviaflobo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtetgdxvpv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxinkj.top/gtbfdipqkn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhixingplan.top/gtbxrirpek.html

Go:   // 无：用配置结构体参数
来源：http://hz.bjfxy.top/gtdxbhuoqt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gthlwenudr.html

C#:   f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtbkqohwxq.html

[C05] 返回多个值
来源：http://hz.cdnleiting.top/gthzejbgku.html

Py:   return a, b
来源：http://hz.gaohongyu789.top/gtsasjvhql.html

PHP:  return [$a, $b];
来源：http://hz.redwolf501.top/gtbhfsnfas.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtkvhpwmsi.html

TS:   return { a, b };
来源：http://hz.hongshengwenyu.top/gtzkfnjkhc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuxming.cn/gtgstvnwda.html

Go:   return a, b
来源：http://hz.zhoulong.xyz/gtrrxhdbyt.html

Ruby: return a, b
来源：http://hz.pengpengdd.cyou/gtdqafvahy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gttgpviiib.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtmhqowujp.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtjilaoocp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zdqjudy.top/gthglzaqci.html

JS:   const square = x => x * x;
来源：http://hz.tanke756.top/gtekpochxn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj20258.top/gthyfainjl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtlilkmgxy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hywenlv.cn/gtpqbeawvw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gthvxdwlqt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtllgftjvu.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtghwovbxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gaohongyu789.top/gttzwxlwdu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cashguo.top/gtgdnqzolp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ehwqpu.com/gtzwrbginw.html

TS:   arr.map(String)
来源：http://hz.haohaochexian.top/gtqvnwbcqk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.snrcjt.cn/gtsfefvxxn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtvvphavot.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigfzy.top/gtmzgunabh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinghuilouyu.cn/gtnjpgcnyt.html

[C08] 闭包
来源：http://hz.yongpay.top/gtxrsqzszj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtbynfqbxl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtccuqykzi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtmtdkkftv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtrqyzvavp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtsyldynyj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtpzvhpmxh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hnxiangtu.top/gtkphqkxog.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtqlddoysh.html

[C09] 递归
来源：http://hz.andypj.xyz/gtljwcgjyg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtpflnctqq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.quarkkingdee.top/gtqowggkmv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtwhwbeqec.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtslxkmklk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fzhhl.top/gtehajpxpc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aizwys.cn/gtqrlycomu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtwkoecqqo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtbhtomqhz.html

[C10] 变量作用域
来源：http://hz.hongshengwenyu.top/gthdqvtmbx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.bjfxy.top/gtqttglpmn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtvalqgdew.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxuanxn.top/gtjseeumnu.html

TS:   同 JS
来源：http://hz.andypj.xyz/gticjktwox.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gttrsxoacw.html

Go:   花括号块级作用域
来源：http://hz.quarkkingdee.top/gtkncmigrr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guowangkeji.top/gtlwyqohkk.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtpbrozpzz.html

[C11] 模块导入与导出
来源：http://hz.havefunace.top/gtjfnugczm.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtencxcgjs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnxiangtu.top/gtichnknvb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xinyue.icu/gthjdkbadi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.birdmap.top/gtgbsluqvm.html

Java: import java.util.List;
来源：http://hz.redwolf501.top/gtnpfdwfdc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtldwxawsp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yongpay.top/gtibcjkesy.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gtdxgvjrny.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gttpsxxdqq.html

Py:   (lambda: print("run"))()
来源：http://hz.fengsongda.top/gtecsszehk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gteksztqqv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gttpzgmbvi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtknxvpefg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtibjiohbb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtdwpzynws.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtvccwxezb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtwysnlulg.html

[C13] 类型声明 / 类型注解
来源：http://hz.gotoacloud.top/gtvobogpjo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gtdispznep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtcyqaflxy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtpngnuqlt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtgojvwbqh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtraimokvn.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtusmubcel.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenjidiqi.icu/gtdzpxuwdu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.andypj.xyz/gtmjyshrps.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtetlivvwe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtuiyvsnoj.html

PHP:  // 无泛型
来源：http://hz.tian-w.cn/gtotbngftd.html

JS:   // 无泛型
来源：http://hz.jiagoushi.top/gtpvpdccwk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigfzy.top/gtmtypuhna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.smart0.xyz/gtaemkdzex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtpvknsnfw.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtgwnzwbvk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gteddkywcf.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gteadjrhvl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daria6918.cn/gtjvhpniud.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtxcidkgck.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xziqi.cn/gtrlmsdabc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtjlbmrwrm.html

Java: // 无解构
来源：http://hz.yj20258.top/gtvnqegjlt.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtrtospuzf.html

Ruby: a, b = pair
来源：http://hz.zhixingplan.top/gtvdkmdrka.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtliayvzpn.html

[C16] 函数 / 方法重载
来源：http://hz.daria6918.cn/gtaknqwvjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgfzy.top/gtupafpdqy.html

PHP:  // 无重载
来源：http://hz.hongshengwenyu.top/gtprtufgip.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuanzx.com/gtxdbuaykh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hammf.cn/gtekmlslct.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtsqeswosp.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnqzz.top/gtcftxtaby.html

Ruby: # 无重载：靠动态参数
来源：http://hz.vqdsnc.cn/gtnmhezzfr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgufenzy.top/gtxpnzakre.html

================================================================================
来源：http://hz.chenlongwang.top/gtifucfkdo.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtiejmnklr.html

================================================================================
来源：http://hz.jinqigufen.top/gtjqkxcnoy.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtbawcyklb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinyuanbaomall.cn/gtinuafjwp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zdqjudy.top/gtmsgdmvek.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtxequwsno.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jianghu66.top/gtklzirdry.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258.top/gtmuqdexah.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hnqzz.top/gtujlftgwh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gtbfxhqcga.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtczbktgbd.html

[D02] 追加元素到末尾
来源：http://hz.zdqjudy.top/gtocbynqws.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtotyyyjvi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtiumembqg.html

JS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtvdawcimx.html

TS:   arr.push(4);
来源：http://hz.tian-w.cn/gtixslamza.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtjxncautj.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtlykzjuok.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangkeji.top/gtvplqdunb.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtutqvidxj.html

[D03] 在指定位置插入元素
来源：http://hz.nanxinkj.top/gtmzqskhay.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtcngsokxt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gtpotbetyn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gtybaidsmp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhongyouzk.top/gtgrlsvsgb.html

Java: list.add(0, 0);
来源：http://hz.guowangkeji.top/gtbzdgtrqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtsperrmwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jiagoushi.top/gtmasadltg.html

C#:   list.Insert(0, 0);
来源：http://hz.cucudq.cn/gtiaqoagbt.html

[D04] 删除元素
来源：http://hz.andypj.xyz/gtghhqgnnc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dianchejie.cn/gtersxaein.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtbbllgauo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtbiaufrso.html

TS:   arr.splice(0, 1);
来源：http://hz.birdmap.top/gtxeewgory.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtfhtomubr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.kuanghao11.cn/gtssvmqdcv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuanzhike.top/gtcukjyioq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtqnkzcaon.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gttsyhzyul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtlaeiwcdx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtsutazagd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtqskqkthv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtgkbtweij.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtyimquoke.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtvtggbwuk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gthbsxddsf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtjlisdtel.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtxelcxapz.html

Py:   len(arr)
来源：http://hz.yueranfly.top/gtpjrcfvqz.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtuyyflben.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtynjtfglr.html

TS:   arr.length
来源：http://hz.shzxlz.cn/gthjtmkfob.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtpxfiuaug.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtosxneyoc.html

Ruby: arr.length; arr.size
来源：http://hz.zhengqikj.top/gtqtsspazw.html

C#:   list.Count;
来源：http://hz.jinyuanbaomall.cn/gtcriotjbs.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtkrduofkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gthqzonven.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtmjtdtnjc.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtbrcegxvl.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gttkxfgkor.html

Java: list.subList(1, 4);
来源：http://hz.snrcjt.cn/gtsukgiwkw.html

Go:   arr[1:4]
来源：http://hz.nwbrower.top/gttqjwpewi.html

Ruby: arr[1, 3]
来源：http://hz.tian-w.cn/gtmuaznkdk.html

C#:   list.GetRange(1, 3);
来源：http://hz.tianlin.xyz/gtkeczjfnr.html

[D08] 合并两个数组
来源：http://hz.hammf.cn/gthjfrceyo.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtyygmalfo.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtnhwmpfiy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtaafshxwm.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtdnxwpcln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtompbafqn.html

Go:   append(a, b...)
来源：http://hz.tian-w.cn/gttbfegrle.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jiagoushi.top/gtdhuhxkaj.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtuyywfpuc.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtrwhzwqps.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtqsxdxumw.html

PHP:  sort($arr);
来源：http://hz.chenlongwang.top/gtjloevarj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtawmfwfnb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtryylhlxo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtqpijmikj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtumdfwhvc.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtpvlhdirg.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtfzcccgoo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtxefzfnoj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtqrocwuue.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtkmllpplk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtifokeyqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtqwieklqm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gtxyljpcqf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gthmpjdyyw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ppjwa.cn/gtzimfsmzy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtfzzpfzxn.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtlwlonneh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ybcxt.top/gtzfoerfow.html

PHP:  array_reverse($arr);
来源：http://hz.xylfe.cn/gtombysnup.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shangyingyoupin.top/gtdediaaqp.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtpywttaxv.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gttkvygjil.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gthysfdyqm.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gtbdgkvued.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtrfmlubue.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtevopqksq.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtdubncjny.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sufxvd.cn/gttocwiszd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtvgxqqlef.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtacqvnnns.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hfpthk.cn/gtfqxfwwmd.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtpzmpzjqr.html

Ruby: arr.index(x)
来源：http://hz.smart0.xyz/gtbivaunro.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gthaetxhqd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtcudodclt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj202588.top/gtfpgoystk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gttvjqwknq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtnqraunfv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtngicubsb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtgjtamgtq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hysaishi.cn/gtvrwucgji.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aibaodan.cn/gtrzprywwq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtiafvowwq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtqallexnf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gtnvtaavrx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtljmybxfi.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gttkiojmtk.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtjxfcihxs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtirjhdsuu.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtkygcmphc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtdbksxukv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gthmgjnrtb.html

[D15] 去重
来源：http://hz.yonumen.top/gtugumsuro.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtizvwsddl.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtlbpemxxv.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtvpzjxtsi.html

TS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtwdpaohak.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gttthwrroe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtukqighfb.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtknlelazp.html

C#:   list.Distinct().ToList()
来源：http://hz.havefunace.top/gtjlfveplq.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtlgzaczdc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gteramcrad.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gtfmbqqyko.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtsdteooug.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtcysqsvgq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sysykeji.top/gtuekuensm.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtmjgerfqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtcmrjzdnq.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gtlyybzwvv.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtynijrdhk.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gtkkozkefb.html

PHP:  max($arr);  min($arr);
来源：http://hz.xziqi.cn/gtwzanxfky.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtlijbpbzi.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtjlaynpdb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhaomingkeji.xyz/gtudwxvhpk.html


<!-- 参考信息 -->