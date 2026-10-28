代发 wailian999

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtlzpzqvgu.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuanzx.com/gtapllgbmo.html

PHP:  is_numeric($x)
来源：http://hz.jqgufenzy.top/gtagifvnxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtwpofsner.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zycfv.cn/gtqslhobwu.html

Java: x instanceof Number
来源：http://hz.hongshengwenyu.top/gtrytyhzsw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtlqwtpxfo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnxiangtu.top/gttjpbqsri.html

C#:   x is int or double or decimal
来源：http://hz.yuxming.cn/gtkfcdtnlt.html

[B14] 判断值是否在集合内
来源：http://hz.snrcjt.cn/gtbvkvdjlo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xylfe.cn/gtsxjicgfp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hysaishi.cn/gtvnvpowyo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtakrlvsbx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtykdcodlh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gtgjwyiwkn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.haohaochexian.top/gthsfovdbo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhiwuduotai.top/gtdieeozoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ybcxt.top/gtwxbqsjzc.html

[B15] 布尔运算与取反
来源：http://hz.nwbrower.top/gttveaahsp.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtjviaeait.html

PHP:  $a && $b || !$c
来源：http://hz.haohaochexian.top/gtpcybmrwn.html

JS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtzdxknnow.html

TS:   a && b || !c
来源：http://hz.yueranfly.top/gtyuvpxzhg.html

Java: a && b || !c
来源：http://hz.gogol.net.cn/gtbzagmthx.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtgzzouynb.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtafvclihn.html

C#:   a && b || !c
来源：http://hz.ehwqpu.com/gtlbmxdvki.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.fzhhl.top/gthbajwxmh.html

Py:   if not data: return
来源：http://hz.mhx1999.top/gtiaownhlp.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtlbdifzqk.html

JS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtesvgjoal.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtnpkwyixw.html

Java: if (data == null) return;
来源：http://hz.yuxming.cn/gtgsmedleb.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gttijkapiv.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtrspnphag.html

C#:   if (data == null) return;
来源：http://hz.guannengcc.top/gtepgebois.html

================================================================================
来源：http://hz.yueranfly.top/gtwdqbljrm.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gtzuloaujs.html

================================================================================
来源：http://hz.jqgufenzy.top/gthmhffupp.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gtpvrpmycl.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtpyhelvbm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtczavevqq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtxdxjfxhk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtqgtzmiid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtfekxrewx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhongyouzk.top/gteppslrkx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtfopbfako.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtvpxbtial.html

[C02] 默认参数
来源：http://hz.yonumen.top/gtecyetkpq.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtxytctopd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydzc1.top/gteqlgnzih.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtjdqmehqu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.snrcjt.cn/gtutvczixe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtyzbhjhqg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhixingplan.top/gthbjeuuao.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtwhthmzfs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sysykeji.top/gtajwescje.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtvvpjhxkd.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigufen.top/gtactyxozb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtmduecvuq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gtuujypqqu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtimbtwqiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhaomingkeji.xyz/gtggwpjmtg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sweek.top/gtwzbuhqma.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangdashe.top/gtnaidyyke.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtkdbxwfka.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtfikgvmbz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yvedp.cn/gtmjuriucw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.snrcjt.cn/gtejqiajnq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtjiaxwves.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuetiantiany.cn/gtwrelehua.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gteacypczp.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtijasfxoy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtqefgydke.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtwljnjnab.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtzgyfoxxr.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtoryupzrv.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtxtbflcvb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj202588.top/gtcpmlutlv.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtfmgqjvng.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtogkyipyr.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtwhicwhjw.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gtyalssixk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.smart0.xyz/gtgxrjkbde.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtihqdpvjb.html

Py:   square = lambda x: x * x
来源：http://hz.daxiang520.top/gtueuvkech.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtkpvbytmf.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtwgsueadj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gaohongyu789.top/gtcqchcaxb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangkeji.top/gtjhbhedqr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yangfankeji.com/gtqjikidkh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ybcxt.top/gtjpcacpau.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtlmophcqv.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gtvxyxemco.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtrrlyxlfo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pycfn.com/gtzvwmuerz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258888.top/gthnakvxcn.html

