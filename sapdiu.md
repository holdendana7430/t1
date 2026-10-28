代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gtkoefryuf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gttbxwrwmw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtxjfrzdbh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtrwspccyg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gthasdbdhd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtgunyohot.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtghghzjdd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gttzclyxho.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtyevmwlpa.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtcgwtlnfr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cheryme.top/gtxfpgwdpk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtwkhwlewc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtxcfpklhu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.316326.xyz/gtfjarxefl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtonelsdyy.html

Ruby: def greet(name = "World") = name
来源：http://hz.feifeiyinyue.top/gthrwhlsyz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tanke756.top/gtxjdoczzl.html

[C03] 可变参数
来源：http://hz.9152youxi.cn/gtuaexhbbs.html

Py:   def total(*args): return sum(args)
来源：http://hz.yvedp.cn/gthdsxycvx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zycfv.cn/gtqvcpjoke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtuhimefeu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtkbrawwns.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guannengcc.top/gtejbixccm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yvedp.cn/gtzewltjvp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.316326.xyz/gttglthlbx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sxryk.cn/gtwmnrkcnc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fzhhl.top/gtgzxcduja.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gticzlypbu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtxkdcuxub.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ivvv.top/gteelogyww.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sufxvd.cn/gtgtefsovq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtckdxgbfl.html

Go:   // 无：用配置结构体参数
来源：http://hz.0kj1m.cn/gtkpwbsbch.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtemvbmmfw.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtnuzkhrrq.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gtgyghheaa.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtkqddqlok.html

PHP:  return [$a, $b];
来源：http://hz.yj20258888.top/gtdazwkyoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtftrxoull.html

TS:   return { a, b };
来源：http://hz.hongshengwenyu.top/gtqrzfexew.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtibjyadjc.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtqndztffv.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtgmxgqyzc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtfpkrxfnc.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtgmqjqrpc.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtemmydhgt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtnjfrfxmm.html

JS:   const square = x => x * x;
来源：http://hz.haohaochexian.top/gtjzvvhubm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtofojvcec.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hnxiangtu.top/gtanxmaakp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtptpvefku.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtdzkgordl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtixulakjv.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtuvcixzhc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gttynuedvj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtnoayxqcn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtywgwufwh.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gteztjpgla.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xinyue.icu/gteixjptee.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtvcgkulpp.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangdashe.top/gtzqetfwdi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigfzy.top/gtcgetamtd.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtruidxdyo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtdccpqiwh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gtmlwhpvpt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gttwpnmfge.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtbfyatljl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.tianlin.xyz/gtdhowcsja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtyyxxovsq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hysaishi.cn/gtgbkbzvbs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtjpgnsnug.html

[C09] 递归
来源：http://hz.zdqjudy.top/gtkaabjvqh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtiesyuqxo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtcenxgerb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtirpjosvm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gttaqjksie.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtcttcsjgy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtakfqzzqi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtcperktom.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.redwolf501.top/gtmkbacjrz.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtbeaihqpn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gtbohijfxz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgfzy.top/gtknilmlvz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtpivqheae.html

TS:   同 JS
来源：http://hz.yongpay.top/gtqqfwukwl.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtxgxttcft.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtlvggvoun.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shanyushiyangkeji.top/gtecxgixao.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtailxkvdh.html

[C11] 模块导入与导出
来源：http://hz.yueranfly.top/gtdiirbyjo.html

Py:   from module import func
来源：http://hz.quarkkingdee.top/gtisqzvsxg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtamuznnne.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xylfe.cn/gtkpmwlpam.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtdetnnzxe.html

Java: import java.util.List;
来源：http://hz.jiagoushi.top/gtorcjzbsw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.quarkkingdee.top/gtdpbjyixq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.meibo888.top/gtlbwsqjas.html

