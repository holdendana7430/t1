代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.hywenlv.cn/gtnwjtnqmq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hysaishi.cn/gtzlripyvq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.52xcode.cn/gtdskikxhf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhongyouzk.top/gtosotgppr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dianchejie.cn/gtauhsasew.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtkbstijxe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gtoocyuuzo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtuypqzqzt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jyoumei.cn/gtesscthlw.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtnvjechyx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.mhx1999.top/gtxyjklbbw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhiwuduotai.top/gtoccccsxr.html

Ruby: arr.map(&:upcase)
来源：http://hz.meibo888.top/gtmikfulaz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xziqi.cn/gtjfmrnvta.html

[C08] 闭包
来源：http://hz.zhoulong.xyz/gtxemptqcm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258888.top/gtjpktifbp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guowangkeji.top/gthpxzjlik.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtqnbdtrlo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtdaysxftz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhijiandao.cn/gtpyicbepn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jyoumei.cn/gtpxknmckc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.snrcjt.cn/gthwgtquhf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtplmuphxa.html

[C09] 递归
来源：http://hz.cheryme.top/gtiwhwglxz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtfpvqwedk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtlqmwzgsn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtaznuvofh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtamrcelnn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jyoumei.cn/gthfgxklhw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxinkj.top/gtjodpwwfn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtxrkytkpj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sxryk.cn/gtsxyaqpsh.html

[C10] 变量作用域
来源：http://hz.tian-w.cn/gtwrbktbja.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtbyslsxan.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.vqdsnc.cn/gtagxtdvzz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.daxiang520.top/gtpxkklvxl.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gterjspaum.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtwrfgkfwd.html

Go:   花括号块级作用域
来源：http://hz.havefunace.top/gtlkpofprf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnxiangtu.top/gtdtfbzvau.html

C#:   块级作用域
来源：http://hz.dianchejie.cn/gtbheusgpl.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtbhoqygar.html

Py:   from module import func
来源：http://hz.chenjidiqi.icu/gtkbbiazfy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtjrfsyjwr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yanxiufei.cn/gtdujxassa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtvflaworq.html

Java: import java.util.List;
来源：http://hz.jiagoushi.top/gtpwqxrafe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtyerdusxn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gtzvskmexk.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtlbnboovm.html

[C12] 立即执行函数 IIFE
来源：http://hz.pengpengdd.cyou/gtaezfvesd.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtidhjmowu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtgjcgsfvy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtvaqrlscs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtiajlydra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtduodmvrp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gttlihryzi.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtcehtmlet.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtrdblbcws.html

[C13] 类型声明 / 类型注解
来源：http://hz.aizwys.cn/gtgjnkgfpe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtcpgckdoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtcvgfstiv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtrkieyobl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtokqunidu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtfdvyrlpe.html

Go:   func add(a, b int) int
来源：http://hz.cashguo.top/gtlrpetbjp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtplaixkql.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hongshengwenyu.top/gtuuurxzbe.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtfvfbqpeq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hammf.cn/gtdeqyodcx.html

PHP:  // 无泛型
来源：http://hz.chenjidiqi.icu/gtbqkwmtyi.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gttvlqrsmk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenjidiqi.icu/gtzxlhannw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.redwolf501.top/gtpyoennkt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenlongwang.top/gtmcqkuxos.html

Ruby: # 无泛型
来源：http://hz.ywan-chungtsiang.top/gtnhyyngjr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtncevuaah.html

[C15] 解构 / 展开参数
来源：http://hz.cheryme.top/gtcixvtixc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gthokiikba.html

PHP:  [$a, $b] = $pair;
来源：http://hz.iojbl.cn/gtygnjtaxf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtwpgfvbvu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hysaishi.cn/gtgdaxfuhg.html

Java: // 无解构
来源：http://hz.sufxvd.cn/gthwwxkbfb.html

Go:   // 无解构
来源：http://hz.wangshuangyany.cn/gtcwnkszsv.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtfmiqioce.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtsylipppa.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtzetuaqnr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtuxyvxhdl.html

PHP:  // 无重载
来源：http://hz.iojbl.cn/gtynzkfvsu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gthhxbhsyk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtcyhuvori.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtplfxcbef.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtgapagwgk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtsnkzpevo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.iojbl.cn/gtlpattwqp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmnrjtgti.html

