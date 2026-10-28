代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.9152youxi.cn/gtmmzvwalx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gogol.net.cn/gtragshbsn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guowangkeji.top/gteggsihfk.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gttpxnbcbq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtnnxwxbsl.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtsurixfdw.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtcpyizmtn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hfpthk.cn/gtlkvobwuk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tianlin.xyz/gtbllhaqog.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtmexwydtu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtljatbeig.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guannengcc.top/gtfmtwkufj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nwbrower.top/gtpsmixsmg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yangfankeji.com/gtfzqpshqt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.meibo888.top/gtzqbfmwye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtsnhowijp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jlsjyb.cn/gtpslimqyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtpnllorgw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gtgjiaekyc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtcockjwvb.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gttekhwimy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtnepxymwx.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gthihqfqmh.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gtopmzsxxn.html

Py:   return a, b
来源：http://hz.smart0.xyz/gtldaoekou.html

PHP:  return [$a, $b];
来源：http://hz.ppjwa.cn/gtuvymbtqq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fzhhl.top/gtafdahwmi.html

TS:   return { a, b };
来源：http://hz.fengsongda.top/gthzjowodk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.316326.xyz/gtjrjbblvk.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtuzdydxny.html

Ruby: return a, b
来源：http://hz.9152youxi.cn/gtugtghgks.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtelixuywf.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtuedjkczu.html

Py:   square = lambda x: x * x
来源：http://hz.aizwys.cn/gthssqlxsy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gterwmlxjk.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gtndemgxkh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nwbrower.top/gtwemxyijy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtjypukmas.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtuxtzxliy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtbkrzhxxe.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shuidangran.top/gtdjrxhuff.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtqzisoznp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cqqwz.cn/gtsmzmnymf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cashguo.top/gtiwcrykod.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.0kj1m.cn/gtququvynm.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtbiuarvub.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xingfuxueyuan.xyz/gtgbestwzi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenzaomai.com/gtplyludfi.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigfzy.top/gtcxxwzzgc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtknvoxjnt.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtxzhsftzo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigufen.top/gtjbjrjxnr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shangyingyoupin.top/gtxwezuxkw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtwiucdzsy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtccaecokg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtjgwvyxbz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenjidiqi.icu/gtgrjbuiyx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gtiswycozq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtpjjtaxrf.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtvnalrdks.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtcpovnajf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtfcgcciyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtxxrpxxny.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gthesnojxz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shzxlz.cn/gtozssemdn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtubsumkvb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtghwvjsub.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.bjfxy.top/gtngyesoxf.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtkkjvdfxg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinghuilouyu.cn/gtzwatvpjw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtakdrywih.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258888.top/gttgwcityr.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtbhwshdkg.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtvrhaaoke.html

Go:   花括号块级作用域
来源：http://hz.tianlin.xyz/gtnznyzdrk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gzhubu.top/gtdvosckoe.html

C#:   块级作用域
来源：http://hz.yongpay.top/gtjhvcibkw.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtlvpwwkca.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtvjelgxmx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtdofhqsse.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtzegkpzzo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydjk.org.cn/gtcfiuuazf.html

Java: import java.util.List;
来源：http://hz.ydjk.org.cn/gtxzqhxzla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtoojsmhys.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtwiqthzlb.html

C#:   using System.Text;
来源：http://hz.shanyushiyangtech.top/gtucfrumyd.html

[C12] 立即执行函数 IIFE
来源：http://hz.yanxiufei.cn/gtcelepjjt.html

Py:   (lambda: print("run"))()
来源：http://hz.meibo888.top/gtjeikeyzo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gteqlkwlqp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtnoifkcwz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtiixreqgl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhengqikj.top/gtyhkginzj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtyljwpzgw.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gthsajatdi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gtezycbnaq.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtnlywvmsq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtyozzvivv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtcfmhscvo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtilhfhgfo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtblzfrukq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtfjaddkyt.html

Go:   func add(a, b int) int
来源：http://hz.nanxinkj.top/gtvlezjece.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtvujzmjjv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gttvysuxyy.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gteasndyun.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.andypj.xyz/gtvdrvvwhn.html

