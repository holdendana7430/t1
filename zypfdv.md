代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtcjakfekq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtmwhtvron.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gtcafqgyye.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgfzy.top/gtnetrpoby.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gtdjjmlzid.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtqclxbxkt.html

C#:   f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gtqpcvnwuq.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gtqdwhsepe.html

Py:   return a, b
来源：http://hz.chenzaomai.com/gtilzuzeuq.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtclljlzxe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtxtanfwzi.html

TS:   return { a, b };
来源：http://hz.vqdsnc.cn/gtabpazcyh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.316326.xyz/gtkamvkaeq.html

Go:   return a, b
来源：http://hz.xinyue.icu/gthigonfjj.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtiaxdatbs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ehwqpu.com/gtfyvhcbkj.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtqueywpud.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtlztqquql.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gthsuuohnk.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtwtgjezsn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pycfn.com/gtqtfuwphu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj202588.top/gtlfbjhflv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yonumen.top/gtabjuazdp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fzhhl.top/gtdxqbnxsd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenzaomai.com/gtynxcqlpy.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtcsefprbj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtahavqboi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuxming.cn/gtcynnkcfk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtmhwjytda.html

TS:   arr.map(String)
来源：http://hz.xuanzx.com/gtnielcxya.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj20258.top/gtsfcfzlsr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtxafmesue.html

Ruby: arr.map(&:upcase)
来源：http://hz.guowangkeji.top/gtwrosvwpc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxinkj.top/gtlgubmwrj.html

[C08] 闭包
来源：http://hz.fengsongda.top/gtcpkpetcl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtcslkrysh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ppjwa.cn/gtrcelffoj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtvorynyqh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangkeji.top/gtafbblttj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hfpthk.cn/gtyjowdeoc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aizwys.cn/gtmokvxujb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sweek.top/gtbdwuzuwo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtththjqkq.html

[C09] 递归
来源：http://hz.shangyingyoupin.top/gtsxewrvvy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtwqyfsgro.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtvevrdnbx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.meibo888.top/gtktjytlks.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtzoppxyxa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shuidangran.top/gtuulskjmo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gtjpwhdbek.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258.top/gtwjdpilas.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yangfankeji.com/gtwqphrqsp.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtuyvyjfcc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuxming.cn/gttescypzk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtkmoavqjw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.birdmap.top/gtuzbeqtbe.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtewguxkcj.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtotpzzbgl.html

Go:   花括号块级作用域
来源：http://hz.bjfxy.top/gthrrjlrfd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtbbhstwyj.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtepmyiqrk.html

[C11] 模块导入与导出
来源：http://hz.xylfe.cn/gtrjgocumh.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtlynnyaxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.52xcode.cn/gtvrmhqhpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtrotxbjxr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aizwys.cn/gttxscrijf.html

Java: import java.util.List;
来源：http://hz.chenjidiqi.icu/gtlrcluxqv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtgmkswmeh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aibaodan.cn/gthsbouzec.html

C#:   using System.Text;
来源：http://hz.jinghuilouyu.cn/gtgsrjugtl.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtlqnlceiv.html

Py:   (lambda: print("run"))()
来源：http://hz.daxiang520.top/gtbtqmdzvz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gttoxaddxc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gttljuubda.html

TS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtmjjuwaov.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fengsongda.top/gtvmamnhdp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtfphfgdhv.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuanzhike.top/gtfqdkhaqq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cqqwz.cn/gtjzsyfrnt.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtucokmrjz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtluowlyes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtjuqjgxbm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtdreuqwty.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtltsnfsvk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtckyssino.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtpudqbpxq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtagdexmco.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.vqdsnc.cn/gtbedgpxvp.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gteygqmfmq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtynmcclom.html

PHP:  // 无泛型
来源：http://hz.gaohongyu789.top/gtfnmvjbao.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtgvlaeirp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtqxxehbbj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtxalpwvck.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aibaodan.cn/gtcglgvbdo.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtarlhospt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgufenzy.top/gtxuldeigs.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtyocdeptl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtfzokicpo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtbnwxregp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtodunditb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtvrzecqfd.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtiyadewtv.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gtojluktpm.html

Ruby: a, b = pair
来源：http://hz.yueranfly.top/gtaggtopxp.html