D. 数组 / 列表 / 集合
来源：http://hz.zhongyouzk.top/gtfvjhxwph.html

================================================================================
来源：http://hz.316326.xyz/gtnmvurxms.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtkwhvwqbo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gtrwjozmwt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ywan-chungtsiang.top/gtetlbasfd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jqgfzy.top/gtpnfaynce.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtrtnycznp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtlmvqquwu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jianghu66.top/gtzajmigob.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hfpthk.cn/gtauuyabtu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.svipenyu.cn/gtuxuwcwnr.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtaplgfhia.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gttueyrgch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtvjuxlkrl.html

JS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtzpoqtkpc.html

TS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtlcsnailk.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtjyfvjwve.html

Go:   arr = append(arr, 4)
来源：http://hz.svipenyu.cn/gtemxenzat.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtvglpmtwf.html

C#:   list.Add(4);
来源：http://hz.ydjk.org.cn/gtymhpoirt.html

[D03] 在指定位置插入元素
来源：http://hz.hnxiangtu.top/gterpifkzg.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gtrkgpaqjo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sweek.top/gtzhyclbum.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ivvv.top/gtsrtokkfi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gaohongyu789.top/gtmnecbfgx.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtdbblqvmj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtmumbbsdu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.9152youxi.cn/gtyrcwohec.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigufen.top/gtwvfmihqd.html

[D04] 删除元素
来源：http://hz.pengpengdd.cyou/gtlftzrwqh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtqzxbazxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtevazgpdn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtyvkcxweb.html

TS:   arr.splice(0, 1);
来源：http://hz.zycfv.cn/gtyloescut.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtgkfafcem.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gtpbbzctma.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtlzocykfy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jyoumei.cn/gtprhukxsn.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtwehigrku.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtbnfdgjks.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtzdbbmcki.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtkxrhtpqm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtrpdzewuv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhaomingkeji.xyz/gtlwvebhjs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydzc1.top/gtgyrojoth.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtksgnbrao.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj202588.top/gtpqcmjihs.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtbekuhvbs.html

Py:   len(arr)
来源：http://hz.9152youxi.cn/gtatlrtxof.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtbexhcmdf.html

JS:   arr.length
来源：http://hz.mhx1999.top/gtfwcmcdnr.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtmnvhjawv.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtxzkkkosw.html

Go:   len(arr)
来源：http://hz.ydzc1.top/gtsgdrtbch.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtnstratzz.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtcwsodici.html

[D07] 切片 / 取子数组
来源：http://hz.sweek.top/gtfistchoy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nwbrower.top/gtmxjemdtm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dianchejie.cn/gtzpfcswhs.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtookufova.html

TS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtwgogdztq.html

Java: list.subList(1, 4);
来源：http://hz.hysaishi.cn/gtwhabmkyl.html

Go:   arr[1:4]
来源：http://hz.xuanzx.com/gtfqdlfvgg.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtxyeeowdv.html

C#:   list.GetRange(1, 3);
来源：http://hz.daxiang520.top/gtpfxelswf.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtwsrnubfr.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtqlsgvery.html

PHP:  array_merge($a, $b);
来源：http://hz.zhiwuduotai.top/gtnbhdqzzg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtsaeaqrgp.html

TS:   [...a, ...b];
来源：http://hz.nanxuanxn.top/gtlrkymtps.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtcvwlzghe.html

Go:   append(a, b...)
来源：http://hz.0kj1m.cn/gtuuctfudr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gtxrxambwf.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenjidiqi.icu/gtpqqycxck.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtkctiozfo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtqszwbscq.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtvmgzojtd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtqjvtwuvq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtagdockmj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gthnffknsq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gtxwrajxxd.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtigfqrolm.html

C#:   list.Sort();
来源：http://hz.tian-w.cn/gtiburbnbl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtjvwrzxvn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxuanxn.top/gtgdvjtnwx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gtiigxykoc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtkfbfjspc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gthbrlrwnu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtqbuuvaup.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hfpthk.cn/gtvbsfszif.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dianchejie.cn/gtsrluyzeh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtvleyltqi.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtlprnsjcz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtdjsccvbe.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtxsqhhdyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtzcytpwcj.html