TS:   arr.map(String)
来源：http://hz.ehwqpu.com/gtsqwlxzop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtidllmqne.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtlbxyeozu.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtlqacshjq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ybcxt.top/gtoropsijw.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtdfxsyzwf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gaohongyu789.top/gtscjamyso.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.316326.xyz/gtsmxsyehc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtfkmciazs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtmvnzfpdt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuxming.cn/gtvitkjrhl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tanke756.top/gtvkpdnagq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hnqzz.top/gtwmavqetp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtkxcypryw.html

[C09] 递归
来源：http://hz.chenlongwang.top/gthcqnxluy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtgctepnkp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhijiandao.cn/gtytoybseq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hysaishi.cn/gtctjrllds.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtounsxody.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gtjtkwejwe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtbgukexga.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtcevjskoq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.guannengcc.top/gtlzpaphvr.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtkqjqyqyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenzaomai.com/gtxbbwfzja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.316326.xyz/gtitulfxfe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.quarkkingdee.top/gtnykswwvv.html

TS:   同 JS
来源：http://hz.iojbl.cn/gtszsilhwn.html

Java: 方法内为块级作用域
来源：http://hz.shuidangran.top/gtntdzjbjk.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gttfpmetrq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zycfv.cn/gtfezhqwpm.html

C#:   块级作用域
来源：http://hz.0kj1m.cn/gtkrtbacbd.html

[C11] 模块导入与导出
来源：http://hz.gzhubu.top/gttywotypp.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gteuwomkzw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gogol.net.cn/gtfoslouri.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gtzbpthjqe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shangyingyoupin.top/gtxnsvrynj.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtcmhuadoz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gthmcufdgd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gtojcofpih.html

C#:   using System.Text;
来源：http://hz.mhx1999.top/gttcrjxuyo.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtobdbrzgg.html

Py:   (lambda: print("run"))()
来源：http://hz.hywenlv.cn/gtalqdawuf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtmqgzpkhx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtatdhzekq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dianchejie.cn/gtgrflweyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtqznyixgb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtsdivbjlo.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtuduhbulh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtunomibob.html

[C13] 类型声明 / 类型注解
来源：http://hz.pengpengdd.cyou/gtzpaojmcr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtkzkqvroq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtojipnygk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtqrryflmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtghmwfkwr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtzjcfkszk.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gtdneqowsj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aizwys.cn/gtvdmjsjfa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtgbghkega.html

[C14] 泛型函数
来源：http://hz.gzhubu.top/gtjtsookln.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinyuanbaomall.cn/gtcgqvwigc.html

PHP:  // 无泛型
来源：http://hz.hongshengwenyu.top/gtkeamfeub.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtkmliifdr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gteysnioup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gthzqrtyso.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtctgmbvgb.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtlffymnde.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ehwqpu.com/gtowfqwihq.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtlmlfajem.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gtqniqipdj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.kuanghao11.cn/gtcxynjjqf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtjgsdkrbf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhoulong.xyz/gtiwlddnmp.html

Java: // 无解构
来源：http://hz.yongpay.top/gtirlsoncs.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtlpvcmbtl.html

Ruby: a, b = pair
来源：http://hz.zhengqikj.top/gtufjcdnxf.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtjlanolfp.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtnnonulng.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.snrcjt.cn/gtqhsxunqk.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtdvcwsimv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtvshqexmh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtsfbfsjem.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gtvzcnhdxh.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj202588.top/gtpstlnrze.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yanxiufei.cn/gtnthonqhp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.quarkkingdee.top/gtujalxgqi.html

================================================================================
来源：http://hz.fzhhl.top/gtiabrqtyg.html

D. 数组 / 列表 / 集合
来源：http://hz.jlsjyb.cn/gtdfgwwopb.html

================================================================================
来源：http://hz.xinyue.icu/gtgpzujcwq.html

[D01] 创建数组 / 列表
来源：http://hz.9152youxi.cn/gtqyzhnwur.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gttpgqonaw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sysykeji.top/gtxnentswt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtyddqmkcv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigufen.top/gtydfaiyrt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtyzeprolr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xylfe.cn/gtevvsmuco.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnqzz.top/gtsuepacdk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gthwvywkjw.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gteqfqdzjq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxuanxn.top/gtuldndaff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtroaojcwh.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtmuappyca.html