PHP:  // 无泛型
来源：http://hz.zhoulong.xyz/gtepzqgqej.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtmsjqhxbo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtuhszpqzi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hywenlv.cn/gtubmiersc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtllvgqvaj.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtdvopozqi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtqdylikzq.html

[C15] 解构 / 展开参数
来源：http://hz.sysykeji.top/gtrwozgwch.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.snrcjt.cn/gtyayiwuif.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtzxcmlimg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtnqnofptc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtwqnbtrwa.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gtpronquej.html

Go:   // 无解构
来源：http://hz.fengsongda.top/gtbxavzzww.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gttkzrqpwf.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gttttmopjd.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtgjlcbfix.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.quarkkingdee.top/gtpfmfdwwf.html

PHP:  // 无重载
来源：http://hz.ppjwa.cn/gtokwuxrlu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jiagoushi.top/gtwneneduc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gthxhipfsa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daxiang520.top/gtpxnuuduy.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtgcaadddq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtrwzgdgbk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.kuanghao11.cn/gtnqlokkfb.html

================================================================================
来源：http://hz.gogol.net.cn/gtgnootsrq.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtweqjqffr.html

================================================================================
来源：http://hz.nwbrower.top/gtvhmktlwl.html

[D01] 创建数组 / 列表
来源：http://hz.yuanzhike.top/gtgiefxhcb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gttudlvmun.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtzrawdnzp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtnwliolof.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.0kj1m.cn/gtlfyabdjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtpqainsuc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtyncyvguq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtmlseeilf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtmnkjpuvv.html

[D02] 追加元素到末尾
来源：http://hz.shanyushiyangkeji.top/gtbbtbybbf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gtmksrsrbs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtjznjdkwz.html

JS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtbhecwoka.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtebgpmxrf.html

Java: list.add(4);
来源：http://hz.hnxiangtu.top/gtgiayfile.html

Go:   arr = append(arr, 4)
来源：http://hz.hongshengwenyu.top/gtariinzvi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gtlqsxdfkz.html

C#:   list.Add(4);
来源：http://hz.chenzaomai.com/gtjjimrumr.html

[D03] 在指定位置插入元素
来源：http://hz.guannengcc.top/gtzgststom.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtffhuxxil.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtfsgubcxw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtafgrtake.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gtnpstaatb.html

Java: list.add(0, 0);
来源：http://hz.aizwys.cn/gtjhuvvlwo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtaxqcqurt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.iojbl.cn/gtohjsrcwd.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtbtbblvep.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtlsamhjrj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cashguo.top/gtgquvkbtk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yueranfly.top/gtsqrnwlnj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.bjfxy.top/gtrquxoglt.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gtqllzxiab.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gtsmvrmgpz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtkjoaaccy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtlcmlyxty.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gthqyvnype.html

[D05] 访问与修改元素
来源：http://hz.yuxming.cn/gtmorezopx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtniprjvuy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.52xcode.cn/gtwbxnxucp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guannengcc.top/gtrxbcxkqh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtgyvmwpfz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtajjwwqdq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.c1oappe.top/gtenmcmbpp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtcjfzlfgd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guowangkeji.top/gteabibgtd.html

[D06] 数组长度
来源：http://hz.0kj1m.cn/gtlnufhuib.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtvjzlbqpv.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtfpsxvyon.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtlohqwhtj.html

TS:   arr.length
来源：http://hz.chenlongwang.top/gtjncodlvh.html

Java: list.size();
来源：http://hz.chenjidiqi.icu/gtpnpqnczu.html

Go:   len(arr)
来源：http://hz.9152youxi.cn/gtwevthiub.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gtrayhuwhz.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtkscwwmwi.html

[D07] 切片 / 取子数组
来源：http://hz.iojbl.cn/gthheegtfz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gtjgkstyxu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yangfankeji.com/gtwaugyzhq.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gticqwpgte.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtdrtxcpae.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtuacnqbgd.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtvtfokmox.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtwpoaygcf.html

C#:   list.GetRange(1, 3);
来源：http://hz.tianlin.xyz/gtxyyxrarh.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtbtgokkah.html

Py:   a + b;  a.extend(b)
来源：http://hz.hfpthk.cn/gtkeshfwif.html