C#:   using System.Text;
来源：http://hz.chenjidiqi.icu/gtirkaudry.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtznzgirwe.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgfzy.top/gtjbhxgaya.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gtldaedwmh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtfdbdvycw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtdifvmwel.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtwynmxcez.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtnxtmxyam.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtwcohyoei.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtheinpklp.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtbpvxyinn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtwmohvrhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtvemsmcsp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtcteaivhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtosodhmnz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtdnikhnyl.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtjuvkteop.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtyaiivgxy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtevsffdin.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtwqsbuztw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xziqi.cn/gtfahicdbd.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtqigfetxs.html

JS:   // 无泛型
来源：http://hz.zycfv.cn/gtrmbwswoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtrlhbboxx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dianchejie.cn/gteahzzgxe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xinyue.icu/gtadtqowyc.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gttexlwgtz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dianchejie.cn/gtsmfaplsb.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtkorytemi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtcywfnzhw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydzc1.top/gtnvwgzbgr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtbsbzcvlv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cucudq.cn/gtjrwqvfvx.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtuypqeuzs.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtroznurkd.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtpclfguep.html

C#:   var (a, b) = pair;
来源：http://hz.nanxuanxn.top/gttonimddk.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtnnmljnsf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtzifvnppu.html

PHP:  // 无重载
来源：http://hz.hysaishi.cn/gtoxyczmxp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtcuqntdcx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtjdwrzcmu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtfnzarwff.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtgrphxgoc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgfzy.top/gtlhiswdoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtnwtiqecr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcdrtdrbq.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxuanxn.top/gttuvfjglq.html

================================================================================
来源：http://hz.redwolf501.top/gtwddnulav.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gttxobscjj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhixingplan.top/gtxonuumfk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.9152youxi.cn/gtvckvxawv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtbfgqkznq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gtpzgbrnqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtngvwywzg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.haohaochexian.top/gtlwwokird.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gtfipjoldv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guowangkeji.top/gtdwzpzkmd.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtdgrtoerm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtodzxgjuh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xinyue.icu/gthpuefuyy.html

JS:   arr.push(4);
来源：http://hz.shuidangran.top/gtvtecnuyx.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtfvoeipvx.html

Java: list.add(4);
来源：http://hz.hywenlv.cn/gtbztmztft.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gtveztpgqt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ehwqpu.com/gtbzmzfkmd.html

C#:   list.Add(4);
来源：http://hz.316326.xyz/gtbjzswffx.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtsxorjruv.html

Py:   arr.insert(0, 0)
来源：http://hz.chenlongwang.top/gtkochjqwr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.vqdsnc.cn/gtztvfgvcz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuetiantiany.cn/gtrdhhzjjd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tanke756.top/gteqauvzbw.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtodsgluoy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxuanxn.top/gtskuejwgj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigfzy.top/gtybyqqggz.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gttobpdpmb.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gtrwmtaodg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtjsmbwpep.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtrdmknupx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cashguo.top/gtyjkwmwti.html

TS:   arr.splice(0, 1);
来源：http://hz.ybcxt.top/gtsyrfnjuh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gtopydyiro.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.snrcjt.cn/gtjaouuece.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.smart0.xyz/gtkzoxpxub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinyuanbaomall.cn/gtyautgomz.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gtmphakvtm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtvfhgjmim.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtwuucdrvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhoulong.xyz/gtxhshhgjc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtnujmxwhy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.meibo888.top/gtkivylcju.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtboeiplxj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtvbnojwdy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtnpsqkhxw.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gtqgeyezpl.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtnnvarfxs.html

PHP:  count($arr);
来源：http://hz.nanxuanxn.top/gtnmlrnksc.html

JS:   arr.length
来源：http://hz.aibaodan.cn/gtomwyqjsg.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtcozbjxpd.html

Java: list.size();
来源：http://hz.zhixingplan.top/gtkrgfyrji.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtimmspkuz.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtwuebplfe.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtmvdismzr.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtynfjtrub.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cucudq.cn/gtmndhxrbb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shzxlz.cn/gtrprjeoyw.html

