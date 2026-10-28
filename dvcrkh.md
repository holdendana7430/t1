代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtxkgdvoyg.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtluxcrxyd.html

Ruby: return a, b
来源：http://hz.yueranfly.top/gtddiuwfqc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtgsxnzqbd.html

[C06] 匿名函数 / lambda
来源：http://hz.xylfe.cn/gthqvfhpog.html

Py:   square = lambda x: x * x
来源：http://hz.jiagoushi.top/gttmyiewjd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtbvgbgxyx.html

JS:   const square = x => x * x;
来源：http://hz.316326.xyz/gtkzqplglj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zdqjudy.top/gtamtmcjlz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.redwolf501.top/gtpmfkdpss.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenzaomai.com/gtbzzkkggf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gaohongyu789.top/gtwteoqzwv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtvexqznqs.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigfzy.top/gtlrlnfqmb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pengpengdd.cyou/gtnvmycyrg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenzaomai.com/gtluoukpue.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtmmjwnxni.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtrytdmeqa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jlsjyb.cn/gtpfzkuibu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.redwolf501.top/gtqfudklnn.html

Ruby: arr.map(&:upcase)
来源：http://hz.zdqjudy.top/gtqpuzgjsz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuanzhike.top/gtkgrvurzv.html

[C08] 闭包
来源：http://hz.sufxvd.cn/gtcrxrlsfo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.snrcjt.cn/gtkwafzxvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.iojbl.cn/gtizgjgwmh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gthujrvexr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtrvjymfno.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.feifeiyinyue.top/gtlsidftln.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ppjwa.cn/gtljdtuwev.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtnomubqjo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtcwueoljz.html

[C09] 递归
来源：http://hz.sxryk.cn/gtroaigzam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtrtrbgzmw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cashguo.top/gtfmeypkto.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtfjbijact.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shangyingyoupin.top/gthhuqfais.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtmjkkqaal.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gtbyutwqvq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtvdzkxwxx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtgykmanhn.html

[C10] 变量作用域
来源：http://hz.xuanzx.com/gtbkutbvey.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gthtxtibht.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtoobhqxkq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtnrsoqeyy.html

TS:   同 JS
来源：http://hz.fengsongda.top/gthqudnefm.html

Java: 方法内为块级作用域
来源：http://hz.cqqwz.cn/gtsmvfhgqg.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtxrblpklz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fengsongda.top/gtgukvhibf.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gthbavedsx.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtyifkzfmu.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtbxoeuwhq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtsujravdx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cqqwz.cn/gthdogwvuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hfpthk.cn/gttsckcedl.html

Java: import java.util.List;
来源：http://hz.birdmap.top/gtfqxodxip.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jianghu66.top/gtfbjnoozp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.dashuyun.cn/gtswjihgzb.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtuqkpkpjv.html

[C12] 立即执行函数 IIFE
来源：http://hz.ivvv.top/gtekcyypyd.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gttswyimwr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hywenlv.cn/gtabznypox.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gthlmojaqe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gttvikkcqe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gogol.net.cn/gtmenjgfqc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtvnutwsss.html

Ruby: -> { puts "run" }.call
来源：http://hz.shuidangran.top/gteuixgzez.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cqqwz.cn/gtsqidwcpy.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtilzcyjxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gtbtcxvggf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gttjlzsnqa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gthrcokbii.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtdzrblvoo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtmfhkuzwb.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtogxuztql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.quarkkingdee.top/gtrrrklxsp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtdnqxatwf.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtnbqcyxnz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtchndaifu.html

PHP:  // 无泛型
来源：http://hz.cucudq.cn/gtyxtbjttn.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtcvuonagt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnqzz.top/gtxhmcaetg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sweek.top/gtmitqbces.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hysaishi.cn/gtamgtggvh.html

Ruby: # 无泛型
来源：http://hz.zhiwuduotai.top/gtmybayiml.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtilzpnskz.html

[C15] 解构 / 展开参数
来源：http://hz.hysaishi.cn/gtuafzsxue.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtpqrprlxa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gttkmejtxx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtriklhftw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtletinyfd.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtkpudffnx.html

Go:   // 无解构
来源：http://hz.iojbl.cn/gtycflgxnc.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gtzbmqanbs.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gtgixsvidl.html

