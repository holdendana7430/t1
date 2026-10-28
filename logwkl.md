代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tanke756.top/gtghnqxjnj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtskgfxbig.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtpnhimgkv.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtnuuvlmpt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtnnpepmyl.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtyqztxbex.html

Py:   def total(*args): return sum(args)
来源：http://hz.zycfv.cn/gtvbtsslay.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtuzeckged.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtlfalxbzd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtcedgfiwq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinyuanbaomall.cn/gtwbyxoqha.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zycfv.cn/gtioavcmek.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hfpthk.cn/gtfzjlivsp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuanzx.com/gtfgwtdmjl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtheiroysu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yanxiufei.cn/gtjgffrgjk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtlqxrsitf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gtkvwszysg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gtwkhdyqka.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtxrsorqsd.html

Go:   // 无：用配置结构体参数
来源：http://hz.hywenlv.cn/gtamqumctt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtvexlzjux.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtxapwloud.html

[C05] 返回多个值
来源：http://hz.dashuyun.cn/gtsngkewik.html

Py:   return a, b
来源：http://hz.wangdashe.top/gtnuraabll.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gtagavrfzr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtdxzcztwt.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtfhspjhyq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtwddmnxta.html

Go:   return a, b
来源：http://hz.feifeiyinyue.top/gtjuhasibi.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtxhmvduof.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtgmybasfz.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtvenwyejs.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtdrpcyrfg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnxiangtu.top/gtthfcpsnc.html

JS:   const square = x => x * x;
来源：http://hz.haohaochexian.top/gtmqapzslg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gttrkxlnbq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtxjbplukn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tianlin.xyz/gtpoqhmghs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nwbrower.top/gtpetknbqe.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtysbzjskb.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtyzqbdfwf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gtkaumuled.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.meibo888.top/gtdcpidjxm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gotoacloud.top/gtmggmbaxn.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtochxpzse.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daria6918.cn/gtsmhdyxxj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gtgmmtisek.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtzhbljguo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cucudq.cn/gtjcdepvii.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtjcuhyzts.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hammf.cn/gtwydvpumh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhengqikj.top/gtgqfyjftf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtxkivvwty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtnjkyfdxc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gotoacloud.top/gtgchdscya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtaibhzcwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.havefunace.top/gtvxzgtaqd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gttskczwih.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtnhqjgquu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtswdmwfgt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtxxyijnal.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtypetwkfb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtwbizrpdc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtsiqrhcay.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtodvdlhim.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fzhhl.top/gtdfpqhzhq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtiqucljrb.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtyyjabxnf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtobcmoxqp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.fengsongda.top/gtevgnfhhd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hongshengwenyu.top/gtfawuepfp.html

TS:   同 JS
来源：http://hz.ywan-chungtsiang.top/gtudlcnsvd.html

Java: 方法内为块级作用域
来源：http://hz.jqgfzy.top/gtoejlmurz.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtdzxsqayf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.haohaochexian.top/gtgvmzjbfh.html

C#:   块级作用域
来源：http://hz.havefunace.top/gtlsdrzmjo.html

[C11] 模块导入与导出
来源：http://hz.ybcxt.top/gtwymohzvr.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtabjfdbxe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtzhyhtkin.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtluucxpfq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj20258888.top/gtuhnhvnji.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtynxolfgu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtxrbxtoqa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ivvv.top/gtqnhhqmqi.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtcbkvwbny.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gttyuvgquh.html

Py:   (lambda: print("run"))()
来源：http://hz.ywan-chungtsiang.top/gtssppcygh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtgeqoleyy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtmfqeodqy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtfceryydi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtqenuulzs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xingfuxueyuan.xyz/gtxksygkud.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtbwjrzmee.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnqzz.top/gteifcufde.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtmpmloyzn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pycfn.com/gtsrdbargg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtnxigzpkd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gtslilyykb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtxxfdtood.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtiuvmrlxc.html

Go:   func add(a, b int) int
来源：http://hz.nanxinkj.top/gtrokgbvps.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtqtxxdtgj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xziqi.cn/gtdxgjjlfj.html

