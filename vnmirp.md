代发 wailian999

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gthahswkbt.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtnskwlgzc.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtbnzrczyh.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gtbvoptosc.html

Java: if (data == null) return;
来源：http://hz.yuanzhike.top/gtvrklqnwp.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtnhwvoopg.html

Ruby: return if data.nil?
来源：http://hz.tianlin.xyz/gtvhngwegf.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtowpaesmi.html

================================================================================
来源：http://hz.9152youxi.cn/gtwimdwpuu.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtvfxfxwlg.html

================================================================================
来源：http://hz.316326.xyz/gtcakyfmwh.html

[C01] 定义函数
来源：http://hz.jinghuilouyu.cn/gtgwggelah.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtmolwiksg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtdrxrmogq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtqvlaxydl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtglffltbe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gthfvlswlt.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtrxxshlpw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.meibo888.top/gtbpwluryj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtdaxscofz.html

[C02] 默认参数
来源：http://hz.birdmap.top/gtktztxden.html

Py:   def greet(name="World"): return name
来源：http://hz.vqdsnc.cn/gtzpylrref.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhaomingkeji.xyz/gtfrtygktg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jiagoushi.top/gtmlikqcdw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtntitfatz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jiagoushi.top/gtnktwbuss.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtzmqisreg.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgufenzy.top/gtcedmcjom.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtvfyctkdx.html

[C03] 可变参数
来源：http://hz.sweek.top/gtqziplzhd.html

Py:   def total(*args): return sum(args)
来源：http://hz.cdnleiting.top/gtenjbmgnr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258.top/gtnowjzlui.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtuomycukz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtatresatb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gtskviugcp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtxcuqcvtn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yangfankeji.com/gtzrfikgtt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtcmvqebkv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cashguo.top/gtyourhstn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aizwys.cn/gtkdogoecg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jlsjyb.cn/gtashunojg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtdbtlnzfs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtmzmepkyr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtmrpseqxy.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtexgumwpo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtugcjywky.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtvbavxztq.html

[C05] 返回多个值
来源：http://hz.zhixingplan.top/gtjajodbag.html

Py:   return a, b
来源：http://hz.316326.xyz/gthqvdyocf.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtddmesdsz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.quarkkingdee.top/gtfugcceyh.html

TS:   return { a, b };
来源：http://hz.jinqigufen.top/gttgfbmgkh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cdnleiting.top/gtsetbbtfn.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtarqsqbge.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gtqcwhnxys.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xziqi.cn/gtihdsymch.html

[C06] 匿名函数 / lambda
来源：http://hz.sufxvd.cn/gtfcxmvpoo.html

Py:   square = lambda x: x * x
来源：http://hz.hysaishi.cn/gteqnfmlqq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtsubgtjtg.html

JS:   const square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtpvstyrhh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtiaklyteh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydjk.org.cn/gtpklkzezz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtqnpwcozx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtonmfguya.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtbaprgabu.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtfraxmzqq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sufxvd.cn/gtyaxckpqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhaomingkeji.xyz/gtqkjtksfu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yueranfly.top/gtwmitcytq.html

TS:   arr.map(String)
来源：http://hz.svipenyu.cn/gtygjykrfz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinqigfzy.top/gtgysallar.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.meibo888.top/gtsnpsndxz.html

Ruby: arr.map(&:upcase)
来源：http://hz.daria6918.cn/gtdbomrtdh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gotoacloud.top/gtnaposqgj.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtdnjkxzfz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtaltjipuk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jianghu66.top/gtsibjcjju.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtlxjfjinb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtygrnycwa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cucudq.cn/gtmlplbbun.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtxqwxpiyv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guowangkeji.top/gtldnxnvik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtssocmojb.html

[C09] 递归
来源：http://hz.jyoumei.cn/gtqlvfsaqx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtycsrcsem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigfzy.top/gtiefxgcrn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtsivutzuu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtuzlfddiz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuanzx.com/gtspuyjgnn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hfpthk.cn/gtwyngxacd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtouyoaqlj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtolprokzf.html

[C10] 变量作用域
来源：http://hz.yangfankeji.com/gtzditshbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gotoacloud.top/gtpjdtnazo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtqtnzqqbp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtvzmnojxg.html

