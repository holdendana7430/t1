代发 wailian999

Py:   return a, b
来源：http://hz.smart0.xyz/gtolrxvnyx.html

PHP:  return [$a, $b];
来源：http://hz.ydzc1.top/gtaxjrxqke.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xziqi.cn/gteqpqcunv.html

TS:   return { a, b };
来源：http://hz.havefunace.top/gtoxbuptbb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtqigdvyms.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtgmyxgrrv.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gtkfdgvjim.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtyzwkvefl.html

[C06] 匿名函数 / lambda
来源：http://hz.yj20258888.top/gtkabtxoxr.html

Py:   square = lambda x: x * x
来源：http://hz.guowangkeji.top/gtognxrddj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.smart0.xyz/gtoydswzfg.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtwulnsdap.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenjidiqi.icu/gtyhuxojbo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cdnleiting.top/gtltptljse.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.316326.xyz/gtinxkhavp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtmgatvigl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sysykeji.top/gtbqbrkmnc.html

[C07] 把函数作为参数传入
来源：http://hz.zhiwuduotai.top/gtdbsojwqa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtlpkrsdfx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtiiwmxddt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ehwqpu.com/gtiipqdwrc.html

TS:   arr.map(String)
来源：http://hz.havefunace.top/gtlqggbawh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yonumen.top/gteycnnlaz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yangfankeji.com/gtzegeinrc.html

Ruby: arr.map(&:upcase)
来源：http://hz.gotoacloud.top/gtoargjecv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtesobxuqd.html

[C08] 闭包
来源：http://hz.zhengqikj.top/gtbjzxmein.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hongshengwenyu.top/gtrihnmwtm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtzjhakvwq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtyzlikfds.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtbfppmqia.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtaslodqxx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ppjwa.cn/gtbssdclgz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenlongwang.top/gtokvmsegn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtdutymbpm.html

[C09] 递归
来源：http://hz.nwbrower.top/gtnoxhvwxj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dianchejie.cn/gttdtcaher.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtvencqbyp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aibaodan.cn/gtoabfoemi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtiraomrft.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtvqwjgmcm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.bjfxy.top/gtqhhghgpt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtupwuzohy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhixingplan.top/gtmcbfnlgu.html

[C10] 变量作用域
来源：http://hz.yj202588.top/gtifjrczkf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtqqcwdygq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gttxuxbwmx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtnskxbpzu.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtpteudmuo.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtasdfnlzr.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtucdwiffr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhaomingkeji.xyz/gtfehhrupp.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtittgmjlf.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtlquapioq.html

Py:   from module import func
来源：http://hz.cucudq.cn/gthlqktmhm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtkstgarji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xinyue.icu/gtpybivshw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtiitnkmvk.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtpfdqaarp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtebwkcfio.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ybcxt.top/gtlrbsuqlj.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtkjwdhkly.html

[C12] 立即执行函数 IIFE
来源：http://hz.ybcxt.top/gtsiptatja.html

Py:   (lambda: print("run"))()
来源：http://hz.iojbl.cn/gthdaspdqr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sysykeji.top/gtknuuznsj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtfsimmnit.html

TS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtwwabggsu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtlvhirmbx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtzhmxrmuh.html

Ruby: -> { puts "run" }.call
来源：http://hz.birdmap.top/gtsygyxioj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtokktfqlg.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtxhdwgymd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtshfuhclj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtpjqpreqr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuetiantiany.cn/gtbsofwabe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtdesvwphz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtcxadklnt.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtvepymibj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtknseibju.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtczxdnqpf.html

[C14] 泛型函数
来源：http://hz.gzhubu.top/gtwotppllo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtijpxdvfi.html

PHP:  // 无泛型
来源：http://hz.yj20258888.top/gtavunepiq.html

JS:   // 无泛型
来源：http://hz.cdnleiting.top/gtpuwfvjqw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtgthppnlg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yueranfly.top/gtuiowcsaf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gthsyjbhnh.html

Ruby: # 无泛型
来源：http://hz.hnqzz.top/gthdhcomev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yueranfly.top/gtzcrouupa.html

