代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtwcumwtvu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtgcenfhas.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nwbrower.top/gtvlqsprxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zycfv.cn/gtdxzblwfi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pengpengdd.cyou/gtlsxlkpfs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gtbshtokwd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shangyingyoupin.top/gtlmrpgnif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zdqjudy.top/gtwdzqtqdp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtqgijmimi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtqoudxkpa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhixingplan.top/gtcgpzmfos.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtmkslvjec.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gtjvxlcqkh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtbdfewfyh.html

C#:   f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtcslvmooc.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gtkjlbvhih.html

Py:   return a, b
来源：http://hz.xylfe.cn/gthlgstlpb.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtwaqbcmsq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tian-w.cn/gtxhyuromb.html

TS:   return { a, b };
来源：http://hz.jiagoushi.top/gtujnmbuzo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtvhwflyzv.html

Go:   return a, b
来源：http://hz.ybcxt.top/gthrdcsxzu.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtldccunsf.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtkgdygggd.html

[C06] 匿名函数 / lambda
来源：http://hz.wangshuangyany.cn/gtiblwwozt.html

Py:   square = lambda x: x * x
来源：http://hz.dianchejie.cn/gtxvbpcpid.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gtqftqfjla.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtckfoyhhe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtvsgwrgvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gteqbynggs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.52xcode.cn/gtijyictrd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gtxufacgos.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtrcqpdvrv.html

[C07] 把函数作为参数传入
来源：http://hz.shuidangran.top/gtouychdia.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtttjdbrzs.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.iojbl.cn/gtfcpqvqqt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shuidangran.top/gtimivgvsd.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtkgrrdxnp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sysykeji.top/gttmooyprw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.havefunace.top/gtzhldsehq.html

Ruby: arr.map(&:upcase)
来源：http://hz.yonumen.top/gtmlolxowr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.kuanghao11.cn/gttlhvrctc.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtzgjwgamx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtolnhntvi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ppjwa.cn/gtaufvurvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtcbixmdoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtjpbpoixp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtufzhwyni.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangdashe.top/gtayohelsu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hammf.cn/gtvbiuvzuz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gttxmyaint.html

[C09] 递归
来源：http://hz.havefunace.top/gtmdqtmxzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtlerpvyrq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgufenzy.top/gtatewvfho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gtctobxgrp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtjjdmjdvv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtcifqrkpe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258888.top/gtajszovkh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtrtxkhevb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtsxhpikzt.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtupbawvhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinyuanbaomall.cn/gtixpjjutu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gtwmgdawll.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtsbdlooka.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtdoltznvx.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gtlwgfhkag.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtstibvobn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cucudq.cn/gtqcrjqdqp.html

C#:   块级作用域
来源：http://hz.yueranfly.top/gtinboxeuw.html

[C11] 模块导入与导出
来源：http://hz.ehwqpu.com/gtnbnwplyk.html

Py:   from module import func
来源：http://hz.tanke756.top/gtydqoszjb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtvtskhaxa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gtjxewjtle.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtqxokdcfj.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtfrlaaxgm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtkxieabht.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hammf.cn/gtievzwwhg.html

C#:   using System.Text;
来源：http://hz.cashguo.top/gtkbzasjqq.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtqexvayif.html

Py:   (lambda: print("run"))()
来源：http://hz.sysykeji.top/gtskaaqrgd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtlgkqbqfd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtmkggwhbu.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtqokboweh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtysgiuszd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenjidiqi.icu/gtzheqbovx.html

Ruby: -> { puts "run" }.call
来源：http://hz.yonumen.top/gtsgypslpm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtngvmlvcc.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtngrmvcfc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.0kj1m.cn/gtdkgcbvku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtjtvvdlzy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtmahqppth.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtcvvwwuom.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtcfocjqdw.html

Go:   func add(a, b int) int
来源：http://hz.ehwqpu.com/gtxdvhimot.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.redwolf501.top/gtvhgodfui.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtyihsrhbg.html