C#:   var (a, b) = pair;
来源：http://hz.yvedp.cn/gtsxxsfblx.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtroqhmmxw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dashuyun.cn/gtkwbvsjmo.html

PHP:  // 无重载
来源：http://hz.sufxvd.cn/gtkpwqdxtf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.snrcjt.cn/gtkztnimvb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gtmveqgglx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtvdfcasol.html

Go:   // 无重载：用不同函数名
来源：http://hz.bjfxy.top/gtjqjbaxux.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gtjanlsutm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.quarkkingdee.top/gtemqigjmr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtclectiaw.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtdnhhnfoo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtznyxubuh.html

[D01] 创建数组 / 列表
来源：http://hz.tianlin.xyz/gthvrqnohe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nanxinkj.top/gtbpkqnluu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nwbrower.top/gtrpifrurp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dianchejie.cn/gtcjfgrafm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtcznjllai.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgfzy.top/gtlnasudzv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtejhwilwa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtgfrqtzsp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnxiangtu.top/gtjeciowkr.html

[D02] 追加元素到末尾
来源：http://hz.ydjk.org.cn/gtnsifzedf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtzymwykli.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtjmrjrdjp.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtntrjfehm.html

TS:   arr.push(4);
来源：http://hz.svipenyu.cn/gtwqbyeicu.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtdbrkxolq.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtqjtnieqs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtfftoaqwj.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtckfjosty.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtuexbvoqi.html

Py:   arr.insert(0, 0)
来源：http://hz.svipenyu.cn/gtbtlqraye.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtuvflowlq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtbjvcjyfc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yonumen.top/gtiswyjcaf.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtprfqpbsb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dianchejie.cn/gtdhlnimbo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtsatelayg.html

C#:   list.Insert(0, 0);
来源：http://hz.xuetiantiany.cn/gtmtowhwdl.html

[D04] 删除元素
来源：http://hz.0kj1m.cn/gteuzbynld.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtqgqggfjp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dashuyun.cn/gtxqijfulg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtlepovoyp.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258.top/gtzgnuxtjn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtehnwjrss.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigfzy.top/gtwjaojeqs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gthfxbmpcn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtszutpnga.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gttwjdoijv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtetspeluf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtbrfcgweb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gzhubu.top/gtauoztnlq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtkmjnwddn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtchosycri.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtfaurzkro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtccopbhra.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.haohaochexian.top/gtpebbtzkb.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtaqsnkzko.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtkaxmjcwk.html

PHP:  count($arr);
来源：http://hz.chenzaomai.com/gtnafuuvnr.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtqhmzynoc.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtjdryiuuu.html

Java: list.size();
来源：http://hz.bjfxy.top/gtdxfckwnj.html

Go:   len(arr)
来源：http://hz.daxiang520.top/gtzuzucpth.html

Ruby: arr.length; arr.size
来源：http://hz.gotoacloud.top/gtgrintglr.html

C#:   list.Count;
来源：http://hz.xylfe.cn/gtpvjjcfvp.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtssmglrck.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258888.top/gtsdleocvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.redwolf501.top/gtcnccjxdo.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258888.top/gtjfvloruj.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtulhrsrvb.html

Java: list.subList(1, 4);
来源：http://hz.jianghu66.top/gtcaaayfuy.html

Go:   arr[1:4]
来源：http://hz.ydzc1.top/gtxtqahxog.html

Ruby: arr[1, 3]
来源：http://hz.c1oappe.top/gtssqwdwev.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenlongwang.top/gtjtptcrxw.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtfbftzjhe.html

Py:   a + b;  a.extend(b)
来源：http://hz.ivvv.top/gthfxhunsi.html

PHP:  array_merge($a, $b);
来源：http://hz.gzhubu.top/gtqawsuznv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtwoaavkqk.html

TS:   [...a, ...b];
来源：http://hz.fzhhl.top/gtlwuyegxs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtdnrmvwqf.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gtcgukspse.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtvbuwqqsl.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gttslasoxn.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtaciaycke.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtzibwbevn.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtgllfrmoh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtydgdiwfk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ppjwa.cn/gtfkgosvdg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtevsimdpa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gttzfuuqol.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtmpegbjbf.html