[C15] 解构 / 展开参数
来源：http://hz.ivvv.top/gtksmqfnhi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydzc1.top/gtqjrbipym.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtsgvggetx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtokqsjzaa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtlllojsce.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtwtgumxdw.html

Go:   // 无解构
来源：http://hz.havefunace.top/gtcbvvdfbd.html

Ruby: a, b = pair
来源：http://hz.smart0.xyz/gtzechtdrk.html

C#:   var (a, b) = pair;
来源：http://hz.pengpengdd.cyou/gtbygintis.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtvegxsevx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gthsoknvjv.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtimyvlfua.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gttwoljitb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenzaomai.com/gtcdfwczod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gthzwfrbcr.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtywpimzla.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shangyingyoupin.top/gtrbthxvfb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gthmhawevo.html

================================================================================
来源：http://hz.xylfe.cn/gtsgfgejuj.html

D. 数组 / 列表 / 集合
来源：http://hz.dashuyun.cn/gtsbgpiedl.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqkndcapl.html

[D01] 创建数组 / 列表
来源：http://hz.aibaodan.cn/gtslvgzymx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuetiantiany.cn/gtvstuqcop.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtojutynia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gtbbpjomlj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.mhx1999.top/gtwihrrnpc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gtokbuzchi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtencmnckd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ivvv.top/gteslxirmg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxuanxn.top/gtkbiemwnw.html

[D02] 追加元素到末尾
来源：http://hz.hnqzz.top/gtbmjimboz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guannengcc.top/gthwtogalw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.havefunace.top/gtzjbfxcwn.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtgilnwbyl.html

TS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gtshqjwlcg.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtukerqrls.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtnkraxgij.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtofvbijod.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtpetzxrsq.html

[D03] 在指定位置插入元素
来源：http://hz.gzhubu.top/gtagosydiz.html

Py:   arr.insert(0, 0)
来源：http://hz.ywan-chungtsiang.top/gtznpddwqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtuomoyied.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenlongwang.top/gtsxljwbmg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtekycivpd.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtwjlpzgof.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtbtoiqckg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtkubyogwr.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gttkzlfugi.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtivwiiwjn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.smart0.xyz/gtituhdpaw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jlsjyb.cn/gtqlewxtah.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhijiandao.cn/gtqnpwhnif.html

TS:   arr.splice(0, 1);
来源：http://hz.snrcjt.cn/gtgehfjbws.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhijiandao.cn/gtlwswnkub.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtsxqrpclx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtgyfplqgu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtwrusribs.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtouhhyntf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtmvmriwpj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxinkj.top/gttlcnbamx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtrmuarunb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtpvrmghvo.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtsswamqxo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtpyttqyub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtwhwidlix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xinyue.icu/gtkbpcyqva.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtakjyhbdp.html

Py:   len(arr)
来源：http://hz.andypj.xyz/gttlfjgnff.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtpfkqphes.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtviumgyau.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtacixnnej.html

Java: list.size();
来源：http://hz.havefunace.top/gtbkegzwnc.html

Go:   len(arr)
来源：http://hz.xziqi.cn/gtcdznbdkv.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtjlzeblkw.html

C#:   list.Count;
来源：http://hz.jyoumei.cn/gtjwwgrmca.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtblvgsgun.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtcdcsycfd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gttsvmvydl.html

JS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtaabiuatj.html

TS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtrqhptrsz.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtvppllsja.html

Go:   arr[1:4]
来源：http://hz.snrcjt.cn/gtlahbtjcz.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtzpgathby.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtksrkpdem.html

[D08] 合并两个数组
来源：http://hz.xylfe.cn/gtkxvlztxm.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtdxufgonf.html

PHP:  array_merge($a, $b);
来源：http://hz.wangdashe.top/gtdtmlynjd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.iojbl.cn/gtlzicsedr.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtzjdbuokm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.wangdashe.top/gtooxowkhi.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtzkxotqvw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangshuangyany.cn/gtfobtetzw.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtlzzycqhy.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtqofbshez.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gturowlqpy.html

PHP:  sort($arr);
来源：http://hz.meibo888.top/gtgrheiewq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydzc1.top/gtxitqhvgg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtksbqojji.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gtvntvmhmh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtinhxvfpm.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtyjefacnh.html

