代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.ivvv.top/gtkfsnxont.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gthxqgueuv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtvzaxaycj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenlongwang.top/gtyckskusr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.52xcode.cn/gtviywjhvk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnqzz.top/gtzqlmhspc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.smart0.xyz/gtnbwaouhq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xziqi.cn/gtzhrqxxwo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtyiknynfa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtraqqhwlw.html

[B15] 布尔运算与取反
来源：http://hz.ppjwa.cn/gtjllndxse.html

Py:   a and b or not c
来源：http://hz.snrcjt.cn/gtzvrbjfmy.html

PHP:  $a && $b || !$c
来源：http://hz.nanxuanxn.top/gthivslgca.html

JS:   a && b || !c
来源：http://hz.jinqigufen.top/gtyytpccvw.html

TS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtwbsajfrh.html

Java: a && b || !c
来源：http://hz.xylfe.cn/gtmvsflfng.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gtbtogkfst.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtfxpgmgvr.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gthezgjxcw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtgqhbuqga.html

Py:   if not data: return
来源：http://hz.sysykeji.top/gtzrywrlni.html

PHP:  if (!$data) { return; }
来源：http://hz.ybcxt.top/gtrebvgknn.html

JS:   if (!data) return;
来源：http://hz.xuanzx.com/gtqefzvzxv.html

TS:   if (!data) return;
来源：http://hz.ybcxt.top/gtcjtskfgy.html

Java: if (data == null) return;
来源：http://hz.birdmap.top/gthoiksuaa.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtghtspoko.html

Ruby: return if data.nil?
来源：http://hz.nanxuanxn.top/gtvynewlnz.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtobjesnuu.html

================================================================================
来源：http://hz.sysykeji.top/gtopetdgll.html

C. 函数与作用域
来源：http://hz.gaohongyu789.top/gtnygnonsh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtepkawove.html

[C01] 定义函数
来源：http://hz.yj202588.top/gtvehpbmnl.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtcnxqavpc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtyzhnbxfp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtqdeobrns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtaoypxiby.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtptnetqia.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sysykeji.top/gtfwfgzyoe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.52xcode.cn/gtmsqgoxzq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtqsgsgxsc.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtezwibipc.html

Py:   def greet(name="World"): return name
来源：http://hz.hongshengwenyu.top/gtuopgenrt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yvedp.cn/gtpdmkvozj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtaznqrsjx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gtondiavoe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pengpengdd.cyou/gtbnhidqri.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxuanxn.top/gtnqphfcok.html

Ruby: def greet(name = "World") = name
来源：http://hz.cashguo.top/gtotvputlp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtyumktrzb.html

[C03] 可变参数
来源：http://hz.jinghuilouyu.cn/gtkjpfizff.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangdashe.top/gtuosenmgt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.mhx1999.top/gtkmcmbizp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtgldtofcy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gturouylin.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yongpay.top/gtuaiaqwxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtxdujwruw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.snrcjt.cn/gtukerojwy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtzgdvguwv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtjgqxerxj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jlsjyb.cn/gtmvbvkrgb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.svipenyu.cn/gthfnydgch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtecdbodzn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.andypj.xyz/gtvftgoqbc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtdawoapox.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtemigzknw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtllujnoqe.html

C#:   f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtnykzhzie.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtjwnfilly.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtnoawudlz.html

PHP:  return [$a, $b];
来源：http://hz.vqdsnc.cn/gtnykibvbr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydjk.org.cn/gtacstvncq.html

TS:   return { a, b };
来源：http://hz.yuxming.cn/gtgswfgnjg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ppjwa.cn/gtfyhhnssd.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtlcceotfn.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gtmjkpqckf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cdnleiting.top/gtrsjbpixq.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtbidlrqim.html

Py:   square = lambda x: x * x
来源：http://hz.0kj1m.cn/gtbbytuvjx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.316326.xyz/gtpsjcvbym.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gtiuaydzdb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtwywhznxw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhengqikj.top/gtemtwtgxv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtnzvblenu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgfzy.top/gthobeqeha.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhiwuduotai.top/gtzpkpxrwh.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtorawhaay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhengqikj.top/gtlrgjtcmm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hammf.cn/gtwmgcltgu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtvwbiajvc.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtnfydqlle.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cheryme.top/gtgdqkunsz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangshuangyany.cn/gtpyjcxgsp.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gtelsjeknf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gtqivacisp.html

