代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtahfvxyqn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gttyiyyirm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinyuanbaomall.cn/gttfenokfb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258888.top/gtayrjxoyh.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtzctkxzra.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtntqpjdvg.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtxxxmhfbm.html

[C05] 返回多个值
来源：http://hz.ppjwa.cn/gtketygnsv.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtoujugqih.html

PHP:  return [$a, $b];
来源：http://hz.9152youxi.cn/gtqrobfaii.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hysaishi.cn/gtahgpjinu.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtenzupzpr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtfzdihiai.html

Go:   return a, b
来源：http://hz.shangyingyoupin.top/gtkmvckkbb.html

Ruby: return a, b
来源：http://hz.zhixingplan.top/gtbdlyzfih.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.316326.xyz/gthgdubcbz.html

[C06] 匿名函数 / lambda
来源：http://hz.wangshuangyany.cn/gtatpvyzwj.html

Py:   square = lambda x: x * x
来源：http://hz.hammf.cn/gtxgcsbdza.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xylfe.cn/gtekzfarzl.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtszpqnqri.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shuidangran.top/gtgewryxdn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtbdbvfefs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ivvv.top/gtukkafygs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtsbngmexn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtbhbafcik.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtryvwtvxf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.9152youxi.cn/gtoayyespb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhoulong.xyz/gtecwicumy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shangyingyoupin.top/gtelickvxr.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtdaooukbk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.52xcode.cn/gtgslkatez.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinghuilouyu.cn/gtncdkkeej.html

Ruby: arr.map(&:upcase)
来源：http://hz.feifeiyinyue.top/gtgvvkycgl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtptfuahkb.html

[C08] 闭包
来源：http://hz.52xcode.cn/gtyzrehihx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtfjezomuk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xinyue.icu/gtscotungt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtifwpauuf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtxpmjdjsm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenlongwang.top/gtzhqcpafv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtrrvejykq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtlrheohkp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtffahgkuw.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtpftlxrtt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtyoyzsygd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtahszfkwy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtxjnpxuoj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtmhmvhozz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenzaomai.com/gtmutjboha.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yuxming.cn/gtohrduqtp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtiyovsuwv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gttbxywumy.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gthkkwqkwa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtqstfdhvv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.meibo888.top/gtwhqtqdli.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aibaodan.cn/gtgbzthdnq.html

TS:   同 JS
来源：http://hz.yuxming.cn/gtxqneagub.html

Java: 方法内为块级作用域
来源：http://hz.c1oappe.top/gtegzttgqe.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtfwsczxoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guowangkeji.top/gtnghbcbkc.html

C#:   块级作用域
来源：http://hz.nwbrower.top/gtuzmgcokf.html

[C11] 模块导入与导出
来源：http://hz.jqgfzy.top/gthujikdek.html

Py:   from module import func
来源：http://hz.yvedp.cn/gtrfeuyzmz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtsqbvpoyh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xziqi.cn/gtfgawoxux.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgfzy.top/gtbjnriztj.html

Java: import java.util.List;
来源：http://hz.svipenyu.cn/gtcurqctrh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cheryme.top/gtxywjxjam.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtoygeseqi.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtmanggghr.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtgnsueggy.html

Py:   (lambda: print("run"))()
来源：http://hz.hfpthk.cn/gtwsebtyen.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtmnyouetb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtnjuhdkje.html

TS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtobklcbbx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gtdhyetmjq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gtrnvwpqtc.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnxiangtu.top/gtrifvetee.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtxdmmknaj.html

[C13] 类型声明 / 类型注解
来源：http://hz.ppjwa.cn/gtmpamfehy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtaqcvihbt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtbpedgvtf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtocneouyw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gttoitpvja.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtizfarxma.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gttxtianzg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gtiqyhzcqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhongyouzk.top/gtezetajer.html

[C14] 泛型函数
来源：http://hz.yueranfly.top/gtyytsdkit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtcfccseww.html

PHP:  // 无泛型
来源：http://hz.yvedp.cn/gtcugiadba.html

JS:   // 无泛型
来源：http://hz.xziqi.cn/gtenzzbegn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtmczxchkz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtxvxwlpno.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtcimvmbuu.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtchwkogkv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dianchejie.cn/gtqtyofcue.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtwhsltzrp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinyuanbaomall.cn/gtxmqfjzxt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtoksuvrdm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtbiopmrjb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cheryme.top/gtfcszzcro.html

