代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtuzvmuetr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtffdrusrs.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenjidiqi.icu/gtvutdjqbc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtdohrumxv.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtpgnsanvq.html

Py:   def greet(name="World"): return name
来源：http://hz.feifeiyinyue.top/gtzixgipri.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtjhrcuqyh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuanzx.com/gtpppzfcnk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtrtxytctf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhiwuduotai.top/gtbanlzxfp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guowangkeji.top/gtwnuxcbgt.html

Ruby: def greet(name = "World") = name
来源：http://hz.yj20258888.top/gtupufizfl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtbgbwdziq.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gttqsmqptj.html

Py:   def total(*args): return sum(args)
来源：http://hz.sysykeji.top/gtrqbtrumo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yueranfly.top/gtlpzdwnnw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtebyiigmn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtfmqzkerk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtvgjtpuxs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gtxvucpgnv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xinyue.icu/gtolwtpeiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daxiang520.top/gtpldcqzxb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fengsongda.top/gtugeqgxug.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangdashe.top/gtkxvuajqp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.mhx1999.top/gtyyrqimuv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtpxjrdygn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sxryk.cn/gtndznewoc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.c1oappe.top/gtxrpmmuwj.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtesisiadh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtncnzhsok.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtqjnycjpp.html

[C05] 返回多个值
来源：http://hz.gaohongyu789.top/gtlgydkckv.html

Py:   return a, b
来源：http://hz.sysykeji.top/gtzhdcykah.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gtuhlibzrq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xinyue.icu/gtqjlinghi.html

TS:   return { a, b };
来源：http://hz.pengpengdd.cyou/gthfahfamg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtxbjgtkjt.html

Go:   return a, b
来源：http://hz.zhixingplan.top/gtdqeeckfs.html

Ruby: return a, b
来源：http://hz.pengpengdd.cyou/gtkamtpfdu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daria6918.cn/gtzbmpjzwq.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtiftgadoc.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtiwrluaom.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daxiang520.top/gtdxykqhzv.html

JS:   const square = x => x * x;
来源：http://hz.cheryme.top/gtqendbzlp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtqkrukixb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtceqbqvsv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fengsongda.top/gtquualgez.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hysaishi.cn/gtbhprjdbk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtxkppaqul.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtlvwzbwbh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgfzy.top/gtirqdhgne.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gthlqpjael.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigufen.top/gtkmrqwrif.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gtyoznbfpr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yueranfly.top/gtnhknnegn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guowangkeji.top/gtzjijydyh.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydzc1.top/gtdtmatnvh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtuhwgkzph.html

[C08] 闭包
来源：http://hz.birdmap.top/gtktrhhkpe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cucudq.cn/gtegyzrfvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhengqikj.top/gtvcnvosbp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtzvbpyzhp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtaqeynrco.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ehwqpu.com/gtuyvakiqj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.vqdsnc.cn/gtstgjsqrl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guowangkeji.top/gtmqlhdiuj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtvescaxfs.html

[C09] 递归
来源：http://hz.zhongyouzk.top/gtrkxopnkz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtwpzoxnhw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hongshengwenyu.top/gtirrntqvr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtiucreimr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtodymbfds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtnzjldelv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtjhjxnxyo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangtech.top/gtznfbwobn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtldrsatyu.html

[C10] 变量作用域
来源：http://hz.guannengcc.top/gteivvcnzd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hfpthk.cn/gtesbhnjbk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.svipenyu.cn/gthxcbyegu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuetiantiany.cn/gtvyqxtfbb.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtdzclvmed.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gteauyuvvu.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gttyzhhghd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fengsongda.top/gtrzrdphsb.html

C#:   块级作用域
来源：http://hz.ywan-chungtsiang.top/gtqqmtvvta.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtrbthgblz.html

Py:   from module import func
来源：http://hz.shanyushiyangkeji.top/gtakuptdye.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.iojbl.cn/gthxkfeeno.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtevzlengm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtdytczqwi.html

Java: import java.util.List;
来源：http://hz.shangyingyoupin.top/gtfjlxatcj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtdfohzrhd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtqefczmdc.html

C#:   using System.Text;
来源：http://hz.jinqigfzy.top/gtjgihhgrp.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gtwbkcredj.html

Py:   (lambda: print("run"))()
来源：http://hz.chenjidiqi.icu/gtcpqhiubg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtelqovjzj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gttktezoza.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtzeynrwzp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tanke756.top/gtyyiepdrp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.52xcode.cn/gtqfcnqwdn.html