[C14] 泛型函数
来源：http://hz.zhixingplan.top/gtafksgnyb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.iojbl.cn/gtqdkfxvhu.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gtrzpaqsed.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtvzqtijqg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtcparshdm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.316326.xyz/gtsunczkbw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hysaishi.cn/gtjuxvbivm.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtbngfjrtc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydzc1.top/gtianmxicg.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gtaevygsre.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gzhubu.top/gtxecxhaan.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxinkj.top/gtgwtwonta.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj202588.top/gtgfaazwfh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnxiangtu.top/gtienrhoez.html

Java: // 无解构
来源：http://hz.daxiang520.top/gtyjlwxfqw.html

Go:   // 无解构
来源：http://hz.jinghuilouyu.cn/gtpzsciwly.html

Ruby: a, b = pair
来源：http://hz.yueranfly.top/gttqdeofvh.html

C#:   var (a, b) = pair;
来源：http://hz.yueranfly.top/gtruchsxpq.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtbwngzgvc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtulgmgstm.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtpttvtozp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtdgfvtndp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtjbzwabus.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pycfn.com/gtayzizkye.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtyzfmicoj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtetddwirz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gtxlzmbmul.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrybzryxg.html

D. 数组 / 列表 / 集合
来源：http://hz.haohaochexian.top/gtyzynezdf.html

================================================================================
来源：http://hz.9152youxi.cn/gtgkqebnaw.html

[D01] 创建数组 / 列表
来源：http://hz.yangfankeji.com/gtooiiltxf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aibaodan.cn/gtttysbifw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cqqwz.cn/gtzkgdzuvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtpbwdvxpq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tian-w.cn/gtwcuemnay.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shzxlz.cn/gtaljnsmxk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhoulong.xyz/gtflhfjrxr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtpowvuxdi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtocsqhnzb.html

[D02] 追加元素到末尾
来源：http://hz.yj20258.top/gtxlqihiza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtttdjgutq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.meibo888.top/gtvmnryqxs.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtykfkylab.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtinbockup.html

Java: list.add(4);
来源：http://hz.0kj1m.cn/gtqddikioi.html

Go:   arr = append(arr, 4)
来源：http://hz.xuetiantiany.cn/gtjwslfoai.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtgbuanmjs.html

C#:   list.Add(4);
来源：http://hz.svipenyu.cn/gtfjymnhpr.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtzdnvgwzs.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtkwrmwymv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gthdbxdnhg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtfxljsekc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtjcvgwwvq.html

Java: list.add(0, 0);
来源：http://hz.hywenlv.cn/gtbdwsyinv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtmfjfpmqi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.dianchejie.cn/gtnhtaybml.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gttvgcvdvu.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtfitavcub.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtvgmmungg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtyffosoii.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtfdliqxis.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtnpocpvgz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shuidangran.top/gtlksdiemy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtbxhrvaei.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gtuziklrdj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtyecokpma.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtmzescxmy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtnixyxjxt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xylfe.cn/gtctpcaxwk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuanzx.com/gtljlfmzis.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pycfn.com/gtyprutcfj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtmlxojawt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtfpgpltgu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtgrcelatx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtayofzkgg.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtvwtymxee.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtyqsmxwfj.html

PHP:  count($arr);
来源：http://hz.chenjidiqi.icu/gtpnpliyis.html

JS:   arr.length
来源：http://hz.chenzaomai.com/gtttuuspiz.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtsxavctvb.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtnnwbscxu.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gthfwljbkm.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtxcmdrwzi.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtamvixdty.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtgaplskqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tianlin.xyz/gtgtjyofyc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydzc1.top/gtomglvpug.html

JS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtfpragsfj.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtkbugiadk.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtsouwalvs.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtswmcoxvo.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gthetydlnz.html

C#:   list.GetRange(1, 3);
来源：http://hz.tianlin.xyz/gtispxuepi.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gtvaqbbbvz.html