Java: // 无解构
来源：http://hz.yuxming.cn/gtobvjhryv.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtnogkejyt.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtjsoqbzsg.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtlnoplbav.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtkidahoad.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.haohaochexian.top/gtdvccwdwc.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtbcrvbltc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cqqwz.cn/gthcbbgres.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtvfhdftff.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtxuknzigj.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gthrlmcwdx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aizwys.cn/gtdxsbcvnn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtbbsnydsd.html

================================================================================
来源：http://hz.zhengqikj.top/gtlgkaatos.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtxhjcqyck.html

================================================================================
来源：http://hz.jiagoushi.top/gtihngywal.html

[D01] 创建数组 / 列表
来源：http://hz.c1oappe.top/gtyyqyhdqw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtruwpiivx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtpqkourzf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtkczqbztd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gtvoavklov.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yueranfly.top/gtfjzhajdp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtdvtvuuis.html

Ruby: arr = [1, 2, 3]
来源：http://hz.meibo888.top/gtijlelnlq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangdashe.top/gtgvosvyqw.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtrllipflo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.tian-w.cn/gtgvginwei.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtlarmgaih.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtswfdnmjy.html

TS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtmvrmpzms.html

Java: list.add(4);
来源：http://hz.zycfv.cn/gtwzkbdlkl.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtzviybrln.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fengsongda.top/gtlgdgykfi.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtjpmdegfy.html

[D03] 在指定位置插入元素
来源：http://hz.redwolf501.top/gtiewosajj.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxuanxn.top/gthviavuqz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtgkiilnlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ybcxt.top/gtscdoermv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtvwzcmnzt.html

Java: list.add(0, 0);
来源：http://hz.haohaochexian.top/gtfxvcdxiy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gaohongyu789.top/gtbwimrjpv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.redwolf501.top/gtshmpmuqq.html

C#:   list.Insert(0, 0);
来源：http://hz.aibaodan.cn/gtmmimgqtx.html

[D04] 删除元素
来源：http://hz.havefunace.top/gttmwoprez.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.snrcjt.cn/gtnmgduqvr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtgkzcekgv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtfmcbvzhf.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtmgawhrce.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgufenzy.top/gtbgdtsnnl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangshuangyany.cn/gtudlawfvz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yueranfly.top/gtazzurxqa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xylfe.cn/gtoyivsptl.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtpwpuuzgp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtvaktaomq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtbcxsmtzn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtbpyrdgvx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shangyingyoupin.top/gtxyihqrtl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydzc1.top/gtddlcjsul.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj202588.top/gtcutimasc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydzc1.top/gtmwdyqcfw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtjhsfmfcw.html

[D06] 数组长度
来源：http://hz.hnxiangtu.top/gthgttxxwj.html

Py:   len(arr)
来源：http://hz.andypj.xyz/gtxlvqrnvz.html

PHP:  count($arr);
来源：http://hz.zhixingplan.top/gtyifjsuxz.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtxwalygad.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtqaiceaty.html

Java: list.size();
来源：http://hz.yj20258.top/gtufgdmzeh.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtpwukfhbg.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtjdpahzlk.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtnlkawdjj.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtsexmuwcn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cqqwz.cn/gtehuokwpe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtkyrkdqyq.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtrrkdbgbs.html

TS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtageuklda.html

Java: list.subList(1, 4);
来源：http://hz.yangfankeji.com/gtdyvzkdem.html

Go:   arr[1:4]
来源：http://hz.shangyingyoupin.top/gtpvrojjjk.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gthwqkxgep.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gthrlhczet.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtfyaqfrek.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtshhoudhm.html

PHP:  array_merge($a, $b);
来源：http://hz.yanxiufei.cn/gtjmotbemx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jlsjyb.cn/gtaeovueor.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtiadxzxol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.9152youxi.cn/gtfrfimqww.html

Go:   append(a, b...)
来源：http://hz.sweek.top/gtaxssogsf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gthrctydqf.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtmjdnpnoa.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtkkqiansw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtdgojqfsf.html