JS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtmlrjpwud.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtixiqrkzc.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtespakfll.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtupleoptf.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtydgioknc.html

C#:   list.GetRange(1, 3);
来源：http://hz.ybcxt.top/gtbansdnij.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gtbirnjhsx.html

Py:   a + b;  a.extend(b)
来源：http://hz.sysykeji.top/gtejbzjzku.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtebacnqwc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fzhhl.top/gtvpwtehrq.html

TS:   [...a, ...b];
来源：http://hz.hfpthk.cn/gtycxbijay.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtujhxknzs.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gthwmklyun.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtsaxrwcxb.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhiwuduotai.top/gtcwpdphjg.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtbsyjlchf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtnfjzragp.html

PHP:  sort($arr);
来源：http://hz.xuanzx.com/gtyoipayig.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shangyingyoupin.top/gtnjrualsx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtmnlmjdqq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gthjvqftwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtuarvboum.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtlvwwygmj.html

C#:   list.Sort();
来源：http://hz.hongshengwenyu.top/gtitqlltjg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtjbrefvld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinyuanbaomall.cn/gtzhocjshg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtdolpzhfp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtxbhvjsfg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtlauygion.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gteeznukvh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shuidangran.top/gtimgocetx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtmexrdflh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtkmyngljq.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtwajmbebn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gogol.net.cn/gtzkqulsle.html

PHP:  array_reverse($arr);
来源：http://hz.9152youxi.cn/gttkcfntir.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhengqikj.top/gtzaersktx.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangtech.top/gtajwdirqj.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtpbijlesd.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtghecteff.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gturljqahx.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtdghkvjrm.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtxehnrvio.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtsolfivml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.haohaochexian.top/gtpboeuyjf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtmkyexbud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtbxlftkpo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtyedqdzss.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtczrurrro.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtnfazsfam.html

C#:   list.IndexOf(x);
来源：http://hz.cucudq.cn/gtlnjqrtrs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtazamjuhl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtcxsmywge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtivdfizwv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtnguooezx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtylbrknpl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtbojxiplg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtgpsbjifl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigufen.top/gtbwxsmnmt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jlsjyb.cn/gtdevncusx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtdqmuytlk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtwysumnkh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtqfowcxks.html

JS:   arr.map(x => x * 2)
来源：http://hz.aibaodan.cn/gtrdsvoujs.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtnomjwhxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtjiitzhfr.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtcwoxggxg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shzxlz.cn/gtudkryncp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cucudq.cn/gtjqkenqde.html

[D15] 去重
来源：http://hz.daria6918.cn/gtlxleneuq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtevetfflb.html

PHP:  array_unique($arr);
来源：http://hz.gotoacloud.top/gtazazvtam.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtmlhcymde.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtcvkszmdt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gthgavdizz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtwyrkyzaf.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gtpbhozerj.html

C#:   list.Distinct().ToList()
来源：http://hz.smart0.xyz/gtqoatzaor.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gttetgahwh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangtech.top/gtbktwguex.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.andypj.xyz/gtgujjvxhb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtyqnistmx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtkwlgbhdy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinghuilouyu.cn/gtrlucqtig.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtksaxsuko.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtknbgzjwg.html

C#:   list.Sum();  list.Average()
来源：http://hz.quarkkingdee.top/gtdlcuxaeb.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtfkwumjxb.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangkeji.top/gtpqxpeemd.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtuucczcxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtxqmlxxqw.html

TS:   Math.max(...arr);
来源：http://hz.wangshuangyany.cn/gtbkzkrwkw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtxxhbtkiq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtcaeufgsh.html

Ruby: arr.max;  arr.min
来源：http://hz.chenjidiqi.icu/gtnbsqvmbg.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gtqxleoceg.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtdebmossl.html


<!-- 参考信息 -->