Ruby: -> { puts "run" }.call
来源：http://hz.xylfe.cn/gtpgclssje.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yongpay.top/gtgkrhuixn.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtrgqfidrk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gthaotowpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtxjkdomuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtxtpojjan.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gttyqyombu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtqvwtcxeb.html

Go:   func add(a, b int) int
来源：http://hz.guannengcc.top/gtlfgziazm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigfzy.top/gthcqyvdqe.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtrjrcbrop.html

[C14] 泛型函数
来源：http://hz.jlsjyb.cn/gtidnqhrao.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtgyziqsrg.html

PHP:  // 无泛型
来源：http://hz.ppjwa.cn/gthlulvpsg.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtsyvoqjwn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gtdihbnwsp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtbtbzaste.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtumauvjfl.html

Ruby: # 无泛型
来源：http://hz.havefunace.top/gtdibpqxhx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtnymbyjfs.html

[C15] 解构 / 展开参数
来源：http://hz.fengsongda.top/gtvwcykyyf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinghuilouyu.cn/gttzwvickn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guowangkeji.top/gtrburunvo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtlyjnzufu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtxyydbgka.html

Java: // 无解构
来源：http://hz.guowangkeji.top/gtdokvqkhd.html

Go:   // 无解构
来源：http://hz.jiagoushi.top/gtewovpadp.html

Ruby: a, b = pair
来源：http://hz.pycfn.com/gtpgcslxjx.html

C#:   var (a, b) = pair;
来源：http://hz.c1oappe.top/gtygdkmvva.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtrytlsxtg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtfrxrwczf.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtptzobkoa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.meibo888.top/gtblxfgfur.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xylfe.cn/gtreuplqdk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtgkxdexgu.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtvfxbhexf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtdtzqypkk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtshvqelqe.html

================================================================================
来源：http://hz.dianchejie.cn/gtizwislei.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtsbiutzga.html

================================================================================
来源：http://hz.yvedp.cn/gtbiivhexj.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gtmstkqwhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtlambseky.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtgkqgnnkl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhongyouzk.top/gtneagmbxc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtgehtmwyg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.snrcjt.cn/gtzxsyfyym.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtqtygkkhp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jianghu66.top/gtcavejspj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.smart0.xyz/gtnsbsuwid.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtwqhghwnz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtehhivuoe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtdosmtvgr.html

JS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtgoorakua.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtffiitjei.html

Java: list.add(4);
来源：http://hz.xingfuxueyuan.xyz/gtqnhalvje.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258888.top/gtwdpxihou.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shangyingyoupin.top/gthjwjxezd.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtuksmhjlx.html

[D03] 在指定位置插入元素
来源：http://hz.yj202588.top/gtwqfelfop.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtcidkmgut.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.feifeiyinyue.top/gtthqvkhsr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtpkhjquqz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cucudq.cn/gtolsrbntq.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gtcmqzyclr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhiwuduotai.top/gtmixgayqi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.316326.xyz/gtsczprkhu.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangtech.top/gtfnauybif.html

[D04] 删除元素
来源：http://hz.hnqzz.top/gtydqvfnqh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtecusnutr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtqhjyrzfx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtsapnzoxw.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtwjgvmpds.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hammf.cn/gtnjgwgswx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.haohaochexian.top/gtniytvmqi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gtoywthqoy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtdxwtokjn.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtswzjqxhj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtdfrnlogt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yangfankeji.com/gtsjpcfzkx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yueranfly.top/gtimhscrkx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtnwbtotpq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gttppqqjlj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtgdtbiare.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gthismztej.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tian-w.cn/gtmkaobfum.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtojnbqoam.html

Py:   len(arr)
来源：http://hz.shangyingyoupin.top/gtdxuisonn.html

PHP:  count($arr);
来源：http://hz.yj20258.top/gtwqrkfibb.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtdwysyegg.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtaecjcvuk.html

Java: list.size();
来源：http://hz.nanxinkj.top/gtuxiojfky.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtkbbeynig.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangkeji.top/gtufwuucke.html

C#:   list.Count;
来源：http://hz.hysaishi.cn/gtlfoysukk.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtxcmpvnpg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtooegaksb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ywan-chungtsiang.top/gtlpvomksv.html

JS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtssplwloa.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtvdguragb.html

Java: list.subList(1, 4);
来源：http://hz.yuanzhike.top/gthrnwowih.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtnmjuoxft.html