PHP:  sort($arr);
来源：http://hz.yj20258.top/gtaasasvql.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtnyeaorvc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtmixsxwzz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtwebzrjkt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtecbdbikl.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtmgykjjcz.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtjbsmlrma.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtdfnmfuar.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zdqjudy.top/gtylkehdbs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sxryk.cn/gtjtoyrogr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gttstxawta.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtqlutnvvv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtlafrldqe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhongyouzk.top/gtindkewao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ywan-chungtsiang.top/gtjikpozir.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtmskzirfw.html

[D11] 反转数组
来源：http://hz.ivvv.top/gtyzfycfrp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtqhwowldn.html

PHP:  array_reverse($arr);
来源：http://hz.guowangkeji.top/gtbabhqeqt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtkgxqhvgh.html

TS:   [...arr].reverse();
来源：http://hz.meibo888.top/gtcovjfbmg.html

Java: Collections.reverse(list);
来源：http://hz.sufxvd.cn/gtipmnybke.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtokcvxosp.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtxyjcafve.html

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtylbhsjve.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtwsrrcjag.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtdgvmhvla.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangshuangyany.cn/gtrrkchbky.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtcsbhduki.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtdsdtwlmg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtxefftaqo.html

Go:   slices.Index(arr, x)
来源：http://hz.gzhubu.top/gtfoobjgpk.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtqhamfklh.html

C#:   list.IndexOf(x);
来源：http://hz.zycfv.cn/gtvuymyqeg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtrwujjzcv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gtgiuiziky.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.iojbl.cn/gttsreqdkm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtorjgjhub.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtrsptgozw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtndnkibpt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtsvapbkpq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gtcsnmypba.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangshuangyany.cn/gtsavsdtfq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtevicrlmy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtelsxvadr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.0kj1m.cn/gtqhixybey.html

JS:   arr.map(x => x * 2)
来源：http://hz.pengpengdd.cyou/gtievykkxs.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gttcecnzhj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtrykgtomc.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtwvmjupcn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtduftjawi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.c1oappe.top/gtzrwvcncb.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtzjfhmrxy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtzhelqhqs.html

PHP:  array_unique($arr);
来源：http://hz.xingfuxueyuan.xyz/gtujmaweaz.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtanpxmsuo.html

TS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtiyxsuiyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nwbrower.top/gtzugainoc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtinxjykia.html

Ruby: arr.uniq
来源：http://hz.tanke756.top/gtckexygil.html

C#:   list.Distinct().ToList()
来源：http://hz.hongshengwenyu.top/gtintzjuzr.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtwbpzrepy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtihpmgqoq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtexplnjzn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtysevnwzq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gthzdbcfzq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.vqdsnc.cn/gtjmqidlgk.html

Go:   // 手写循环累加
来源：http://hz.jinqigfzy.top/gtarnugovx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtixorgrrv.html

C#:   list.Sum();  list.Average()
来源：http://hz.pengpengdd.cyou/gtdwnyrzvp.html

[D17] 最大值与最小值
来源：http://hz.nanxuanxn.top/gtfmeitjvp.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtbkqvpaph.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtvvenyuqc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtrllzyemh.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtladcrhpc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gtuvcpftqm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sufxvd.cn/gtzrzdmkvj.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtyejzchtz.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtwcvoxysj.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtuelbeuuz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shzxlz.cn/gtgawhncci.html

PHP:  array_merge(...$nested);
来源：http://hz.gogol.net.cn/gtncrhbhyd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtzdkrwmit.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtxjjotnbe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtifacvwzh.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtfflsvevx.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtzdyvqafm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtjialhwim.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtvqlqdnrh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtbhvutssr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydzc1.top/gtglyravdb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtmoudtdbd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gttyxsyalf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gterhozmmq.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtbakjzqxt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gtdzspfscq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnqzz.top/gtebtiwnts.html

[D20] 统计每个元素出现次数
来源：http://hz.dianchejie.cn/gticthaohh.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gtvspwagsb.html

PHP:  array_count_values($arr);
来源：http://hz.havefunace.top/gtevozbvej.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtzlmsukvb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtimxamboo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhixingplan.top/gtruhvnjef.html

Go:   // 手写 map[T]int
来源：http://hz.xingfuxueyuan.xyz/gtjzdeejtw.html

Ruby: arr.tally
来源：http://hz.hongshengwenyu.top/gtvxursena.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtsisfksgo.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtvlaaqtjj.html

Py:   x in arr
来源：http://hz.yonumen.top/gtjcpmyyso.html


<!-- 参考信息 -->