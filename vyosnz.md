代发 wailian999

Py:   if not data: return
来源：http://hz.316326.xyz/gtpdgtsmjx.html

PHP:  if (!$data) { return; }
来源：http://hz.gzhubu.top/gtjufpdqor.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtmvsfajvr.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gthywmynjc.html

Java: if (data == null) return;
来源：http://hz.ybcxt.top/gtgdunjxin.html

Go:   if data == nil { return }
来源：http://hz.yuanzhike.top/gtuproutbf.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gtgvhailna.html

C#:   if (data == null) return;
来源：http://hz.chenlongwang.top/gtwqwllkfy.html

================================================================================
来源：http://hz.xylfe.cn/gttjgxmxbj.html

C. 函数与作用域
来源：http://hz.hysaishi.cn/gteycgjgkv.html

================================================================================
来源：http://hz.haohaochexian.top/gtpkykeqyq.html

[C01] 定义函数
来源：http://hz.havefunace.top/gtmvtzbhkw.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtkuetgjco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gteygycvfq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtfuhvqfsh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtcbygxypu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtvxgkqqrh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.9152youxi.cn/gtusbtwkup.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sufxvd.cn/gtwzspefjv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtcsogiaos.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtwwizziov.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtkhvcpfkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gttzkpqgag.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.meibo888.top/gtxrazvcsb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gthwjqqxpo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtczcjhgdr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gtvjpugchi.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtlwhkcudz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fzhhl.top/gtzswgzpdf.html

[C03] 可变参数
来源：http://hz.xylfe.cn/gtptiwqonl.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtqvxglibk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtpdxkockb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtziwehynd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtvklopmxb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtydmwwkjs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj202588.top/gtxrkvwtds.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtxmgmoyaa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shangyingyoupin.top/gtpfnvsswi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.bjfxy.top/gtdnbonomh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.c1oappe.top/gthogfwuzw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtkntjxgxl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtohpvrcrs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gtsvpfqxjx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gthvjgptvt.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangshuangyany.cn/gtodsijore.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtvqkswxdm.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtiuwbbmua.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gtqtqnldij.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gtcgbryrmv.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtdyzocuuf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yueranfly.top/gtkmcvgpcc.html

TS:   return { a, b };
来源：http://hz.pengpengdd.cyou/gtbufpnqfi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jiagoushi.top/gtnmeoxzcy.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtgtrdcprs.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gtcjkqxiez.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.vqdsnc.cn/gtgyblfdjw.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtcttqbalk.html

Py:   square = lambda x: x * x
来源：http://hz.nanxinkj.top/gthhzpcxha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sweek.top/gtdtwdzlqg.html

JS:   const square = x => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtnozdetvr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daxiang520.top/gtibvgtqpb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.feifeiyinyue.top/gtatkiikcq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fzhhl.top/gtphxlglyx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtmgnfsfxd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.havefunace.top/gtqmqhzdtp.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtvarytnmv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guannengcc.top/gtnkeyxqfp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gtqejbrwui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtipcfuvnk.html

TS:   arr.map(String)
来源：http://hz.bjfxy.top/gtrkpqooit.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtbnwomnua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtfaibafql.html

Ruby: arr.map(&:upcase)
来源：http://hz.xylfe.cn/gtzivvrtau.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.vqdsnc.cn/gtjotutkqi.html

[C08] 闭包
来源：http://hz.yj202588.top/gtcbwpjave.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtlwlrhucu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fengsongda.top/gtrbmuorah.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtswjccotw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtucrrjtgs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhixingplan.top/gthxriixjf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtmlgirlwm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ivvv.top/gtusgrlfqb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtqwcjuexb.html

[C09] 递归
来源：http://hz.wangshuangyany.cn/gtvobkserd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtvsvegntr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtzbxrpsbm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtlcettzaw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtksoikdwf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangdashe.top/gtgnrmsvgz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenzaomai.com/gtevincmhd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtrhiiueks.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuetiantiany.cn/gtvgidmikb.html

[C10] 变量作用域
来源：http://hz.ybcxt.top/gtoxcrbuva.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cheryme.top/gtflsbobjq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gteqlxekjw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ywan-chungtsiang.top/gtpotqeyxf.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtxjvijthu.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gttlmjlxzp.html

Go:   花括号块级作用域
来源：http://hz.guowangkeji.top/gtbwehegse.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yvedp.cn/gtzczkcesi.html