[C16] 函数 / 方法重载
来源：http://hz.meibo888.top/gtvhtxgxyv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangkeji.top/gtgykllets.html

PHP:  // 无重载
来源：http://hz.zhongyouzk.top/gtmjvuorky.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tianlin.xyz/gtppelqayf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtorpleoad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtasuciwtg.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtfepxddkk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.52xcode.cn/gtvpsrqjow.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuxming.cn/gtzxetfvhq.html

================================================================================
来源：http://hz.cucudq.cn/gtdozeoopj.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gtqacogema.html

================================================================================
来源：http://hz.hysaishi.cn/gtdcqvpaej.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtcsplzjyu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dianchejie.cn/gthkhaokdy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtfgyxpczd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtnospxnmz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gotoacloud.top/gtysdhzbfk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtgqjprfeq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtjvvtilem.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtaqburlvo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtizdzlyzy.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gtfkijmjiz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xingfuxueyuan.xyz/gteddoqxxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gttahzxbet.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gthkwllctf.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtuzhcibxx.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtkxvemadj.html

Go:   arr = append(arr, 4)
来源：http://hz.tian-w.cn/gtgfzaiegh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aizwys.cn/gtnmwirexs.html

C#:   list.Add(4);
来源：http://hz.daria6918.cn/gtunovzkts.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtcjejrycn.html

Py:   arr.insert(0, 0)
来源：http://hz.shangyingyoupin.top/gtsvqvunki.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtabbhlemh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.bjfxy.top/gtoitwnqsg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtbigzlilo.html

Java: list.add(0, 0);
来源：http://hz.hywenlv.cn/gtwjtkhfmv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtnqunmwps.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gtvpiayflm.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtphmlzvaw.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtojduiafh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dashuyun.cn/gtygctgxqv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhoulong.xyz/gtbojakjxu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258.top/gtcgtllewe.html

TS:   arr.splice(0, 1);
来源：http://hz.cqqwz.cn/gtcuctofzc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtnedqirdj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenjidiqi.icu/gtnqxmpjsp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cucudq.cn/gttcqbtcxr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.andypj.xyz/gtfrdadxub.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtplhjpdqv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtutfkndfs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fengsongda.top/gtktnrklim.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.snrcjt.cn/gtvjlgigcg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtcrymiaae.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gthwbprgfk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtzclozvxx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtgpegckmb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cheryme.top/gtfhnoltag.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtkijhcfbn.html

Py:   len(arr)
来源：http://hz.sweek.top/gtzamvprlr.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtyrqblrtr.html

JS:   arr.length
来源：http://hz.ppjwa.cn/gthvcclirj.html

TS:   arr.length
来源：http://hz.tanke756.top/gteansqktf.html

Java: list.size();
来源：http://hz.yongpay.top/gtrmtjarfl.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtvfxdhfgs.html

Ruby: arr.length; arr.size
来源：http://hz.jinghuilouyu.cn/gthokoxspl.html

C#:   list.Count;
来源：http://hz.c1oappe.top/gtvifnrftn.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtyldhcqyd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtepugqnoh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtsmlldjnt.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gthbeyqqrz.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtllvzuzev.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtvrxuilmi.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtadxdnzke.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtgojsnklh.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtdgncumfr.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtqwkztczv.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gtfwxhwgnz.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gtmnyfvayt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.svipenyu.cn/gtdrytpetb.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gteoxfwmur.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.havefunace.top/gtfqgplehb.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtkqabxgog.html

Ruby: a + b;  a.concat(b)
来源：http://hz.havefunace.top/gtplxcwkcf.html

C#:   a.Concat(b).ToList()
来源：http://hz.jlsjyb.cn/gtodtoglww.html

[D09] 排序（升序）
来源：http://hz.havefunace.top/gtdkimzvba.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtzdqnexiv.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtrvosqhov.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtrwedhbfa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daxiang520.top/gtxttaorrn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ybcxt.top/gtfuudhjcx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtzjrwxdjm.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtwpjoneyx.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtycoycpgx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtyilvraik.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hfpthk.cn/gtptbnufmr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtlnaxmudv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.dashuyun.cn/gtkwefazmy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtardjsboj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhixingplan.top/gtlundkpwi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.316326.xyz/gtmbtrwcvq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtwvdfksbh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtrfjsqxlg.html

