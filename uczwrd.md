代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.ydzc1.top/gtkjiepdpw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtpauigmxe.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtjupmucgh.html

[C05] 返回多个值
来源：http://hz.zhoulong.xyz/gtehgyliqn.html

Py:   return a, b
来源：http://hz.tianlin.xyz/gtehupmitp.html

PHP:  return [$a, $b];
来源：http://hz.zhijiandao.cn/gthutemull.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtiphiekqd.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtvnlqpdhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtuxoxlqok.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtjdccpjtt.html

Ruby: return a, b
来源：http://hz.daria6918.cn/gtodztqefo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangshuangyany.cn/gtfozvwlcp.html

[C06] 匿名函数 / lambda
来源：http://hz.hongshengwenyu.top/gtnfjemuuk.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtbojqnnoc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yanxiufei.cn/gtyawoxcmb.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtpttmxona.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtwmphuxib.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cashguo.top/gtilqgflgw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aibaodan.cn/gtkxpeatnw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.iojbl.cn/gtxbfxqtfs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ppjwa.cn/gtqptzniyq.html

[C07] 把函数作为参数传入
来源：http://hz.dashuyun.cn/gtokkqoxsn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gttpvobvux.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pengpengdd.cyou/gtciqzuasp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtitjepqch.html

TS:   arr.map(String)
来源：http://hz.xingfuxueyuan.xyz/gtrjnqqaie.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinghuilouyu.cn/gtusunazwk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.birdmap.top/gtgsktrsbs.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtsluuqoqf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fzhhl.top/gtfxgzaelx.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gthbbignyb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.snrcjt.cn/gtaefohpfr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxuanxn.top/gtnvliljcj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtgihxithv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gttzrrnvka.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jianghu66.top/gtodwdztao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtzczwgzab.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hnxiangtu.top/gtagvtkdqd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtpyclffpb.html

[C09] 递归
来源：http://hz.shuidangran.top/gthdwokibs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtobmfovtp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtetrybbpe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtezvdbehh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gttpaouqaa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtxguscucr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.snrcjt.cn/gtahmmqkfw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jyoumei.cn/gtkykxhvuu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtgycniexa.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtdnemttkf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtjziutbsh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtaxbihqgm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.c1oappe.top/gttswihlwy.html

TS:   同 JS
来源：http://hz.aizwys.cn/gtolwersor.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtttpqockb.html

Go:   花括号块级作用域
来源：http://hz.zhijiandao.cn/gttytlsogn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sysykeji.top/gtassulyaw.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtmtgheaus.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtxyfhcnzt.html

Py:   from module import func
来源：http://hz.shanyushiyangkeji.top/gtwsrcmupe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtpooksqxk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.9152youxi.cn/gtbphcfiwd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gthuwrsgaq.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtkqycwnuc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cheryme.top/gtpicjlmuf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtfqjgijvg.html

C#:   using System.Text;
来源：http://hz.jinyuanbaomall.cn/gtlwzmufuc.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuxming.cn/gtrnytywxq.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigfzy.top/gtzrvmshaf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtnbmosalf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtxblxbfii.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangshuangyany.cn/gtvajeswap.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cheryme.top/gtcpwbvaqh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigfzy.top/gtjsrzdvnm.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gthmuwgjaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gttrzeqgzw.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtwkeiuuvl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daxiang520.top/gteiriotpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtnqjzwtkx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shzxlz.cn/gteudeucpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtcuvxkmxo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtltfphysu.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtmisdajqm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yongpay.top/gtkqdehcrc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtpivxglor.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtmxzpqglx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtcbgkkhmk.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtovkzgjdr.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtwrnshtji.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtdfvewhba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtiymrjrfv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinqigufen.top/gttksjaujd.html

Ruby: # 无泛型
来源：http://hz.kuanghao11.cn/gtczzlmciu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yongpay.top/gtwkuknrqf.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtmsfhlnaq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtvftbctbt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtrlstztol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gttdwtwsqx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtmuivmfhu.html

Java: // 无解构
来源：http://hz.ydjk.org.cn/gtakrwemuv.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtqaeacwfv.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gtjbbanmvp.html

C#:   var (a, b) = pair;
来源：http://hz.chenzaomai.com/gtcpzhfjrf.html

[C16] 函数 / 方法重载
来源：http://hz.shzxlz.cn/gtqlrfcwfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.meibo888.top/gtjfzwutkf.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtliuhwonw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gtqdkbroyi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtkhjilgkz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yongpay.top/gthxzjxbds.html