[C08] 闭包
来源：http://hz.shuidangran.top/gtwymtgkob.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtjsrvodse.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenjidiqi.icu/gtcsazyhqb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtqfbktvvf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gttfdawhbw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gtvbyogydc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtejwkgxvn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtyvpcizgh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtcszvyvqy.html

[C09] 递归
来源：http://hz.andypj.xyz/gturzzuirx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.birdmap.top/gtpvsnxqnw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtkdqaqgjh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtyvpaksvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtkokdsdxp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtzhsubkfv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gogol.net.cn/gtyvlqwbcl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtnugaivfn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtvuahxfwz.html

[C10] 变量作用域
来源：http://hz.quarkkingdee.top/gttikgyqaa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sweek.top/gtyslnsrms.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtdrjoeqhk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtdlmlaway.html

TS:   同 JS
来源：http://hz.fzhhl.top/gtfjgygszu.html

Java: 方法内为块级作用域
来源：http://hz.xziqi.cn/gtypgbiyxp.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtalnapajh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtnuzhznmi.html

C#:   块级作用域
来源：http://hz.birdmap.top/gtpxvbkcya.html

[C11] 模块导入与导出
来源：http://hz.hfpthk.cn/gtymyfumzi.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtcykzvezo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangshuangyany.cn/gtgbawzxvr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cdnleiting.top/gtzxasyibr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.quarkkingdee.top/gtusnmontj.html

Java: import java.util.List;
来源：http://hz.52xcode.cn/gtwnrkiqhs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gzhubu.top/gtlelvlkbz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hysaishi.cn/gteijckkrd.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtsuxlnocw.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gthmzbfsht.html

Py:   (lambda: print("run"))()
来源：http://hz.0kj1m.cn/gtvfyrjrph.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtqnlqtylz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtnjpjwtpj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtfssgatwk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtzhhrflik.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtrqrnsueh.html

Ruby: -> { puts "run" }.call
来源：http://hz.guowangkeji.top/gtblkcisui.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtvxhiicir.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtzvwekpex.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gtfgsibqdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtnplnmrkx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cdnleiting.top/gthlhdwyfj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.c1oappe.top/gtxauktwht.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtngiwvymn.html

Go:   func add(a, b int) int
来源：http://hz.ehwqpu.com/gtkdievfto.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtrydpokby.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tian-w.cn/gtidtosqtt.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtjpskiehu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtgnvfvoqm.html

PHP:  // 无泛型
来源：http://hz.nanxuanxn.top/gtseegljdo.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtithemywo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuxming.cn/gtxtwjrlvf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gthszmweda.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtjxtltkkq.html

Ruby: # 无泛型
来源：http://hz.kuanghao11.cn/gtahnnxndb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sweek.top/gtscuqmtwz.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gthhkmzpbh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinghuilouyu.cn/gtozogxeeb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenlongwang.top/gtxsdtddzs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtcntltxmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtsappfysx.html

Java: // 无解构
来源：http://hz.jiagoushi.top/gtaijdrwbh.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtbbzprrkb.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtavfqxiwo.html

C#:   var (a, b) = pair;
来源：http://hz.ydjk.org.cn/gtpuxzmqwf.html

[C16] 函数 / 方法重载
来源：http://hz.jiagoushi.top/gtbvrcbhya.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtsaffealp.html

PHP:  // 无重载
来源：http://hz.hfpthk.cn/gtlgssfbqu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gtbyjtdtit.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtpjxfeosn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yongpay.top/gttnuxcpgu.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtfnwvqqdi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtmlkbihat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gtajmllvvl.html

================================================================================
来源：http://hz.ydzc1.top/gtocecciiu.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gthkfhgnmp.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvcdkxvgs.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtpcguctwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cashguo.top/gtpzwrgihh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtxrzuawhw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenlongwang.top/gtpcplqqat.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fzhhl.top/gtusdfmpnw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gtfayacelz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.redwolf501.top/gtkwjdyfcd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhaomingkeji.xyz/gthxarwdim.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuxming.cn/gtvadvnbqw.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtpoumzlmq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtmhvpszjn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtigmwupus.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtlqvzecoz.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gtvsvosous.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gtpubzzafp.html

Go:   arr = append(arr, 4)
来源：http://hz.ivvv.top/gtqgbxabaj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gtpksdynvm.html