TS:   [...arr].reverse();
来源：http://hz.xylfe.cn/gtbyrccagu.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtsbletkyl.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgfzy.top/gtucqojaoi.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtmgywxzde.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtybzlbnhv.html

[D12] 查找元素下标
来源：http://hz.tian-w.cn/gtrlyaxdod.html

Py:   arr.index(x);  x in arr
来源：http://hz.tian-w.cn/gtpmplfram.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.bjfxy.top/gtadvybgkp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtctwxzrhl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtvhfrilxe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtxnsjseub.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtvxgqcbkx.html

Ruby: arr.index(x)
来源：http://hz.aibaodan.cn/gtccnlydgv.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtgafqafdf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtpzomlyjk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtbmyiftvx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtorvzbqse.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtoqzgrmat.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gthgtzdxqy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.0kj1m.cn/gtfwxtxrcw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtfyvlfgqf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtgfctnoul.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtbpnztaiu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtzzmfjgnj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigfzy.top/gtnfjzalkl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhijiandao.cn/gthoysndnd.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gttnziugfo.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gthfbrsglc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtfwkcmntq.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtafkaekpo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtsphplfsy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtqsvkhjmn.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtcjbcslmq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtuaqsfozd.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtauyjvjfo.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gthgxnqbgw.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtdnjehzwr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sxryk.cn/gtyxchskrb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtplwwmxeo.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtyzczvzge.html

C#:   list.Distinct().ToList()
来源：http://hz.iojbl.cn/gtwaodmaqo.html

[D16] 求和与平均值
来源：http://hz.vqdsnc.cn/gtfcpgplqv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtrfiqbjrv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tianlin.xyz/gtncbuxdmu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtymxymmpi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtdntynbfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtqlrkmtip.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtwkgmrynd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigfzy.top/gtkxiyhomm.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtbwzoswal.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtmowwmiab.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtsxxxrweu.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtbfhmsrxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtqahcgqqu.html

TS:   Math.max(...arr);
来源：http://hz.vqdsnc.cn/gtdidjtvmt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gtwdgbnoth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtoliwqjem.html

Ruby: arr.max;  arr.min
来源：http://hz.aizwys.cn/gtxlpclcin.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtgfyqsnut.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtdpfavgej.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtaoumfihv.html

PHP:  array_merge(...$nested);
来源：http://hz.shangyingyoupin.top/gtqxamqreg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yonumen.top/gttaxbvyeq.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtkykimysr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gtxepelthk.html

Go:   // 手写双层循环
来源：http://hz.sweek.top/gtbfixmoba.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtkqxxpfdr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtjvhzsodt.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtdzrycpsv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtmuektuwz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuanzhike.top/gtdncdksgg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuetiantiany.cn/gtjnzrjjfv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtyvolxcsl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gtulyutlbm.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gthiiudhob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yueranfly.top/gtxgsvxxlu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtciqafcim.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gtfgdhszqc.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtulqkdgss.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtcnnvbfep.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtsktwlfud.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtnyhbfdxs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.vqdsnc.cn/gtrdssumdb.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gtovzjmmzk.html

Ruby: arr.tally
来源：http://hz.chenzaomai.com/gteaazimrq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtyotymjxc.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigufen.top/gtrjiesbwp.html

Py:   x in arr
来源：http://hz.wangshuangyany.cn/gtppwbaknj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gthdiresas.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gthfjopfmh.html

TS:   arr.includes(x)
来源：http://hz.wangdashe.top/gteiwscypo.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtlkxytioe.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtrgspkcpn.html

Ruby: arr.include?(x)
来源：http://hz.fengsongda.top/gtmgdqswpr.html

C#:   list.Contains(x)
来源：http://hz.c1oappe.top/gttsyguxla.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtkepthdug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtzjrdumtt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gttkwoijcp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtlowobtdb.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtyaaithtr.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtlzrftmdm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yanxiufei.cn/gtktpmokoe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtutaqsxtn.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtnffdmtba.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gtbfngudbf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtrnpauxwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fengsongda.top/gtevofeneh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtwopoudfd.html


<!-- 参考信息 -->