代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtguwuepyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtteuqmknj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtswmmcpos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtyxswvqnb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gtnfklynhp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gtlatulsrd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hywenlv.cn/gteshsxkea.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtmxybefgu.html

[C02] 默认参数
来源：http://hz.wangshuangyany.cn/gtgxkqnkrq.html

Py:   def greet(name="World"): return name
来源：http://hz.wangshuangyany.cn/gtstpjccxi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtorakerga.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cheryme.top/gtwxynweei.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtyorlsgou.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtufztsyka.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ivvv.top/gtfvbpmerj.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gttjubziys.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtpfrtvnwr.html

[C03] 可变参数
来源：http://hz.nanxuanxn.top/gtadlevyzu.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gturwlcgog.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtndtiufdz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gthhgklorp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtppukbqgs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtnziuvfru.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtuzrxtgtf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guannengcc.top/gtaihygesx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtxishqxnp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pengpengdd.cyou/gtxphxoyfr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gtouuhehpq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zdqjudy.top/gttzcanrxz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtqoiowtmg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.52xcode.cn/gtggmprdrf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daria6918.cn/gtmixzbske.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtcwxhishz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtrhrvdamn.html

C#:   f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gthmwlagmc.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtcgnldael.html

Py:   return a, b
来源：http://hz.havefunace.top/gtfnfaqdwo.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtakmneolf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.52xcode.cn/gtonsmvpvx.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtmagyafge.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gtmxnixbwg.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gttcegivyi.html

Ruby: return a, b
来源：http://hz.jinqigufen.top/gtuqstgouv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nwbrower.top/gtnbkiwhih.html

[C06] 匿名函数 / lambda
来源：http://hz.zycfv.cn/gtfutgsshp.html

Py:   square = lambda x: x * x
来源：http://hz.snrcjt.cn/gtqznezmtm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cucudq.cn/gtjlclclze.html

JS:   const square = x => x * x;
来源：http://hz.hammf.cn/gtrrxikooh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtmfaornml.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gtiticqxqg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ppjwa.cn/gtzbqrozyo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhijiandao.cn/gtucjrbybt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hywenlv.cn/gtsomtzjad.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtbziseidg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gthqwshmgw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gtjmpojtnq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtcugmshhz.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtbggcewro.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tianlin.xyz/gtiiedijsi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ybcxt.top/gtgpxzssia.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtbkfsuevc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtatkvbpfd.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtxqpryhdi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cheryme.top/gtcryaxhdh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtlpcyllpa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtudlxreia.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtifbamiru.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtiotujxpu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtdsicuggp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yangfankeji.com/gtmhrlhpew.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtbasaiyfq.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtanhmnkxc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtmsotzpfn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtvnduovfa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gtchqxeunl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtnmyfeffw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtzwkujzvl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gtwiqibigc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gtmrmnrarc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yvedp.cn/gthhzwpiof.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtynluszha.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtoyrksmjv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dashuyun.cn/gtmoseisuh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zycfv.cn/gtrmqyewri.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtrlctttao.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtwvhedlmp.html

Go:   花括号块级作用域
来源：http://hz.ehwqpu.com/gteaarhudj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtmygouujg.html

C#:   块级作用域
来源：http://hz.jinqigfzy.top/gtehdfizrc.html

[C11] 模块导入与导出
来源：http://hz.yangfankeji.com/gtsjtzikpc.html

Py:   from module import func
来源：http://hz.yongpay.top/gterqgakae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenlongwang.top/gtzvoafntp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.iojbl.cn/gthimxxukb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtwcxznjfp.html

Java: import java.util.List;
来源：http://hz.shangyingyoupin.top/gtnezbmejh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtjyrspigq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtryzmxrqk.html

C#:   using System.Text;
来源：http://hz.yonumen.top/gtnqroefgk.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtxjeizjjg.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtbsaroele.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtubhoeesj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtrktfhukh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtcfstwqrx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydzc1.top/gtpmdwqeci.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jiagoushi.top/gtavziipfw.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtmemjcepu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ivvv.top/gtdjxnmqdv.html

[C13] 类型声明 / 类型注解
来源：http://hz.jiagoushi.top/gtmsgbfkpl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnxiangtu.top/gtnyoncagr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtyxtdbges.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtkrwudpzq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtpopybpyt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtmxyojyjc.html