C#:   list.Sort();
来源：http://hz.9152youxi.cn/gtlgyxajxl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shzxlz.cn/gtqzbjufbd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.iojbl.cn/gtrcfevowz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gthpxadqnc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtpfxvybcm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtfczushhu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hywenlv.cn/gtzcdttkwj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gtklqwewzo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guowangkeji.top/gtkefqqfbb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.mhx1999.top/gtfmlimxjx.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtkgfuktlm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aizwys.cn/gtoevhqrxi.html

PHP:  array_reverse($arr);
来源：http://hz.yonumen.top/gtcooierce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xziqi.cn/gteslqvmoc.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtjzsmnged.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtxttxrdzl.html

Go:   slices.Reverse(arr)
来源：http://hz.zhiwuduotai.top/gtsvdjydxb.html

Ruby: arr.reverse
来源：http://hz.shuidangran.top/gtonnfyscx.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtvxtllspf.html

[D12] 查找元素下标
来源：http://hz.gzhubu.top/gttwruptub.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtcigwisae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guannengcc.top/gtplkebsdh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtwnjboaby.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtxqcrvbez.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtnbfmhpfn.html

Go:   slices.Index(arr, x)
来源：http://hz.wangdashe.top/gtjizfxpbo.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gthwrlesru.html

C#:   list.IndexOf(x);
来源：http://hz.yangfankeji.com/gtjnalwnwc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtrstlrywl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydjk.org.cn/gtvxofjjsr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtjkggskdz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtqyqnkzay.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtbuxwpfqb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daria6918.cn/gtjoxhwdnu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangtech.top/gtazfmmoej.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj202588.top/gtslzvhbkb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtmfngqjnk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shuidangran.top/gtjzltxnpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtarenrmvc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtssfjoboi.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtnjmrnxln.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtwaalygic.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtqdzpppkd.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gttkzlxjvn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuanzhike.top/gtllzfqosc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guannengcc.top/gtftczlufw.html

[D15] 去重
来源：http://hz.yj20258.top/gtskdlfnqu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jyoumei.cn/gtkychoqqx.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtoydwrqeb.html

JS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtcytmpdyr.html

TS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtcbresfpg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtnwoekxmw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtikoikqys.html

Ruby: arr.uniq
来源：http://hz.guannengcc.top/gtpeelpcym.html

C#:   list.Distinct().ToList()
来源：http://hz.daxiang520.top/gtvguhwcbw.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gtpsupkkjp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtmchnrvng.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtcwavigxl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtfmgrjpmf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gttwfjshfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtegpslssc.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtexlnmwfu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.52xcode.cn/gtmqyihmjp.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtiqocmhmg.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtfpaxnakd.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gtcyzqyvtu.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtyvqxkfsv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtuecnwshc.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtbmqcdqvu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtgasonlca.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtaksqwviv.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gthwqgzpbu.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtmxqjfboy.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtnszhxngq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtdiuyuupb.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgufenzy.top/gtepjyahzb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtdgdezwrk.html

TS:   nested.flat();
来源：http://hz.yanxiufei.cn/gtaqcitlmq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtsetfnhie.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtbldroinu.html

Ruby: nested.flatten
来源：http://hz.hnqzz.top/gtbwptuqxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuxming.cn/gtktoqyuiw.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtfdjarter.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fengsongda.top/gtakcxseum.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yueranfly.top/gtplitvoyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gticwytvev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gtafkqjrzy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hammf.cn/gtegmmhnba.html

Go:   // 手写 map[string][]T
来源：http://hz.dashuyun.cn/gtwnaauown.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtxkzqqkpx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gaohongyu789.top/gtmulsrrwq.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtplwnzvul.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gthqprkyya.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtcoxgqhff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtukzjqihd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtqstzdbdq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtlzxngved.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtgntgxwus.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtrsqdsqqq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gtygqkyits.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtefsnwwzx.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gttsbrczmf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gthvwcvvcj.html

JS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtwachaqpx.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtzocdlmzb.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtqnwvkcfw.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtmstcpzrr.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtsuaraaqm.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtpyngwogv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.dianchejie.cn/gtywbamakh.html


<!-- 参考信息 -->