[C14] 泛型函数
来源：http://hz.daxiang520.top/gtygnjvqma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtqekablys.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtlnwehxfy.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtfpdjoqqh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtmmnbwdit.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hammf.cn/gtqprqsbbh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tanke756.top/gtzelohlvg.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gtatbkdagt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtqszcubxz.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtmhtphmzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhixingplan.top/gthegmfory.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gttvppjahj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtrqhpvpiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gtzupqvciz.html

Java: // 无解构
来源：http://hz.jinqigufen.top/gtwhgupdrm.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtwinobdil.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gtnykyjklf.html

C#:   var (a, b) = pair;
来源：http://hz.chenjidiqi.icu/gtzblgpqid.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258888.top/gtzzkgicvy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shangyingyoupin.top/gtykmjtcda.html

PHP:  // 无重载
来源：http://hz.xuetiantiany.cn/gtxdnepkki.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtvavbczep.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtmvcwwpac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgufenzy.top/gtjqlvomnv.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtvudslxsu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtufqrmpoi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxinkj.top/gtezslksre.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmirxtucn.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtqsafmsij.html

================================================================================
来源：http://hz.mhx1999.top/gtwhnjbtrp.html

[D01] 创建数组 / 列表
来源：http://hz.zhijiandao.cn/gtabrpbpjz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtxigvyrhy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtpyhalhlt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtkthepuzy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xingfuxueyuan.xyz/gtvplsizty.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigfzy.top/gtysbrxmsc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtaaauobvg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxuanxn.top/gtnwpltwfa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.andypj.xyz/gtvuvjawpf.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtjtcnjxob.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtugfdyspw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtzntujaln.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gthikwpfur.html

TS:   arr.push(4);
来源：http://hz.mhx1999.top/gtfpeqcjpt.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtbfxvrjcy.html

Go:   arr = append(arr, 4)
来源：http://hz.bjfxy.top/gtgsfpfogg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtjlddlptm.html

C#:   list.Add(4);
来源：http://hz.9152youxi.cn/gtydgqcnqj.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gttmyylppf.html

Py:   arr.insert(0, 0)
来源：http://hz.zhixingplan.top/gtwrdpvpqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtnkintzfz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aibaodan.cn/gtmpvwjysq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtjccpxdja.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gtohshpqrs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cucudq.cn/gtnwuypfxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fengsongda.top/gtqgaftlwe.html

C#:   list.Insert(0, 0);
来源：http://hz.pengpengdd.cyou/gtdpdtayqp.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtehgfegfb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuanzhike.top/gtruteuieb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtkxekmwxt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtsldcpyjn.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtmnrcufvr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtujpmmngc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtyqeucyhk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtknufdnht.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtxezsalmz.html

[D05] 访问与修改元素
来源：http://hz.hongshengwenyu.top/gtaammdaxn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtaitstlxq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hysaishi.cn/gtkcyjgddk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtcimrfohp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtjhryqxep.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.iojbl.cn/gtnaiwhzgu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtqxfmtohx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtaycmzanu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gotoacloud.top/gtbayfaiuw.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtbprizuqr.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtntelfjcj.html

PHP:  count($arr);
来源：http://hz.xinyue.icu/gtztzwsylq.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtmzokikbq.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtcnoqzwkj.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtalqvnftl.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gtlruwcaud.html

Ruby: arr.length; arr.size
来源：http://hz.yangfankeji.com/gtaesyqtqg.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtreiwimfz.html

[D07] 切片 / 取子数组
来源：http://hz.sweek.top/gtpicpahec.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtawdbxxvi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtvjaubpwg.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtzbnjxokt.html

TS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtueodzvrx.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangtech.top/gtcqbfigtw.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtudnpyasx.html

Ruby: arr[1, 3]
来源：http://hz.wangdashe.top/gtarvrycnx.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtuprtznvz.html

[D08] 合并两个数组
来源：http://hz.hnqzz.top/gtvskupiru.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtnfhziuvw.html

PHP:  array_merge($a, $b);
来源：http://hz.redwolf501.top/gtjxqlqqsb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtulcyoaaj.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtxdqayyzs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtucwtnyvf.html

Go:   append(a, b...)
来源：http://hz.havefunace.top/gtedpnibnj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhijiandao.cn/gtsyegsfyo.html

C#:   a.Concat(b).ToList()
来源：http://hz.feifeiyinyue.top/gtamdwvdhh.html

