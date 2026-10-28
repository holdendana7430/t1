代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.hfpthk.cn/gtmpepvyql.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtqtcmmdmc.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtzoujqgeu.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gtmvpopkjk.html

Py:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtaxvfhgjd.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtgjpqrxae.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gtcccogvtt.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtczpkdxua.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtzvmbrnfx.html

Go:   return a, b
来源：http://hz.jqgfzy.top/gtkmxpaxzu.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gttxgotrzo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.iojbl.cn/gtwxotcqvf.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtlbyykyjt.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gtpbkjtfud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtumnjgdgv.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gtypqkxikk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtkezwfupb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtramrldlz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gotoacloud.top/gtxpagjfmk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zycfv.cn/gtcewttaux.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtntzfhnoz.html

[C07] 把函数作为参数传入
来源：http://hz.shuidangran.top/gteqjrczcf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.wangdashe.top/gtmvvwdetj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangkeji.top/gtcqjwxidl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtflncvfac.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gtsmlppcfw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtpwtfzcoq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gtxzkomwlc.html

Ruby: arr.map(&:upcase)
来源：http://hz.ivvv.top/gtboefrznj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jianghu66.top/gtyxplvfcy.html

[C08] 闭包
来源：http://hz.hysaishi.cn/gtwohotztz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ivvv.top/gteuiddjxz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtzjkgwrnw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtlzdwktae.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtceikyljo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jiagoushi.top/gtfwxfelgd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtxsjplgxj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.9152youxi.cn/gtpizjsvio.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtufehrmdm.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtuhkwcvpx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.redwolf501.top/gtgbhnqqdv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gtuqtrngnm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtrjcsdnwr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtocbcfwpk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sysykeji.top/gtginsejrq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gthjscmkdz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtnxrludve.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtgodbjdvt.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtajkilrgo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigufen.top/gtwanttdue.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.fzhhl.top/gtiqtgjnkn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gttcqueuol.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gtcrqdsqln.html

Java: 方法内为块级作用域
来源：http://hz.sysykeji.top/gtrnbadzmb.html

Go:   花括号块级作用域
来源：http://hz.redwolf501.top/gtnoohfbjl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fengsongda.top/gttlygyrhh.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gtgqhkrjge.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtsvwasgpu.html

Py:   from module import func
来源：http://hz.shuidangran.top/gtjwklwizt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.c1oappe.top/gtasoqerhm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtavaemrji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtmqvczbev.html

Java: import java.util.List;
来源：http://hz.bjfxy.top/gtsscnvxam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtiscphlap.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aibaodan.cn/gttcxrwvcf.html

C#:   using System.Text;
来源：http://hz.yongpay.top/gtfvjeeiql.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gtzyqcwcmy.html

Py:   (lambda: print("run"))()
来源：http://hz.bjfxy.top/gtazkytxsi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtgecvgddv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtanuxgbpo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtjggluikk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258.top/gtziesfgaz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gtwlpieytw.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuanzx.com/gtgsujudfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jqgfzy.top/gtufxowesa.html

[C13] 类型声明 / 类型注解
来源：http://hz.pycfn.com/gtefvkxfen.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gttnjkebbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtrrgelluj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gthrzalbaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtpkpztuud.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtdvhpmggd.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtnvxyfddq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gaohongyu789.top/gtwmeykfjv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.feifeiyinyue.top/gtuvajmynd.html

[C14] 泛型函数
来源：http://hz.cqqwz.cn/gtbhvakzaj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenzaomai.com/gtkwhxjnzu.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gttumkyefn.html

JS:   // 无泛型
来源：http://hz.feifeiyinyue.top/gtqyhcbyrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtbystndif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtcslinzpt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuxming.cn/gtwhqctunu.html

Ruby: # 无泛型
来源：http://hz.sxryk.cn/gtpwkxarvi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtvtjiiulw.html

[C15] 解构 / 展开参数
来源：http://hz.zhiwuduotai.top/gtedkijhkm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtuxncbbab.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sysykeji.top/gtwbpfqtdj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtegjrvztq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtzsaibyns.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtqxoeyide.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gtvpqgoyqp.html

Ruby: a, b = pair
来源：http://hz.jqgufenzy.top/gtrykqxtlk.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtsiencfwi.html