TS:   同 JS
来源：http://hz.bjfxy.top/gtulhsionu.html

Java: 方法内为块级作用域
来源：http://hz.meibo888.top/gtrojlixhj.html

Go:   花括号块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtabiqigdy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhengqikj.top/gtguwbftkf.html

C#:   块级作用域
来源：http://hz.zhoulong.xyz/gtoknkbjlg.html

[C11] 模块导入与导出
来源：http://hz.xingfuxueyuan.xyz/gtgtdlwkvn.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtrvawaqkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zdqjudy.top/gtxalhtwtr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtdbnfnren.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuxming.cn/gtlrwycsrf.html

Java: import java.util.List;
来源：http://hz.guannengcc.top/gtijbijdjk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtronzpbir.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pengpengdd.cyou/gtohaqxtkc.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gtjrpzwpal.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtciazrizi.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgfzy.top/gtutznujqs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gtqjpstsmo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gtlitsaqcr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.meibo888.top/gtxhrxxgda.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pycfn.com/gteetxucmx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtehlbgpsc.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtvigagplb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtufwzttwp.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gttfjgaqrf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtzejuvwrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gtikjhqqbn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.snrcjt.cn/gtgececbmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtfnopyksp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtyrpflbsa.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtlbmebhbd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aizwys.cn/gtpfqurfsf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gtudwltseo.html

[C14] 泛型函数
来源：http://hz.chenjidiqi.icu/gtsnilsbge.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtuqrybiol.html

PHP:  // 无泛型
来源：http://hz.iojbl.cn/gtjccyuwcz.html

JS:   // 无泛型
来源：http://hz.daxiang520.top/gtzruvtckm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhaomingkeji.xyz/gtdgrfufyg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtzaabfzlz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtcuhssjox.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtrljrunaq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtncwchaab.html

[C15] 解构 / 展开参数
来源：http://hz.gotoacloud.top/gtgnkewazr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtojdogurb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtrsbpglzl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtidjwzybt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtssbmxizu.html

Java: // 无解构
来源：http://hz.fzhhl.top/gthcddyvnk.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtnlayfiiw.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtfkvfmvvo.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtbjwftvie.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gticnsxtwl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuxming.cn/gtxlhbagdm.html

PHP:  // 无重载
来源：http://hz.yueranfly.top/gtqnzhcyxc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shuidangran.top/gtuzcagksp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtgwtwiint.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtodddpskg.html

Go:   // 无重载：用不同函数名
来源：http://hz.havefunace.top/gtqktjorra.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guannengcc.top/gtmyeiefmj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxinkj.top/gthydjxcjo.html

================================================================================
来源：http://hz.aibaodan.cn/gtnpnaqgof.html

D. 数组 / 列表 / 集合
来源：http://hz.bjfxy.top/gtgzclpoxl.html

================================================================================
来源：http://hz.cashguo.top/gtunwpuxht.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gthelwhrkd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yangfankeji.com/gtrxvbubzu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenzaomai.com/gtvdptxlfh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtzyxxoqqt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtdkbjjfwv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtdisaodhx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.bjfxy.top/gtrqscmxwn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigfzy.top/gtrwoacmer.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sufxvd.cn/gtyeuvmipj.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtiyeukwtu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtulrivlpl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258.top/gthhfsyqce.html

JS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtojdzufxm.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtjyuqydvy.html

Java: list.add(4);
来源：http://hz.fengsongda.top/gtjmmgpihb.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtrpwziury.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gttktwuitx.html

C#:   list.Add(4);
来源：http://hz.quarkkingdee.top/gtahfptaog.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gtcnungizv.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtevgyactq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.svipenyu.cn/gtdwlrtgak.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gtcylfwref.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtjgbunvtt.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gteuukhzjf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ppjwa.cn/gtcezxxdzz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtlmyokbgh.html

C#:   list.Insert(0, 0);
来源：http://hz.pengpengdd.cyou/gthxcoewfk.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gtfofjygxf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgfzy.top/gtxddlqkvw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtajjbfmcy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinghuilouyu.cn/gtgyvpiayz.html