[D09] 排序（升序）
来源：http://hz.yanxiufei.cn/gtfisqewtp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtkgbsbjey.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtauaqfzqt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinghuilouyu.cn/gtwrmutfiw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtzaebwttz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hywenlv.cn/gtberjzppm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtvkyrgsaz.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtfemhduph.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtptaakcwi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuxming.cn/gtwmetghgd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gtrxfnicsl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtdirugwqc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtzfvbmhhc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhixingplan.top/gtqfzsurxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.birdmap.top/gtbgctlkxg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.0kj1m.cn/gtctdlhvtl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangdashe.top/gtlpmcndmd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtehhdfoqy.html

[D11] 反转数组
来源：http://hz.cashguo.top/gtkwsordfi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtvimpxzci.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtvjuehnww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.pengpengdd.cyou/gtzbqpftnf.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtsbaljlbi.html

Java: Collections.reverse(list);
来源：http://hz.tian-w.cn/gtspdjhozr.html

Go:   slices.Reverse(arr)
来源：http://hz.cqqwz.cn/gtovbnrwol.html

Ruby: arr.reverse
来源：http://hz.bjfxy.top/gtoshufwxb.html

C#:   list.Reverse();
来源：http://hz.haohaochexian.top/gtktuoromq.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gtrvhrfbxg.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gtbdddrwup.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hongshengwenyu.top/gtfuxbbkqn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtbzzjfovf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtewncoths.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtszbgqiqo.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtvjnvmecd.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtmduiogoh.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtievrzumm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtioncrgmo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtjfmypsku.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gzhubu.top/gtqsfnwnpw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtwqtgdkyx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtsuwgyczi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jianghu66.top/gtamcdrewy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtqbkufvhz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtogrbcmoh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gthuxdhecd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sufxvd.cn/gtmkjhoarv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtljuqnwph.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gthksylvvx.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtzfopzsln.html

TS:   arr.map(x => x * 2)
来源：http://hz.dashuyun.cn/gtouttydgr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtgxhowqqs.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtrlgbwxnp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.bjfxy.top/gtyklrqjhs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj202588.top/gtrmxzbrbu.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtcpbinzvv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtvvwmbcrl.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtyzwtowul.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gthmxawucv.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtopxqhmbc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtxbkpigaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtkftvhopw.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtuykblmib.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtphwjnxqx.html

[D16] 求和与平均值
来源：http://hz.ehwqpu.com/gtayorcnbt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gtmpzxrmcx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgfzy.top/gtiqbhcxps.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtflfycqcp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtwkdtlukd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.svipenyu.cn/gtgrkbzvmj.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gthwgaofng.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sxryk.cn/gtvgthqbex.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtwgxmaxir.html

[D17] 最大值与最小值
来源：http://hz.ppjwa.cn/gtjajzonou.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtzjcpsghz.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtgsbvbbzy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtbnwrljjh.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtdpcgiuet.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtcbdtdhjq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jiagoushi.top/gtycykbiqo.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtvxgdffaa.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtbnavinkn.html

[D18] 扁平化嵌套数组
来源：http://hz.redwolf501.top/gtflhgwnnm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtcwraywqx.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtgmcmxjgc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gtepugofdw.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtwtojtmxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtkflmmelk.html

Go:   // 手写双层循环
来源：http://hz.redwolf501.top/gtfgfqwyyz.html

Ruby: nested.flatten
来源：http://hz.aizwys.cn/gtkhyfknvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gttvgcaqak.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtstmdnnsn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtqezaksax.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhaomingkeji.xyz/gtqcyeokht.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangdashe.top/gtncvnxcbz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtguxitpbk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gtqgvhmbzh.html

Go:   // 手写 map[string][]T
来源：http://hz.zhongyouzk.top/gtblplljql.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.redwolf501.top/gtsueashld.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.bjfxy.top/gtcysotevx.html

[D20] 统计每个元素出现次数
来源：http://hz.tianlin.xyz/gtwpzwcslo.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtvyamxvav.html

PHP:  array_count_values($arr);
来源：http://hz.meibo888.top/gtntpyfqgj.html


<!-- 参考信息 -->