[C16] 函数 / 方法重载
来源：http://hz.hywenlv.cn/gtzfutqitf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtnekdyzgx.html

PHP:  // 无重载
来源：http://hz.hongshengwenyu.top/gtsbcbtfky.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.52xcode.cn/gttvcxotjg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtaxfirhhc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hywenlv.cn/gtprzhzeau.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtsmsabyyp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.bjfxy.top/gtsytphcfx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gzhubu.top/gtetwvmevj.html

================================================================================
来源：http://hz.aibaodan.cn/gtgiunhmki.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtbwpxqozv.html

================================================================================
来源：http://hz.jyoumei.cn/gtejyrykpv.html

[D01] 创建数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtzpcszlxt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhongyouzk.top/gtkrfvbyle.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtupfhuccr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.316326.xyz/gtnndirvgj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigfzy.top/gtqivrjvmt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtyohrknun.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtwmnnfwfx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtgdicysmr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gttxacvemb.html

[D02] 追加元素到末尾
来源：http://hz.cheryme.top/gtmctujsix.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cqqwz.cn/gtuwcgwvrg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigfzy.top/gtcyyvgpwq.html

JS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtxsthjpij.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtexigappu.html

Java: list.add(4);
来源：http://hz.jyoumei.cn/gtvihgysgg.html

Go:   arr = append(arr, 4)
来源：http://hz.zhixingplan.top/gtmsegbsjl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtcexuoxsg.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtcflaguef.html

[D03] 在指定位置插入元素
来源：http://hz.hysaishi.cn/gtdcofoboi.html

Py:   arr.insert(0, 0)
来源：http://hz.c1oappe.top/gthsssknzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gtugicnflp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fzhhl.top/gtfvatxwrq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pengpengdd.cyou/gtpsnzykea.html

Java: list.add(0, 0);
来源：http://hz.jinghuilouyu.cn/gtrffidmbv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtvpsuordo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.52xcode.cn/gtvqjqnjwb.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtmzethmhw.html

[D04] 删除元素
来源：http://hz.xingfuxueyuan.xyz/gtbzbjussi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtopgsgean.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.kuanghao11.cn/gtbqywieol.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtbsdecvgz.html

TS:   arr.splice(0, 1);
来源：http://hz.xziqi.cn/gtgvczjtms.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtoxybvgfz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ywan-chungtsiang.top/gthwzopdkh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gtcqtyzmvz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxuanxn.top/gtywcghehb.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtqlvfrasb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtxxgexzdd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dianchejie.cn/gtxotcdflt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtzamtjtgq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtinknydzy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhijiandao.cn/gtxjaspvjt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtdikzlcab.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtiolaonbh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtxsfttgex.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtxwuelvfr.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtrzzhjbrx.html

PHP:  count($arr);
来源：http://hz.shanyushiyangtech.top/gtcszzuepr.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtvibdxsdi.html

TS:   arr.length
来源：http://hz.smart0.xyz/gtfxipfrjd.html

Java: list.size();
来源：http://hz.ybcxt.top/gthpotalmw.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtxbsmcnpn.html

Ruby: arr.length; arr.size
来源：http://hz.fzhhl.top/gtoplgeqhq.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtbiqtagzq.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gtmpgvjlvi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gthxlossqn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gttheukcmj.html

JS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtjqswckeu.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtpsswqtam.html

Java: list.subList(1, 4);
来源：http://hz.jinqigfzy.top/gtvnveqhvh.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gtighyzbta.html

Ruby: arr[1, 3]
来源：http://hz.bjfxy.top/gtklbmeznx.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtctzkzqpr.html

[D08] 合并两个数组
来源：http://hz.xingfuxueyuan.xyz/gtmswpbrzo.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gthkyegzla.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtkhrzlwbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cqqwz.cn/gtrcgwlwsu.html

TS:   [...a, ...b];
来源：http://hz.jqgufenzy.top/gtdswycmbi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtdydnhukn.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangtech.top/gtpwihkhav.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtrjmkkxrc.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtkjpaoayj.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtkfftxrdk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtevbpokvb.html

PHP:  sort($arr);
来源：http://hz.xinyue.icu/gtfphkaawr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yonumen.top/gtjpeulagp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtcfgibumg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fengsongda.top/gtimpajrat.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtankkckcw.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtrfuwxrzl.html