[D11] 反转数组
来源：http://hz.yj20258.top/gtowblrpmc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtuvvccmeu.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtefixhpsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shzxlz.cn/gtwtodnveh.html

TS:   [...arr].reverse();
来源：http://hz.52xcode.cn/gtmonbhuyk.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gtwfpsyzha.html

Go:   slices.Reverse(arr)
来源：http://hz.xuanzx.com/gtnbfcxtcu.html

Ruby: arr.reverse
来源：http://hz.mhx1999.top/gtotfuzium.html

C#:   list.Reverse();
来源：http://hz.jqgfzy.top/gtdqflcdxo.html

[D12] 查找元素下标
来源：http://hz.hnxiangtu.top/gtbcflefog.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtxhwjvbxb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtjrmkyvbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtnchjjxsk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtumoubszc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yvedp.cn/gtxhjclrxa.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gtsflmcmak.html

Ruby: arr.index(x)
来源：http://hz.guannengcc.top/gtotihbfsc.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gtslfwxulf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtffituyrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangkeji.top/gtxjhrdnhx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtsjoxmial.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtofxydxan.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtlloewncb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hongshengwenyu.top/gtsbzbjtdb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gthnthvsap.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtcfqfockj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gtdzhxzeqi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinyuanbaomall.cn/gtxzofymwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtlkxnlgzg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtmabdwmts.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtqwowdroo.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtfkwaovux.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtfiapvllc.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtcclnsyht.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daria6918.cn/gthpzllozd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtwuxzfzrc.html

[D15] 去重
来源：http://hz.havefunace.top/gtouycxpqj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtinvosthc.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gtkvfgqxmb.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtwafhaxln.html

TS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtllzbdqfd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtitnxkdaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jyoumei.cn/gtglitgrxs.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gtxqaubxrx.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtnjaclogb.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtjxvckzon.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hammf.cn/gtanjcuvvb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtqzbvdqvv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtpunnhfwd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtwltafeqf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gterqodeam.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtjmfwezvw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.smart0.xyz/gtrmamrcuv.html

C#:   list.Sum();  list.Average()
来源：http://hz.wangdashe.top/gtyzhlbazw.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtckxqspda.html

Py:   max(arr);  min(arr)
来源：http://hz.hammf.cn/gtpzosuhlg.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gtjyhtfnrw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtqlpxkvoy.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtewcfsahy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtjbmlqyio.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydjk.org.cn/gtfvakyfgg.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtdyvqyxkq.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtenhlfojs.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtlkyrqndo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daxiang520.top/gtzkhnshom.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtkluvzmza.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtnzsnuemr.html

TS:   nested.flat();
来源：http://hz.hnxiangtu.top/gtexpfkhvo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtunhrkxnk.html

Go:   // 手写双层循环
来源：http://hz.tanke756.top/gttkuzgpgo.html

Ruby: nested.flatten
来源：http://hz.316326.xyz/gtqqjbckkb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtzzuivzqa.html

[D19] 按字段分组
来源：http://hz.meibo888.top/gtqnwnbypw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtmagfhejp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtxuarzetc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtwhctdhqj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gttrcfcqew.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gtnypdirox.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtpowmgytn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258.top/gtztokngxt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtkqfacztv.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtghkuyofo.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtjclzunpd.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtbxlwqywc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtsmjzameq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtlnpofppc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtfoueaxhs.html

Go:   // 手写 map[T]int
来源：http://hz.meibo888.top/gtronxhgby.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtyejelluf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.snrcjt.cn/gtzyydnttj.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtbwarxgdk.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtjcokofiz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.316326.xyz/gtpcpizocv.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtxptkbogf.html

TS:   arr.includes(x)
来源：http://hz.yonumen.top/gtibndwceo.html

Java: list.contains(x)
来源：http://hz.jqgfzy.top/gtxjkkhxyj.html

Go:   slices.Contains(arr, x)
来源：http://hz.mhx1999.top/gttnoqjfka.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtmgaaxone.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtixrdbmnu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.bjfxy.top/gtiasxeulu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtpgfhugvb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtezhnvxin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hysaishi.cn/gtkxselmkr.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtnifumxhq.html


<!-- 参考信息 -->