Go:   // 无重载：用不同函数名
来源：http://hz.jyoumei.cn/gthffxcltl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtfiazeryg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tianlin.xyz/gthkojblzw.html

================================================================================
来源：http://hz.guannengcc.top/gtswbjihvo.html

D. 数组 / 列表 / 集合
来源：http://hz.ywan-chungtsiang.top/gtsqvcvoux.html

================================================================================
来源：http://hz.52xcode.cn/gtfbrwacrd.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtmjbaspuf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuxming.cn/gtlilaqdwp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zycfv.cn/gtimyxqveb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtygqetano.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.haohaochexian.top/gtaceronfc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sysykeji.top/gtfkgrdibn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigufen.top/gtskvtlbyn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shuidangran.top/gtyoqieuij.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.0kj1m.cn/gtfiomnqps.html

[D02] 追加元素到末尾
来源：http://hz.sweek.top/gtorsskfob.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ywan-chungtsiang.top/gtzcvgfmvg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gttzuausrd.html

JS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtnhtbvegc.html

TS:   arr.push(4);
来源：http://hz.tanke756.top/gtozgjzvwd.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtcrhxrhlz.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtwqknihgc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtizkvwtkn.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtvmwmnonb.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gttjryhegf.html

Py:   arr.insert(0, 0)
来源：http://hz.pycfn.com/gtkirbkguv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tanke756.top/gtufhnotob.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtptwxwbbe.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenlongwang.top/gtokvpppgf.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangtech.top/gtoogatsru.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtjzdnxyqp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jiagoushi.top/gtdbdqyfei.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gttrrenmzg.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtbatbwiwv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtqvoajwcv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fengsongda.top/gtuatbniwb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtjvjpdcws.html

TS:   arr.splice(0, 1);
来源：http://hz.snrcjt.cn/gtnpylexkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cucudq.cn/gtqxctxmng.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gtbjpkjqlq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gthhoavgtv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtxyufytwo.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtuffjffzd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtxzglpvpp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtfihgsyhx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtxndydhfa.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnxiangtu.top/gtgfgtrvov.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gaohongyu789.top/gtyaggjdrb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtybxnzblg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtkdmvrksd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.feifeiyinyue.top/gtfcgbatab.html

[D06] 数组长度
来源：http://hz.zycfv.cn/gtxsehwucu.html

Py:   len(arr)
来源：http://hz.iojbl.cn/gtonjvkmxp.html

PHP:  count($arr);
来源：http://hz.guowangkeji.top/gtlxkmvxhu.html

JS:   arr.length
来源：http://hz.yonumen.top/gtdidaxgid.html

TS:   arr.length
来源：http://hz.guowangkeji.top/gtjkihadgp.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtqnequgon.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gttnmrezfc.html

Ruby: arr.length; arr.size
来源：http://hz.hongshengwenyu.top/gtcomttpig.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtuvnrbutk.html

[D07] 切片 / 取子数组
来源：http://hz.jlsjyb.cn/gtrkmfzeqg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtpajcxjki.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtnqhjgdkx.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtshnwqsfq.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtmdldhqma.html

Java: list.subList(1, 4);
来源：http://hz.xinyue.icu/gtergzgyvg.html

Go:   arr[1:4]
来源：http://hz.cqqwz.cn/gtzzdbuycs.html

Ruby: arr[1, 3]
来源：http://hz.xylfe.cn/gtgkmqkidd.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtyhwzdrgp.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtfgfenrdn.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gthtyditcm.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtdfvptlwr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigufen.top/gtfukyaugd.html

TS:   [...a, ...b];
来源：http://hz.zhoulong.xyz/gtqgrlugow.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtmjeceelq.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gtamgwgrxv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gtdieznlln.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gtytilngos.html

[D09] 排序（升序）
来源：http://hz.yuxming.cn/gtuobrcexw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtxqxldime.html

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtamzidqrh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtpwtyfhmw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtyhfahcsq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.andypj.xyz/gtnjzdgpwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtpqlcynot.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtkvjwvygt.html

C#:   list.Sort();
来源：http://hz.yonumen.top/gtwixzfyud.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigfzy.top/gtkosrobjm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinqigufen.top/gtkscyxhzr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtdqswjdac.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtwiuehrgr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtmukzgcvs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hywenlv.cn/gtotsaklrf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.quarkkingdee.top/gtvbmizvtw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.mhx1999.top/gtypwoptkr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtegvsqejd.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtdgjontrf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtjmqwacjj.html