TS:   arr.push(4);
来源：http://hz.nwbrower.top/gtlrjhzfgd.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtxbehbgle.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtdjoyalcp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtmyaacwrt.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangkeji.top/gtcafsegdf.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtqyiynfmd.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtkuztqtbh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gtmcyfcebq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtmaedjpdb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.andypj.xyz/gturoesabl.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtulesvpyb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuxming.cn/gtffgdeihq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gtoqwsfhzw.html

C#:   list.Insert(0, 0);
来源：http://hz.sweek.top/gtbvhcmmhd.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gtwoytzqsh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtrptdghij.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guannengcc.top/gtuyravwfj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yangfankeji.com/gtyxyongyn.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtiohlbzoy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtqtldivya.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daria6918.cn/gtpntrppbf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hywenlv.cn/gtmlpzvyvu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtvolgwqoi.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtbrgenodw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtlicrrlce.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtmsmvpkub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtprjjzaho.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtavxbigxj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtoceztxcf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sysykeji.top/gtkugpphqp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuxming.cn/gtpssxzkyw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtdwkjbhjr.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtompyyfra.html

Py:   len(arr)
来源：http://hz.birdmap.top/gtxtruhgvi.html

PHP:  count($arr);
来源：http://hz.aibaodan.cn/gtdpaxmdpm.html

JS:   arr.length
来源：http://hz.xziqi.cn/gthsjuwmcx.html

TS:   arr.length
来源：http://hz.feifeiyinyue.top/gtszgamdbi.html

Java: list.size();
来源：http://hz.gzhubu.top/gtbxdfbquw.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtalhzlebz.html

Ruby: arr.length; arr.size
来源：http://hz.shuidangran.top/gtlcfxvnaq.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtyvljjcex.html

[D07] 切片 / 取子数组
来源：http://hz.chenzaomai.com/gtywivycgi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gaohongyu789.top/gtsgxovrsm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtejvrhkjv.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtqpimimgu.html

TS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gttmloczxs.html

Java: list.subList(1, 4);
来源：http://hz.birdmap.top/gtkfkwmuzh.html

Go:   arr[1:4]
来源：http://hz.ydjk.org.cn/gtkwxanwcs.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtsymuyjdu.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gttobtpefe.html

[D08] 合并两个数组
来源：http://hz.haohaochexian.top/gtuevtsaly.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtcnggslnl.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtzjehpxgi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gthaqdlyvj.html

TS:   [...a, ...b];
来源：http://hz.bjfxy.top/gtpdmourkd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.svipenyu.cn/gtghvhlygi.html

Go:   append(a, b...)
来源：http://hz.yj20258888.top/gtuyxbmnne.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dashuyun.cn/gtlxqofgrn.html

C#:   a.Concat(b).ToList()
来源：http://hz.hysaishi.cn/gtawfzpjja.html

[D09] 排序（升序）
来源：http://hz.tanke756.top/gtwbqdtyxr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtxalnudag.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtvzbdnxwq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yanxiufei.cn/gtaoedihua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tanke756.top/gtihryzljx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtjgaezscs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtsjqcoluz.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtnmgltgjw.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtijfeexip.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tanke756.top/gtcfprozck.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tianlin.xyz/gtfxeuwehv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtfudsyhdm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtlewxmjyp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtusdakttw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtjibjviba.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtrsibldwv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtwpwivyre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258.top/gtnbpsvkpg.html

[D11] 反转数组
来源：http://hz.smart0.xyz/gtxqdlijkp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258888.top/gtizusybgi.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtwidelxti.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtbmpoljvo.html

TS:   [...arr].reverse();
来源：http://hz.vqdsnc.cn/gtmpdyfbdy.html

Java: Collections.reverse(list);
来源：http://hz.xylfe.cn/gtireprfvb.html

Go:   slices.Reverse(arr)
来源：http://hz.jiagoushi.top/gtgnuvlsdi.html

Ruby: arr.reverse
来源：http://hz.yuanzhike.top/gtkskubyhq.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtmeqccwwp.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gthsiouhzl.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gtivekkogb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigfzy.top/gtyyxfdyhb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtlisqromg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtyjwrtmxd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yueranfly.top/gtvnyotsgt.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtijvlklkg.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtupuvzuen.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtbujdypfo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhixingplan.top/gtzhvfxpnh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhixingplan.top/gtbdvilbit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtpeuuxdrp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtjrgmvdqu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtoxjffypi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gtmgegxlcu.html


<!-- 参考信息 -->