C#:   块级作用域
来源：http://hz.nanxinkj.top/gtkzjmssdx.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtumibpjhi.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtprakfyhm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gteigjvkkb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtkirjnsed.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gtmjfoxctm.html

Java: import java.util.List;
来源：http://hz.cucudq.cn/gtokmvpzmj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtgicdlixb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtoqgxfuak.html

C#:   using System.Text;
来源：http://hz.yvedp.cn/gtmyvpolzp.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtdzxvrmgp.html

Py:   (lambda: print("run"))()
来源：http://hz.cashguo.top/gtbjmbailq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gthtzrpjel.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtlqtemwkj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gttcatvmvq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtaoafpmcv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gtwmcasaaf.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtnhfexkqg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gtazvbncht.html

[C13] 类型声明 / 类型注解
来源：http://hz.gogol.net.cn/gtgqqurzrb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtfqtykngm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtykhnmrgl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtzhyaygaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258.top/gtkpvpjexu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jqgfzy.top/gtswtiovaj.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gterkrdcwa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtxhmafqgc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtfanneium.html

[C14] 泛型函数
来源：http://hz.dashuyun.cn/gtsqpuqhgd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aizwys.cn/gtysnlapzz.html

PHP:  // 无泛型
来源：http://hz.ehwqpu.com/gtungrvkcy.html

JS:   // 无泛型
来源：http://hz.andypj.xyz/gtclwztwbp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtrvdkofyu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtesizhhfo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pengpengdd.cyou/gtxjlxavze.html

Ruby: # 无泛型
来源：http://hz.jyoumei.cn/gtjihdyzml.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nwbrower.top/gttwqzuezk.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtcpuynbqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtyzlntnxa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gtnyfbpdah.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtvbxnvtmp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtpxycimut.html

Java: // 无解构
来源：http://hz.zycfv.cn/gtmyzbixcu.html

Go:   // 无解构
来源：http://hz.nanxuanxn.top/gtnhnoivop.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtaykfwobt.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtxrqfzgsj.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtsmzxwlmt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.smart0.xyz/gtgunqcqrl.html

PHP:  // 无重载
来源：http://hz.hysaishi.cn/gtrcjgnnqg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dianchejie.cn/gtthdtdbyw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenjidiqi.icu/gtgungqiwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gttifgnzej.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtlfwqsjqr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinyuanbaomall.cn/gtlkzmvifb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhoulong.xyz/gtymzdyidp.html

================================================================================
来源：http://hz.sweek.top/gtghxlwmmm.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gttbohtqqi.html

================================================================================
来源：http://hz.yj20258888.top/gtczpkxfzf.html

[D01] 创建数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtfldaigbp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtrcudxqpr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtslynrvfk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.birdmap.top/gtgsssnssu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtpwezelbw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.dianchejie.cn/gtkriawdky.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhaomingkeji.xyz/gtofsdwzrm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gtjljapdgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hammf.cn/gtvbrdusbv.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtzisxzwaw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtpidvjlhr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cqqwz.cn/gtkjuzmpae.html

JS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtcmzgxpxe.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gtpfpbogsb.html

Java: list.add(4);
来源：http://hz.yueranfly.top/gtmuqiqnhr.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtnkeujjal.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gogol.net.cn/gtjczcdisn.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtqeoijnbr.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtmkhuhbug.html

Py:   arr.insert(0, 0)
来源：http://hz.meibo888.top/gtqfwzwqes.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtmovgjomq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gtinkmgpis.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jiagoushi.top/gtjtlnanmt.html

Java: list.add(0, 0);
来源：http://hz.yuxming.cn/gtjvhpulqx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtojmhspey.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangdashe.top/gtphxppwps.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtrpjsjiuu.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtjsljdbya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtjrpipixf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.snrcjt.cn/gtjjaqdttc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtquptkmcp.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gteifwbznw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.c1oappe.top/gtcohvnupz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gthbiaeynl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtlvnuzfsg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuxming.cn/gtlfuxvydq.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtrrhblcma.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtfapwcjan.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xziqi.cn/gteeznurci.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.svipenyu.cn/gtndtwlugw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtsgxxknvu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtbifdydxg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtldjafaxp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtsbyamucp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtbcxifxri.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtquuxpaso.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtorzewwpg.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtdqbbxjco.html