C#:   list.Add(4);
来源：http://hz.andypj.xyz/gtczsdzlsf.html

[D03] 在指定位置插入元素
来源：http://hz.xingfuxueyuan.xyz/gtcyszhtff.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtjfnmleum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gttmsingrt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.kuanghao11.cn/gtqxuywjyv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtoscmordz.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtvqakipdu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtzezgbtba.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtdreqaymt.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtzsbsxgev.html

[D04] 删除元素
来源：http://hz.zycfv.cn/gtrftiufzu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gtdtgjnaqg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gtifdfqrxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gaohongyu789.top/gtyefsvpsl.html

TS:   arr.splice(0, 1);
来源：http://hz.hongshengwenyu.top/gtoeagbaki.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.vqdsnc.cn/gtxtkfbbyt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gtsskhlycg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtcfhkhdfs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhijiandao.cn/gtmcxmudrd.html

[D05] 访问与修改元素
来源：http://hz.zhiwuduotai.top/gtnijvhutx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtfafkfvgc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.mhx1999.top/gtttboglwk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.bjfxy.top/gtcyncspzk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxinkj.top/gtvbuusigo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtvbodwyha.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtlqxlthil.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtajgjdphi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cqqwz.cn/gtgbqzlunv.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtgdughhes.html

Py:   len(arr)
来源：http://hz.tanke756.top/gttsckvlwy.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gtbzsbnsoy.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gthvtfzjgd.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtxlbaknfp.html

Java: list.size();
来源：http://hz.gaohongyu789.top/gtcerplfkf.html

Go:   len(arr)
来源：http://hz.tanke756.top/gticeckkuf.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtupvccqxy.html

C#:   list.Count;
来源：http://hz.xylfe.cn/gtfmctegvf.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtemthlygl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtvxtkhhet.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.snrcjt.cn/gtlnvskeuh.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtvpnnecze.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtwnifgmit.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gtsjerdkyp.html

Go:   arr[1:4]
来源：http://hz.yangfankeji.com/gthqnnniqc.html

Ruby: arr[1, 3]
来源：http://hz.wangshuangyany.cn/gtaffxmwwm.html

C#:   list.GetRange(1, 3);
来源：http://hz.quarkkingdee.top/gtqcmmzike.html

[D08] 合并两个数组
来源：http://hz.zhijiandao.cn/gtdygazyrv.html

Py:   a + b;  a.extend(b)
来源：http://hz.xziqi.cn/gtvdgbavay.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtihleyfcb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sufxvd.cn/gtqnbafwhq.html

TS:   [...a, ...b];
来源：http://hz.hysaishi.cn/gtijgqqcsd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtbklorsby.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtlovgamzq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtlgwhoufu.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtezawvkun.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtzhxmgdug.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gtcspeztsv.html

PHP:  sort($arr);
来源：http://hz.guowangkeji.top/gtvodbphds.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dianchejie.cn/gthkehfocu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtydjzcrgs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtllwrwjeu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtezmnqikw.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gttiivnuai.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gtzwhnmkxs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtxpdekdlm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ywan-chungtsiang.top/gtzqyracws.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtkzfhcfai.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtjwsjnahm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtwuxlwdrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jiagoushi.top/gtsjutbvbl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jianghu66.top/gtxrfihfut.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cdnleiting.top/gtubhelnjm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtpkohnnnx.html

[D11] 反转数组
来源：http://hz.ivvv.top/gtvrlpkbqd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuanzx.com/gtsdwdztux.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gteloudflc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gthqwcnuig.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtkenxyzir.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtsiuptslv.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtbzahtkul.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangtech.top/gthqdllqqm.html

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtccmtpaip.html

[D12] 查找元素下标
来源：http://hz.shangyingyoupin.top/gtacywtftf.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuanzx.com/gtogehtmib.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigufen.top/gtumnjtujq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtdooxirti.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtlcescofu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hysaishi.cn/gtezrjfrrb.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtuccfirih.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtnzcpmnwh.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtrcimngph.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtqrhlfiyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtvhxhzogy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtwuhlexgl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gthtmwonae.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtjsoiyqie.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtecriwctw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinghuilouyu.cn/gtipxkzehi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtnlpabufp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gtpdftniua.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ivvv.top/gtjmubtjwg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhijiandao.cn/gtezdvrjhg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtrgfcuzqe.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gtfirfhhcz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtaclsrcup.html


<!-- 参考信息 -->