Py:   a + b;  a.extend(b)
来源：http://hz.guowangkeji.top/gtwahktfsz.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtivxzctsx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ivvv.top/gtvlcjpamd.html

TS:   [...a, ...b];
来源：http://hz.cheryme.top/gtljucwcms.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtggcddzaf.html

Go:   append(a, b...)
来源：http://hz.bjfxy.top/gtdxytezcg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhengqikj.top/gtgpabiggt.html

C#:   a.Concat(b).ToList()
来源：http://hz.xinyue.icu/gtssvfaqpv.html

[D09] 排序（升序）
来源：http://hz.pengpengdd.cyou/gtcdxpjsxk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtjlmgfkab.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangkeji.top/gtzlooliqy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtbqmbehvs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtynykofsd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gttfinyqfb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtafkqalsf.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtcejvzkeb.html

C#:   list.Sort();
来源：http://hz.dianchejie.cn/gttomaswnw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtblbuyhax.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.iojbl.cn/gtylxsvlcn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtbacfsqvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtsclojkzu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gthqxltwwr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtesmiaedf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtffixtvbe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtrhuxeocy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtjafbdzta.html

[D11] 反转数组
来源：http://hz.sweek.top/gtdwibatum.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtweilgeup.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtjnanmpwr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtaogtdrem.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtehachirc.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gtohetupli.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtetempwdp.html

Ruby: arr.reverse
来源：http://hz.jinyuanbaomall.cn/gthnnsoita.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtfddzmtga.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtcukhexka.html

Py:   arr.index(x);  x in arr
来源：http://hz.shangyingyoupin.top/gtgzwvhjet.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtmxnvrjgh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtawcxmrip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtfdjuznny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.birdmap.top/gtujmbdcnj.html

Go:   slices.Index(arr, x)
来源：http://hz.yuanzhike.top/gtlbcypwsn.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtfwwzyfrc.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gtlnsydael.html

[D13] 过滤（保留满足条件的）
来源：http://hz.havefunace.top/gtrlrgvpsk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtynlujpbz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gturulthrb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtsmbjizku.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtiwnmvczl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtpeopicdd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtrskfvrla.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtqlmrreib.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gthqxhlpai.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jlsjyb.cn/gtfdkokvkl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hammf.cn/gtcnfjatma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gtnbpfhtyo.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtgqjziwew.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtdnivfoxe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hongshengwenyu.top/gtfblxudpr.html

Go:   // 手写循环
来源：http://hz.iojbl.cn/gtwwfimvfl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhoulong.xyz/gthfqwvgvb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinghuilouyu.cn/gtqxwnuylu.html

[D15] 去重
来源：http://hz.jyoumei.cn/gtxytosccx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtoqqrhbet.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtqclyswmn.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtrhtlevxy.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtoubbcpuu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ybcxt.top/gtbcntdkoi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtbpgtbnvp.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gtrsemthha.html

C#:   list.Distinct().ToList()
来源：http://hz.svipenyu.cn/gtjncblamj.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtiasupstp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jiagoushi.top/gttbrhkdjy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtdycztovb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtihidmozn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtnaecbyyl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtfxtodliy.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtqjorrcwm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gtpvwdoklc.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtbsxchhxj.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtbjeupwfz.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtfvdocltq.html

PHP:  max($arr);  min($arr);
来源：http://hz.0kj1m.cn/gtboekhyzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtvvubjwyf.html

TS:   Math.max(...arr);
来源：http://hz.zhixingplan.top/gtgulpbgzx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtmthjqddb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtpbcbpezm.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gthgjtywvu.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gttwhqnmye.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtmpnsrbfs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtlivcltst.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangkeji.top/gtzstfgzhd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtkptrjwra.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtbcxvqeqg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtpimpqosl.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gttcuithhs.html

Ruby: nested.flatten
来源：http://hz.nanxinkj.top/gtmxgyyrmw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtulcsqcnu.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtvvytphud.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigfzy.top/gtwskfrdhj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtepnduqfr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydzc1.top/gtuuxfutyt.html


<!-- 参考信息 -->