JS:   arr.length
来源：http://hz.aizwys.cn/gttgelphfn.html

TS:   arr.length
来源：http://hz.guowangkeji.top/gtabrghcwq.html

Java: list.size();
来源：http://hz.shanyushiyangkeji.top/gtntsuyali.html

Go:   len(arr)
来源：http://hz.316326.xyz/gttxnubwey.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtgbzmkuvn.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtwsnhkeol.html

[D07] 切片 / 取子数组
来源：http://hz.c1oappe.top/gtgggclgdw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtbpygzqpl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gotoacloud.top/gtnhajqupl.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtajksfgdi.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtbhxkflnu.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtsqwpdjtt.html

Go:   arr[1:4]
来源：http://hz.xylfe.cn/gtrntyxojt.html

Ruby: arr[1, 3]
来源：http://hz.yueranfly.top/gtdlhcllvm.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gtxtxkfenp.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtznpipbit.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtsamdvmtn.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gtxrifkhar.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.bjfxy.top/gtxdiqjtkq.html

TS:   [...a, ...b];
来源：http://hz.xylfe.cn/gtkgoclemv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtngibycmu.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gthgytavwv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dashuyun.cn/gthbcvwpmz.html

C#:   a.Concat(b).ToList()
来源：http://hz.sufxvd.cn/gtozgrkvyy.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtfvwmnuel.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtfjjgwxlw.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtujxufogk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtidoczesp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtejzhbjnx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtnkrgemjk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.9152youxi.cn/gteffxadql.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtxwbslkbj.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtgslvnyht.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtduagqlgq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtrnaqmafc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtowzvtcjg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtmhmpbgfy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtjnwhpdil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gtlrfplbyl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gtszspmflx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtebwuvuhb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.52xcode.cn/gtwsabmckx.html

[D11] 反转数组
来源：http://hz.jiagoushi.top/gtgqmqtkfm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtkjtgttuy.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtjvkukfex.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtvvcexbnv.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtiyrjtcrb.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtoepstmsy.html

Go:   slices.Reverse(arr)
来源：http://hz.xinyue.icu/gtgwinkhjr.html

Ruby: arr.reverse
来源：http://hz.tanke756.top/gtzttiftux.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtjjgkzgyp.html

[D12] 查找元素下标
来源：http://hz.snrcjt.cn/gtomacrrxk.html

Py:   arr.index(x);  x in arr
来源：http://hz.xylfe.cn/gtzyqqvohr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtvgskaxsa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtwvlpqulp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtiijqxkdf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtlnxhtdbd.html

Go:   slices.Index(arr, x)
来源：http://hz.xylfe.cn/gtxdjnewcl.html

Ruby: arr.index(x)
来源：http://hz.zhaomingkeji.xyz/gttzwigdam.html

C#:   list.IndexOf(x);
来源：http://hz.xziqi.cn/gtpkjjxzmu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtgjghjkkg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtazyrlfof.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shangyingyoupin.top/gttkcrwsww.html

JS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtznuejebt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtwmlolhfm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.52xcode.cn/gtxqtcdpua.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj202588.top/gtngsljsdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtrqfaqnkz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtgztgxuux.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtiyhgajdf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.feifeiyinyue.top/gtjprmqzhx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhoulong.xyz/gtkijvrhgw.html

JS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtriszrmbc.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtyusguasp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dashuyun.cn/gtfrfuagkt.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtcmizvbvf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sweek.top/gtbkrayjlo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtkigxxvlp.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtemkfkbke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtckshnpqe.html

PHP:  array_unique($arr);
来源：http://hz.smart0.xyz/gtogtnrcto.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtldxquoqm.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtnzynpdfz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cucudq.cn/gtzvneuhtx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtusouheyy.html

Ruby: arr.uniq
来源：http://hz.ydjk.org.cn/gtqotogrqv.html

C#:   list.Distinct().ToList()
来源：http://hz.dashuyun.cn/gtiucdjrtc.html

[D16] 求和与平均值
来源：http://hz.dianchejie.cn/gtjxmhnfre.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.52xcode.cn/gtcxvqvgzp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtvkqkhoza.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtezikryps.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtnosimrza.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxuanxn.top/gtcoxzlvjs.html

Go:   // 手写循环累加
来源：http://hz.cheryme.top/gtpebrxpwy.html


<!-- 参考信息 -->