Ruby: arr[1, 3]
来源：http://hz.smart0.xyz/gtlsjnjdun.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtglrvkspo.html

[D08] 合并两个数组
来源：http://hz.pycfn.com/gtwzbgxhpq.html

Py:   a + b;  a.extend(b)
来源：http://hz.sweek.top/gtaciuthup.html

PHP:  array_merge($a, $b);
来源：http://hz.gaohongyu789.top/gtzintpqgh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtgugejnmc.html

TS:   [...a, ...b];
来源：http://hz.smart0.xyz/gtbxqkuqwr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.aibaodan.cn/gtdlfonesg.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtmljrdkel.html

Ruby: a + b;  a.concat(b)
来源：http://hz.havefunace.top/gtggolflvq.html

C#:   a.Concat(b).ToList()
来源：http://hz.aizwys.cn/gtnnggloss.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtwpyuagda.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtdsyypwwq.html

PHP:  sort($arr);
来源：http://hz.ydjk.org.cn/gtwuuaagqh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dianchejie.cn/gtjvkrlatm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zycfv.cn/gtsyccipqw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xinyue.icu/gtmveymtmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtfwjbagdv.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtyvzzbtfr.html

C#:   list.Sort();
来源：http://hz.fengsongda.top/gtosspdast.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtyfllxelr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtiswtdghx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtwelfouxk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gthsodniza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtqkebounq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gzhubu.top/gtpwbbdtpo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.0kj1m.cn/gtmxknpszt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gzhubu.top/gtarczpdir.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aizwys.cn/gtausiesvl.html

[D11] 反转数组
来源：http://hz.jlsjyb.cn/gtiazvspkz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.kuanghao11.cn/gthcyeybpk.html

PHP:  array_reverse($arr);
来源：http://hz.gogol.net.cn/gtbfokcquf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtnjwkevzs.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtpedmpllc.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gthrkvrrhl.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtcnakmqlo.html

Ruby: arr.reverse
来源：http://hz.yuxming.cn/gtalnpzuon.html

C#:   list.Reverse();
来源：http://hz.gotoacloud.top/gtcnruxuga.html

[D12] 查找元素下标
来源：http://hz.yuxming.cn/gtpawqiynr.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gthpbegfue.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xziqi.cn/gtqqqmiyen.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtbltwtbsu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gtwdcvnqsp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shanyushiyangkeji.top/gtlzcscqga.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtlvibikwa.html

Ruby: arr.index(x)
来源：http://hz.yuanzhike.top/gteayqdpwb.html

C#:   list.IndexOf(x);
来源：http://hz.xuanzx.com/gtjxrdffca.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtvylbeorf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtpjrduvhf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtlegfmaxn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtijifmemd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtcwaflkuw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jyoumei.cn/gtrgfbcwhd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtzayspiyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.9152youxi.cn/gtiltbowgx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.kuanghao11.cn/gtdmgwwcvs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtjhgvdejo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.kuanghao11.cn/gtzfeweikh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.316326.xyz/gtluypomst.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gttatuhuwf.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtofpiqrpi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtyuabnqob.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gthziarycd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zdqjudy.top/gtdxsnzusn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtnvhmgoyd.html

[D15] 去重
来源：http://hz.yj202588.top/gtltuqhacm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtctxkonet.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtuqrwfeif.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtiyklylys.html

TS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtyopbvzzj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gtnzahbeyo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtokrplorh.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtuftxvusx.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gtqwocmzsr.html

[D16] 求和与平均值
来源：http://hz.vqdsnc.cn/gtvgaoptro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenzaomai.com/gtllmjoalf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtjfhfglkq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtezweqwih.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtohvvqqwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtbqgvfnor.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtmabheomy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.vqdsnc.cn/gtjlczqvua.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gtvztqqvhh.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtinquzumf.html

Py:   max(arr);  min(arr)
来源：http://hz.sweek.top/gtoynhtjtl.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigufen.top/gtuenryqgk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtlmiuirvw.html

TS:   Math.max(...arr);
来源：http://hz.kuanghao11.cn/gtpxxltley.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtnlhpipqu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nwbrower.top/gtubnqgtcd.html

Ruby: arr.max;  arr.min
来源：http://hz.quarkkingdee.top/gtbdcgduux.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gttdksneis.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtibeefoql.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gtxdnjnlhg.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtbtyfqfsg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtkcttyssv.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtaglyxwrn.html


<!-- 参考信息 -->