PHP:  array_merge($a, $b);
来源：http://hz.9152youxi.cn/gtjmxvdbre.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gtujewphzt.html

TS:   [...a, ...b];
来源：http://hz.0kj1m.cn/gtztivoyth.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gttszlslmw.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtyjrbxyrx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gttgepctzy.html

C#:   a.Concat(b).ToList()
来源：http://hz.xinyue.icu/gtplnzrtvx.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gtvfvoiavd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtyhjeuzow.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtfesmcsmc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinyuanbaomall.cn/gtpwfqvfns.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guowangkeji.top/gthfvouzvd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hammf.cn/gtlwnjflqu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtkwowzbse.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtiegpgxdn.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtwmqlnoic.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtnuyvanyl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gthirwthrp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtlarncesm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtriazsrrj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtaivnkcif.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtpzeciefa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pengpengdd.cyou/gtwphjkssm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gtguquhrca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.smart0.xyz/gtejvhheam.html

[D11] 反转数组
来源：http://hz.cucudq.cn/gtfluysoco.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.vqdsnc.cn/gtnobkonkl.html

PHP:  array_reverse($arr);
来源：http://hz.havefunace.top/gtjaugthso.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtdelvghtx.html

TS:   [...arr].reverse();
来源：http://hz.ydzc1.top/gtxwhoyyda.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtyomcxggd.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtlnlcvpow.html

Ruby: arr.reverse
来源：http://hz.jiagoushi.top/gtvvtrdmlj.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtnxxybgeo.html

[D12] 查找元素下标
来源：http://hz.chenjidiqi.icu/gtmzmtqpze.html

Py:   arr.index(x);  x in arr
来源：http://hz.svipenyu.cn/gtofjsbvzk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xziqi.cn/gtrwdwljpt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtjzntvcfc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtwidjekmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gtidujuvzv.html

Go:   slices.Index(arr, x)
来源：http://hz.yj202588.top/gthfrgjuak.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gtzrsvlrwm.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtvjevsbpf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhixingplan.top/gttxibbzuw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtqwtmwzmm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtwdmwnyoc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtgyhlqcko.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtjweumzax.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gtuzmtltjz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.snrcjt.cn/gtligscupg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtezhbqpuj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gthrpjbmlq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydzc1.top/gtfclkhxfi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gtdrzdxpnk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gtheddzaez.html

JS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gttvofjvia.html

TS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtnesheuzk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtvgjslfww.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtnxusmmud.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtofdvtgsc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yueranfly.top/gterrxxhwg.html

[D15] 去重
来源：http://hz.daxiang520.top/gtzrkxsceo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtayxvlwsm.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gtfygiabqa.html

JS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtyknlexgl.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtqyfkvqna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtwpxwovdz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.0kj1m.cn/gtfyqxzorj.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtrypforus.html

C#:   list.Distinct().ToList()
来源：http://hz.jyoumei.cn/gtasfhgwok.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gthzqusjju.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtbkhccywe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtfflkdreq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtqrzavbos.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtmfhhazes.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhaomingkeji.xyz/gtuudzfdjx.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtteprqhkb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gaohongyu789.top/gtynwheuef.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangshuangyany.cn/gtypfmzbca.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gttitkvgwo.html

Py:   max(arr);  min(arr)
来源：http://hz.sufxvd.cn/gtsfgdvumj.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtymuniuqo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtpxedzwvq.html

TS:   Math.max(...arr);
来源：http://hz.xziqi.cn/gtdrmezstg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtilopcspa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.9152youxi.cn/gthpalmrbi.html

Ruby: arr.max;  arr.min
来源：http://hz.yongpay.top/gtiiqcacty.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtjeieydfb.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtikpmkley.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtwhbibtoe.html

PHP:  array_merge(...$nested);
来源：http://hz.jlsjyb.cn/gtuuaaykeg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.iojbl.cn/gtvpdtppvp.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtszaodcqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtpuypsviy.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtxtxjtmzp.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtibgjfykt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.0kj1m.cn/gtsmdhyxqj.html

[D19] 按字段分组
来源：http://hz.svipenyu.cn/gtvwsyxhzz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangkeji.top/gturefzuiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhiwuduotai.top/gtpecxbwed.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtksrhgmaa.html


<!-- 参考信息 -->