C#:   list.Sort();
来源：http://hz.jlsjyb.cn/gtpcqfhkqa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gtvtiwmhtl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gthmboapbi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtlufsbowg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtimjabowu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtwknoszdv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sysykeji.top/gtbyhpkqwy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtrltaamef.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.iojbl.cn/gtnmzslyhj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtvexggbtz.html

[D11] 反转数组
来源：http://hz.sysykeji.top/gtmfrvnpke.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fengsongda.top/gtpissdbxc.html

PHP:  array_reverse($arr);
来源：http://hz.aibaodan.cn/gtknerokqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtgvigojky.html

TS:   [...arr].reverse();
来源：http://hz.zdqjudy.top/gtlofgadid.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtgmfudtaa.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtltjxtdsg.html

Ruby: arr.reverse
来源：http://hz.bjfxy.top/gtwwbawzyn.html

C#:   list.Reverse();
来源：http://hz.nanxuanxn.top/gtrpidtdex.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gtljbwqala.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtrvzxqykf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gthtvufvgw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtlcqobpsg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtpeqswkwc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cdnleiting.top/gtwyuwdqgf.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtugtlmtvr.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtncnidsqh.html

C#:   list.IndexOf(x);
来源：http://hz.jqgfzy.top/gtlxhltzzn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtmkfwewfv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtsnhvyiyr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtbgqyljtw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.vqdsnc.cn/gtfrrtkegp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gthxtvgncq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydzc1.top/gtpknlvnvl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtxtgenamq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gtinqqtojs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtgvwacxvg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtkzxtrpin.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhiwuduotai.top/gtjgagcwew.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xziqi.cn/gtgnujgiqj.html

JS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtfnchplmq.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtejblsqqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guowangkeji.top/gthztwsgny.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtghoqumfr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtzyzqwhur.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gogol.net.cn/gtolsohczu.html

[D15] 去重
来源：http://hz.cashguo.top/gtthmvkbyk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtzqsgojjg.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtdietyhks.html

JS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtxsvzffsu.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtduknhkmv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtwfraaxhz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.kuanghao11.cn/gtwuofgmpe.html

Ruby: arr.uniq
来源：http://hz.hnxiangtu.top/gtfhbmrjdl.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtlvowfpwc.html

[D16] 求和与平均值
来源：http://hz.hnqzz.top/gtmbnezngq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtjjxjuydd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.52xcode.cn/gtaesuslfx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gthhvfndzn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gttswukbls.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtubaixkbl.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtjlhrngsm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtkodzjxlz.html

C#:   list.Sum();  list.Average()
来源：http://hz.tianlin.xyz/gtgnwmsjxq.html

[D17] 最大值与最小值
来源：http://hz.wangshuangyany.cn/gthruqapxl.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtxjhojoxw.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gttoweancy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhongyouzk.top/gtuwhadvks.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtffoznzkp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pengpengdd.cyou/gtnblsadly.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtxqeagnim.html

Ruby: arr.max;  arr.min
来源：http://hz.nanxinkj.top/gtmqfaryin.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtjeeaqiqn.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtuzowqbqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gtsnsxfmxv.html

PHP:  array_merge(...$nested);
来源：http://hz.hywenlv.cn/gtkhkdscrx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtwtwktwrl.html

TS:   nested.flat();
来源：http://hz.havefunace.top/gtlqpxdfgd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hongshengwenyu.top/gtmyufkqvj.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gttsfwhpnv.html

Ruby: nested.flatten
来源：http://hz.hysaishi.cn/gtzfccnded.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hongshengwenyu.top/gtwrzhpmgu.html

[D19] 按字段分组
来源：http://hz.xylfe.cn/gtmyvdgmgd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zdqjudy.top/gtedgfijaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ybcxt.top/gtncfktvpw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtusmqthsj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtxhqjmylu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtzrjjzdqj.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtvhgbghcm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gteqhnlxwb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gthrefdrwb.html

[D20] 统计每个元素出现次数
来源：http://hz.haohaochexian.top/gtqfbynave.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtpibinnpf.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtdemobrrj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gttgblhrzx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtyzfxsyvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtcvkexkyt.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gthfiptzqz.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtpdpgjnny.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtsoscmyfj.html

[D21] 判断是否包含某元素
来源：http://hz.meibo888.top/gtwbvtaynt.html

Py:   x in arr
来源：http://hz.zhengqikj.top/gtjcbxuovs.html


<!-- 参考信息 -->