PHP:  array_reverse($arr);
来源：http://hz.aibaodan.cn/gtucftuezx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtisaafmuq.html

TS:   [...arr].reverse();
来源：http://hz.zhiwuduotai.top/gttjdvohys.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtnbxjrlpa.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtudaqfmjn.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtknmuplmf.html

C#:   list.Reverse();
来源：http://hz.hfpthk.cn/gttnchdcpe.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtgodqvswo.html

Py:   arr.index(x);  x in arr
来源：http://hz.bjfxy.top/gtwimfnxjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.c1oappe.top/gtegamwfsy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtchmbrvym.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtbywbbmju.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtvmmrtjlv.html

Go:   slices.Index(arr, x)
来源：http://hz.ybcxt.top/gtagltdjkv.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtjtpjuciw.html

C#:   list.IndexOf(x);
来源：http://hz.dianchejie.cn/gttubhyzxm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtyrdapezh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gthhnkitsm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtuyfxttxu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtkbcvsnuq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtqlwbfnvj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtmnwpetan.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gtngelbeig.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xziqi.cn/gtlbrchckz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhixingplan.top/gtwsskvwuz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sysykeji.top/gtxjzoxkce.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtgmuzwzwm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgfzy.top/gteiwikkyz.html

JS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtjtsmncif.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtkdjzwwcb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtskuithrh.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtydazdcwe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hammf.cn/gtelcyukgv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gthlugtazp.html

[D15] 去重
来源：http://hz.wangdashe.top/gtxxgcwejm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtpcnncodu.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtjzbocdut.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtrpvrpkxc.html

TS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtdxlnwkep.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtoitghkek.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xylfe.cn/gtscsvlhms.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gtrqojyrgg.html

C#:   list.Distinct().ToList()
来源：http://hz.zhiwuduotai.top/gtusqmxncm.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtveenrkfy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtisumkgtj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtkohpeopb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtqzzwwhpd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gtesicbzcz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtjosqwuur.html

Go:   // 手写循环累加
来源：http://hz.zdqjudy.top/gtglwvhidh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtrrkwnugg.html

C#:   list.Sum();  list.Average()
来源：http://hz.ivvv.top/gtojieoxxj.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtjtghhapg.html

Py:   max(arr);  min(arr)
来源：http://hz.zdqjudy.top/gtkryqpqaj.html

PHP:  max($arr);  min($arr);
来源：http://hz.aibaodan.cn/gtkxwwcsli.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gtralweyof.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gttxdhqpip.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gttttorysu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtvingfisl.html

Ruby: arr.max;  arr.min
来源：http://hz.ybcxt.top/gtpukqnhti.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtqofcpymg.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtvtydmhim.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.snrcjt.cn/gtrhbknjui.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtlwaaclsq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuxming.cn/gtoopeabmu.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtgdgqjsbx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yanxiufei.cn/gtahwofysl.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gtjdssytyj.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtsfuaexsw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.snrcjt.cn/gtnqxbatto.html

[D19] 按字段分组
来源：http://hz.yj20258.top/gtynvxdoyu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtbrlmvlct.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtchagdbgp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhongyouzk.top/gtatqeszgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtkibvdxkc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtkiuvdywo.html

Go:   // 手写 map[string][]T
来源：http://hz.snrcjt.cn/gtcnvqdnhb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.snrcjt.cn/gtfvomnpyu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtiylpmcen.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtlhdywqww.html

Py:   Counter(arr)
来源：http://hz.jqgfzy.top/gtxsviimmu.html

PHP:  array_count_values($arr);
来源：http://hz.vqdsnc.cn/gtwojmfgmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtjvczflot.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtrtortiai.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gthoggktqo.html

Go:   // 手写 map[T]int
来源：http://hz.cqqwz.cn/gtolrixzbu.html

Ruby: arr.tally
来源：http://hz.yanxiufei.cn/gtdfzphhol.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtcwydyymc.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtkaygmfel.html

Py:   x in arr
来源：http://hz.gotoacloud.top/gtqsdvonbi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtsvcppqbi.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtzfekuela.html

TS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtwagoynfp.html

Java: list.contains(x)
来源：http://hz.dashuyun.cn/gtadyeifrx.html


<!-- 参考信息 -->