Go:   func add(a, b int) int
来源：http://hz.tianlin.xyz/gtcwxazhyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.meibo888.top/gtltbwzshb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ybcxt.top/gtveqruxnr.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtlaywmdfj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydjk.org.cn/gtwxefvpda.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtvgazyhfh.html

JS:   // 无泛型
来源：http://hz.ydzc1.top/gtdxikinvg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtoulnaqrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtgxbxkeii.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jianghu66.top/gtvgcwedsl.html

Ruby: # 无泛型
来源：http://hz.ywan-chungtsiang.top/gtybnegefk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gtamyddmvl.html

[C15] 解构 / 展开参数
来源：http://hz.wangshuangyany.cn/gtifjpcbvh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtlvnaniwx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtmvluwjcv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtiqvsqfar.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtehdmerhb.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtuzcsresx.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gtkqgfyuwl.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtjmfqglco.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtqbojqdji.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtmgvjluip.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.snrcjt.cn/gtqjkqiffo.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtrvgdohty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtzngyiwju.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtycxuummr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtjkuulirh.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtnrpnegzc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtmjwtzset.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guowangkeji.top/gtyddletud.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyhuwlkyc.html

D. 数组 / 列表 / 集合
来源：http://hz.zhaomingkeji.xyz/gtjbngyvsn.html

================================================================================
来源：http://hz.redwolf501.top/gtngdohtmg.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtpmlfsixm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.kuanghao11.cn/gtfxyibdke.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtpwnftqkt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtidqtlxaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangkeji.top/gtgoejsadk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yongpay.top/gtfdhshbxx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhijiandao.cn/gtgbbrgpis.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtgqciykra.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhiwuduotai.top/gtkuprlebg.html

[D02] 追加元素到末尾
来源：http://hz.cheryme.top/gtlupbteww.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhiwuduotai.top/gtwavqtfls.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtzyjxjbna.html

JS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gthvklzrxi.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtumfahtng.html

Java: list.add(4);
来源：http://hz.yangfankeji.com/gtnulqqiyi.html

Go:   arr = append(arr, 4)
来源：http://hz.daxiang520.top/gtgntcbupz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.redwolf501.top/gtevfruxdp.html

C#:   list.Add(4);
来源：http://hz.ivvv.top/gtevoqlfak.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtyczrbiic.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtrupdtarl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yueranfly.top/gtkidgjocy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtuohoihgk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.haohaochexian.top/gtdilknmso.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtrrywsvox.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtphwxlqwu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtcgdegyxa.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtjrycvutc.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gtybdohtsq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtcyqsrhwq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigufen.top/gtdmlmgvyo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.c1oappe.top/gtqyfflbmp.html

TS:   arr.splice(0, 1);
来源：http://hz.redwolf501.top/gtnswphytq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhengqikj.top/gtxhwhezex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtdskoprwj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtbjscaplg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtxfbfoguz.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gttfmlhcfn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtqlpnbutv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtkszeogxv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yongpay.top/gtdlpmcosa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gttycraqij.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtsqdoaiyl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtvbpsbaro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtkxjzjtde.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtegwckezv.html

[D06] 数组长度
来源：http://hz.xuetiantiany.cn/gtpsvfzklt.html

Py:   len(arr)
来源：http://hz.cdnleiting.top/gtpzgqabhe.html

PHP:  count($arr);
来源：http://hz.cqqwz.cn/gtzhmspqwx.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtucssnpgw.html

TS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtiormseet.html

Java: list.size();
来源：http://hz.sysykeji.top/gtvqmlsoma.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtlrebqseg.html

Ruby: arr.length; arr.size
来源：http://hz.yj202588.top/gtkfstktam.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtndbrvnfo.html

[D07] 切片 / 取子数组
来源：http://hz.nanxinkj.top/gtpfcctsuo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtcisckknt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sysykeji.top/gtnvjpjyia.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtehqbkafq.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtbqogxzgg.html

Java: list.subList(1, 4);
来源：http://hz.yvedp.cn/gtqtiippam.html