TS:   arr.splice(0, 1);
来源：http://hz.ivvv.top/gtvaajolgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtnipdgfrq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gttcqhrhjj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.snrcjt.cn/gtowyzmdqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtczxeeyvt.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtabyjfogv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtomjbhygi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gtdwoqhtzj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daria6918.cn/gthuquxxqs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.316326.xyz/gtgxssxsrd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtpfxefepy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ybcxt.top/gtnjnffkan.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtvhqkwcso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sysykeji.top/gtfxlvejdt.html

[D06] 数组长度
来源：http://hz.snrcjt.cn/gtxlrrzqxq.html

Py:   len(arr)
来源：http://hz.iojbl.cn/gtmfkssgtp.html

PHP:  count($arr);
来源：http://hz.cashguo.top/gtyhrcluah.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtodnweqap.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtjaaxcngs.html

Java: list.size();
来源：http://hz.jinqigfzy.top/gtrzruqstl.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gthydqfvoj.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gtdlkwblwz.html

C#:   list.Count;
来源：http://hz.xuanzx.com/gtumzrpbjd.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gttvrgdsvj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gthwfqnbpb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigfzy.top/gttofdxxrg.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gthvasmkee.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtmwqpvasb.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtjreusizs.html

Go:   arr[1:4]
来源：http://hz.cqqwz.cn/gtozhyqlby.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtnriotqoh.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gthdcvglug.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtxmxlousp.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258.top/gtswfmzpez.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gttqvvkmbx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtcxrheeek.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtrunekjuy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtqafmgmyi.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangtech.top/gtlkbcfhbk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtncwceumg.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtrbjekwnq.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtolutjjth.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtdsbvnxso.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtxndlmvay.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zycfv.cn/gtesmsnnvo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtxcnrmbmj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gtxupjpvjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtppuauzei.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtzvecqzwg.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtiwusngic.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtlhrybyqg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gogol.net.cn/gtwcksrygj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtpaeksbyv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtrbtfizta.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtcnrcbndv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.feifeiyinyue.top/gtzmzdonru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtwgprkbuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zdqjudy.top/gttchcojyp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtmxqajlie.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtsbofkjul.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenzaomai.com/gthhcfvuig.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gtpcumgokp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtkfcdbpox.html

TS:   [...arr].reverse();
来源：http://hz.xziqi.cn/gtdljjgocl.html

Java: Collections.reverse(list);
来源：http://hz.hnqzz.top/gtlixwkvvo.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxinkj.top/gtxfbilizs.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gtbtcwqhnu.html

C#:   list.Reverse();
来源：http://hz.jinqigfzy.top/gtyqnxyffz.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtqeesxkxj.html

Py:   arr.index(x);  x in arr
来源：http://hz.zycfv.cn/gtgtxhaeby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gtnmqjwrdd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtjafvgiai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtwnkrcptf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guannengcc.top/gtvhliieoz.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtqpiqiwhu.html

Ruby: arr.index(x)
来源：http://hz.haohaochexian.top/gtdqlhnyfq.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtzuzowtkc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtpevtkmez.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pycfn.com/gttgaaozcj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtvakxbyqa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gthxwetwug.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtidluluca.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtmsjcxtde.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtnrjwpbxj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gtqhqirwee.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtpaugolou.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhaomingkeji.xyz/gttbndoibf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtmnlrstve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.feifeiyinyue.top/gtrnpkivew.html

JS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtlrwwyccy.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtsuojnyom.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.havefunace.top/gtuprfppkw.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtiozxwlju.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nanxinkj.top/gtfywkorkx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtanjtiuwp.html

[D15] 去重
来源：http://hz.cqqwz.cn/gtebjzjatd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtzlrwlqqy.html

PHP:  array_unique($arr);
来源：http://hz.zhaomingkeji.xyz/gtsfuxxdkn.html

JS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtzdsvjkkk.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtdmyrndzi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yvedp.cn/gtpwoqqjpe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtlrggsdyf.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtlfserrrl.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangtech.top/gttwljtkrv.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gtmnqlqjmj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtwkuudpzr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtnilesugl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtcdogjnkq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtqcboqiyg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuanzhike.top/gtbnjcxyzo.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtezglhanf.html


<!-- 参考信息 -->