C#:   list.Sort();
来源：http://hz.hongshengwenyu.top/gttczrmqbs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tianlin.xyz/gtnxbthmhd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhongyouzk.top/gtjvffasqw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtndxjxdad.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtcxyzzjdo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtdpfqgssz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydjk.org.cn/gtjxwctgze.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.52xcode.cn/gtcnmnoikm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtkukaijab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gtrxlhdwjr.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtjniehdnc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuanzx.com/gtnqqtojum.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtdfgpamjz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtkzeekehw.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gthjkmavvi.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtvxdnywox.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxinkj.top/gtglaaaqlr.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtgmgmsxje.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtoalmpuvr.html

[D12] 查找元素下标
来源：http://hz.zhixingplan.top/gtykenjepk.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtolthynhq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aizwys.cn/gtbliapvpq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtoaucvmau.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtuqkpfuis.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.mhx1999.top/gtqyfxydge.html

Go:   slices.Index(arr, x)
来源：http://hz.tianlin.xyz/gtivzbdivg.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gtzvsqrtmj.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtkpjiufjz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtfwzinhzz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guowangkeji.top/gtoalrsoeg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.smart0.xyz/gtkrnofbqc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtpcygdimf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daria6918.cn/gtrxfcotjw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xinyue.icu/gtwbrorrtd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.snrcjt.cn/gtvafepqzo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fengsongda.top/gtgqqjnkve.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtotdoyyfv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtlcvrovaj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.smart0.xyz/gtoofslazh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.feifeiyinyue.top/gtpigodndl.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtdgnwvnxi.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtjtmnqjrn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hysaishi.cn/gtsxnqdcvo.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtfqtzyncu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nwbrower.top/gtfhgllgrp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtfxywogpc.html

[D15] 去重
来源：http://hz.guowangkeji.top/gtyfmhboaf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtznntbgkx.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtbzyueowk.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtewokiltk.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtghrqpzbr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gtyryubllp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ehwqpu.com/gtkfuorlpi.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gtbjyyvpns.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtvsonbqck.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtxfncmftu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtphcvrhik.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtgezsuhrl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtfhqfjgxe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gttqtxnvlg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtdcjwvqbi.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtbdixfkkb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtkykgdfos.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtghrqqfch.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtdasebvfm.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtrdgiwmof.html

PHP:  max($arr);  min($arr);
来源：http://hz.sysykeji.top/gtpswbalnv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.vqdsnc.cn/gtypkoiqdy.html

TS:   Math.max(...arr);
来源：http://hz.jinghuilouyu.cn/gtoohmbmdm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtfgsxyycn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daxiang520.top/gtxlquxfml.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gtxywjycsh.html

C#:   list.Max();  list.Min()
来源：http://hz.wangdashe.top/gtkqpjlhzi.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtjvhgwfzm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtsijmsgud.html

PHP:  array_merge(...$nested);
来源：http://hz.sufxvd.cn/gtgpcuoffs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtdnqsmfzz.html

TS:   nested.flat();
来源：http://hz.tanke756.top/gtmumcbxnk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.c1oappe.top/gtnolbxddu.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtgeoljozn.html

Ruby: nested.flatten
来源：http://hz.zhixingplan.top/gtfwxheuit.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.feifeiyinyue.top/gtgcsclina.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gtuxirhttu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtzmyiwtfc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtyujtevxz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ivvv.top/gtfebkbqdu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtummeehwe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gtlvnpqkdd.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtioqspicg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jiagoushi.top/gtgladwoks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtvopovhyk.html

[D20] 统计每个元素出现次数
来源：http://hz.vqdsnc.cn/gtrceiptid.html

Py:   Counter(arr)
来源：http://hz.chenjidiqi.icu/gtcparvkpp.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtlvbcytgo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtxcqklgqv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gttzxtlwyz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ybcxt.top/gtoaziuxvj.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtrekcplui.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gteaakmfua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ppjwa.cn/gtenpiwkdt.html

[D21] 判断是否包含某元素
来源：http://hz.cheryme.top/gttegkuaum.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtsjmxdmrh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinghuilouyu.cn/gtuyrtsqby.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtnqhcigfs.html

TS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtimapkcnu.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gtfzidrbah.html


<!-- 参考信息 -->