Go:   arr[1:4]
来源：http://hz.jlsjyb.cn/gtrfxysfpl.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gtuevlynmr.html

C#:   list.GetRange(1, 3);
来源：http://hz.redwolf501.top/gtbagbvsmc.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtaydhnmli.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gtanaektoi.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtmntoqlig.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtcmjnvtte.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtvztcfquv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtvjowliot.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtzmluwvxx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.kuanghao11.cn/gtqsqgbpkq.html

C#:   a.Concat(b).ToList()
来源：http://hz.zdqjudy.top/gtyauglcal.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtifmvclqh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtbjeqbnuq.html

PHP:  sort($arr);
来源：http://hz.316326.xyz/gtotuifzzd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenjidiqi.icu/gtsqmmqlsd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtwptdyegw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtmcgokrdx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gteunmfqrp.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtitulyjbt.html

C#:   list.Sort();
来源：http://hz.zdqjudy.top/gtduxsowvf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtanfbppow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.haohaochexian.top/gtnhlqsrpx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtjtlyvpke.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtkaogrquq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtjiyikeyq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtuhhlgknv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxinkj.top/gtzafewakc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dianchejie.cn/gtlufdosjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtvjjpqhed.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtffhhqnfl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gogol.net.cn/gtljujyyjt.html

PHP:  array_reverse($arr);
来源：http://hz.aizwys.cn/gtlgcxuwzr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangdashe.top/gtablwkrbk.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtbdtirvgs.html

Java: Collections.reverse(list);
来源：http://hz.chenzaomai.com/gtuhmbqkfu.html

Go:   slices.Reverse(arr)
来源：http://hz.52xcode.cn/gtofqmwdgb.html

Ruby: arr.reverse
来源：http://hz.sufxvd.cn/gtiqhxingm.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtczkamcsi.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtadfexubc.html

Py:   arr.index(x);  x in arr
来源：http://hz.fzhhl.top/gtvqertxiy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtfpkxfunt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gteeamkqmo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtckzkucxd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtoeixnnpn.html

Go:   slices.Index(arr, x)
来源：http://hz.jiagoushi.top/gtyvshpbye.html

Ruby: arr.index(x)
来源：http://hz.nanxinkj.top/gtclwwzqvb.html

C#:   list.IndexOf(x);
来源：http://hz.c1oappe.top/gtfjdeggwe.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuetiantiany.cn/gtkqlygtyz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtrkfxhdex.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtojcwuaee.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtuhlykpmu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtmimueosi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cheryme.top/gtukasjwmj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gtifnjnjvs.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtlxziehah.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinghuilouyu.cn/gtbpkzhgoj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xylfe.cn/gtepnvobzk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtndxmodeg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nwbrower.top/gthspgggif.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtfvmigvho.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtvyskzdfu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtarncsjia.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtlgaytjxm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ybcxt.top/gtejeemiiw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.snrcjt.cn/gtkimvgfto.html

[D15] 去重
来源：http://hz.iojbl.cn/gtqophyhfq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtfkjnelpg.html

PHP:  array_unique($arr);
来源：http://hz.316326.xyz/gtothsivgw.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtxrtskouh.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtfvajxdnc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.316326.xyz/gtalkebrkp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtmjpmgxuw.html

Ruby: arr.uniq
来源：http://hz.svipenyu.cn/gtqobfpwlq.html

C#:   list.Distinct().ToList()
来源：http://hz.chenzaomai.com/gtumehklce.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gthfxnekpr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtmgbemase.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dashuyun.cn/gtzrxtcetq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtetfanmrc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtjbsmipru.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtbynauatj.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtrjlsasco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtjwwwnnfs.html

C#:   list.Sum();  list.Average()
来源：http://hz.gotoacloud.top/gtuupjnvrk.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtvbumqdyp.html

Py:   max(arr);  min(arr)
来源：http://hz.chenzaomai.com/gtqlpvacty.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtezjgcsns.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gtimdtfmwi.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtwuchcoiq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aibaodan.cn/gtmyaeijzv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtphntbmfw.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigfzy.top/gtjbvqtobs.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtkricvxla.html

[D18] 扁平化嵌套数组
来源：http://hz.meibo888.top/gtsuygyljr.html


<!-- 参考信息 -->