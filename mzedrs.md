代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tanke756.top/gtklsawzhj.html

TS:   arr.map(String)
来源：http://hz.bjfxy.top/gtwyuvmwym.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhiwuduotai.top/gtdisiegsp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtzgkqlzks.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuxming.cn/gtrfokrcwj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daria6918.cn/gtzyexqrnr.html

[C08] 闭包
来源：http://hz.chenjidiqi.icu/gtoiwyludh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jyoumei.cn/gtkerwtnul.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtmxveklmv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtplezohgk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtevfszmbo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnxiangtu.top/gtctyqzbge.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangkeji.top/gtaikgiphi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtooadklhd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtmdahsvsm.html

[C09] 递归
来源：http://hz.shanyushiyangtech.top/gtqsihjxvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtlznttuyq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.feifeiyinyue.top/gtxhrcqgea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtnuvucisj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtxyujrqqv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zdqjudy.top/gtupqpzysv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtcbmexhlb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtmideoifh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cheryme.top/gtecbpclbu.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtiljmzdoc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xingfuxueyuan.xyz/gtwcepdclh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtfnowizmt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.andypj.xyz/gtkxdjyjmc.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtpsgtodpa.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtaqeslbsc.html

Go:   花括号块级作用域
来源：http://hz.mhx1999.top/gteoeuxkiw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangshuangyany.cn/gtciomaszl.html

C#:   块级作用域
来源：http://hz.gogol.net.cn/gtijqxmuhc.html

[C11] 模块导入与导出
来源：http://hz.tianlin.xyz/gtapwfymtr.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtgpqsjccf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinyuanbaomall.cn/gtfvmgphym.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gogol.net.cn/gtgttcdbgu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gaohongyu789.top/gtqgazpwdf.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtlnfslqlk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtzpizxzsn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtvbsnuvle.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtgpbryvox.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gthxktaxbd.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtduqmxozc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.iojbl.cn/gtmjdhezlp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtxkpwuxqe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtrdwiwutn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.0kj1m.cn/gtbknazhir.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtqdgooxyr.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtsdvexbmv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gtiahpupss.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtnlmnkjys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tian-w.cn/gtkddzyxfg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtfuiqpyna.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtitbbyjka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtbzyztwig.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtgkbbqjrv.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtcikuwctb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xylfe.cn/gtkobddqaq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhiwuduotai.top/gtgkdheive.html

[C14] 泛型函数
来源：http://hz.sweek.top/gtsfewjmxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtkwahuxql.html

PHP:  // 无泛型
来源：http://hz.xuanzx.com/gtbfvganzb.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtgivtaakn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jianghu66.top/gtlakedwze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tanke756.top/gtghypevox.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gtoruzklmr.html

Ruby: # 无泛型
来源：http://hz.jyoumei.cn/gtkzrtodkp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gtmzzacjan.html

[C15] 解构 / 展开参数
来源：http://hz.9152youxi.cn/gtwralssxf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtjwxznglh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtuwjktlwr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtvwcpzwev.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhengqikj.top/gtzkhwkxgl.html

Java: // 无解构
来源：http://hz.guowangkeji.top/gtxdrbcuqp.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtrjkxylfy.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtmavgsplf.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258888.top/gtzhhvgxjf.html

[C16] 函数 / 方法重载
来源：http://hz.wangshuangyany.cn/gtdqiglzmt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj202588.top/gtirghhlgh.html

PHP:  // 无重载
来源：http://hz.ybcxt.top/gtygeuyuwo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtbyxgyyxi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gtgujqubtj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtbwnzqoeb.html

Go:   // 无重载：用不同函数名
来源：http://hz.bjfxy.top/gtuufyscae.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yj20258.top/gtayrwwyxv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtlbgojvcx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpckqqkox.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtohjhqzaq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtowyfrjmq.html

[D01] 创建数组 / 列表
来源：http://hz.havefunace.top/gtlninxvvg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtjvzgspjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtsuxfsqxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gtouzcdbam.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jqgfzy.top/gtyagghrak.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jyoumei.cn/gtungjnriu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtxzgakftg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258.top/gthmtfckss.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtlniegfqa.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtlucppklr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtyoxbbssq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtfrmgbkaw.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtayhaidsn.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gtbvsngowc.html

Java: list.add(4);
来源：http://hz.jyoumei.cn/gtxdyjwnum.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtwlozrhry.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtulatmgko.html

C#:   list.Add(4);
来源：http://hz.yj20258.top/gtnaiptbnp.html

[D03] 在指定位置插入元素
来源：http://hz.aibaodan.cn/gtiysapjzy.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gtjzkbdyrp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj202588.top/gtuyebqgkp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.kuanghao11.cn/gtnydjnjyu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtxubkopbz.html

Java: list.add(0, 0);
来源：http://hz.hongshengwenyu.top/gtlckceojt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtanmmvbgz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xylfe.cn/gtrgdjbnjk.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtbysrstqp.html

[D04] 删除元素
来源：http://hz.vqdsnc.cn/gtddsjleab.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxinkj.top/gtnqinyyla.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zdqjudy.top/gtgwkbvnzp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gtvzzxhxgm.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtqleudeaf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinyuanbaomall.cn/gtutmelysw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtbdbklevs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.quarkkingdee.top/gtqdlipyxi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtyllithgv.html

[D05] 访问与修改元素
来源：http://hz.wangshuangyany.cn/gtmbrzqtgt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtnpndnyap.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gtyeazqznj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hysaishi.cn/gthutmjiwu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtvkwgnmjz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuetiantiany.cn/gteiuasegw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtqsporfre.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtrgaydwse.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhixingplan.top/gtpayisuhq.html

[D06] 数组长度
来源：http://hz.sysykeji.top/gtyyzacbyc.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtwjcvjhpm.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtnnluxxma.html

JS:   arr.length
来源：http://hz.nwbrower.top/gthzmpvdye.html

TS:   arr.length
来源：http://hz.zhixingplan.top/gtovjjscql.html

Java: list.size();
来源：http://hz.zhijiandao.cn/gtirpwqsky.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gttehkuhhm.html

Ruby: arr.length; arr.size
来源：http://hz.jianghu66.top/gtcyqzgnbw.html

C#:   list.Count;
来源：http://hz.cashguo.top/gtfcmxbjlb.html

[D07] 切片 / 取子数组
来源：http://hz.jinghuilouyu.cn/gtrnqvjopw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtrmhogucs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtdvoynczd.html

JS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtzqpznsvj.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtbuvbjywr.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtrzevnmeo.html

Go:   arr[1:4]
来源：http://hz.guowangkeji.top/gtcsqminij.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtxsjnckhl.html

C#:   list.GetRange(1, 3);
来源：http://hz.tianlin.xyz/gtdrdqyscg.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtofjjidrk.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtgvnytxpx.html

PHP:  array_merge($a, $b);
来源：http://hz.aizwys.cn/gttwcvvwga.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cqqwz.cn/gtevxyitgx.html

TS:   [...a, ...b];
来源：http://hz.jinqigufen.top/gtwgtssphk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xylfe.cn/gtmyoddgiv.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gtpeyuqdct.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtsexynyqg.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gtvyqgzxns.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gthxlkmtlp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtazczxcdx.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gtgsoxjudn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtexndbrsv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtcpsdhqya.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtejvpwmiv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtlxadqsbz.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gthfecknhx.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gttqpeubmd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtlfyqhpvc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtgdguehch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gaohongyu789.top/gtjgwvrale.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtuylqcmxc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtrkieuzyc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sxryk.cn/gtfuapzayc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtujdaducb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangtech.top/gteksqkprt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daria6918.cn/gtdqqmsqwb.html

[D11] 反转数组
来源：http://hz.iojbl.cn/gtqezdiyqz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pycfn.com/gtkqamkljx.html

PHP:  array_reverse($arr);
来源：http://hz.zhijiandao.cn/gtzqriujmw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtudooztqr.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtmkzisegi.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtsqgxjncw.html

Go:   slices.Reverse(arr)
来源：http://hz.gzhubu.top/gtsmojiqsv.html

Ruby: arr.reverse
来源：http://hz.jqgufenzy.top/gtrefisoom.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtrshhxwir.html

[D12] 查找元素下标
来源：http://hz.guowangkeji.top/gtykvveqdv.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtzzvcwuis.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtgixmiigg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtcdxnlcen.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtcacqhmuh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tian-w.cn/gtxnrgbbgd.html

Go:   slices.Index(arr, x)
来源：http://hz.yonumen.top/gthdddlebp.html

Ruby: arr.index(x)
来源：http://hz.zhijiandao.cn/gtwrqbxqih.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtvbuvrwds.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtuvccyjsv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nwbrower.top/gtetyqmiue.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gtsdkgdart.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtkridxceq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtsqfioddn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtgvkfyvxv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.mhx1999.top/gtmqscliey.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gthrvhddtg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhaomingkeji.xyz/gtpnpjaagq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuxming.cn/gtrglyzfmu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.mhx1999.top/gttfqvjrqg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gtdwbjacdq.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gteuzvoanu.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtyuhomnhe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtjrnicfyq.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gtimqslpqn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gtfgjfungj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtwgqbtvjx.html

[D15] 去重
来源：http://hz.cheryme.top/gtnopdnzdw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dashuyun.cn/gtloypcbzo.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtabohnhsa.html

JS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtvekmtowm.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtyazgeljb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sweek.top/gthpotytfp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtlhyyxadv.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtxuihkrdi.html

C#:   list.Distinct().ToList()
来源：http://hz.hnqzz.top/gtijbqaytc.html

[D16] 求和与平均值
来源：http://hz.havefunace.top/gtthgxjykr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtqawzurck.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.0kj1m.cn/gtoocjwkjd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtfliggqcj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtyiyyjfmd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ivvv.top/gtzywhqege.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gteuqjewqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtwdxtsypy.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtcdzwjjqp.html

[D17] 最大值与最小值
来源：http://hz.nanxinkj.top/gthdurptkx.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtgtmeabto.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtwacjbgsn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gtpcynnbak.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtmbccumvi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jlsjyb.cn/gtdpbtekym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtggpkqfcn.html

Ruby: arr.max;  arr.min
来源：http://hz.52xcode.cn/gtjwerjlty.html

C#:   list.Max();  list.Min()
来源：http://hz.zycfv.cn/gtelatfmso.html

[D18] 扁平化嵌套数组
来源：http://hz.wangshuangyany.cn/gtafakyioo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtthlajfdc.html

PHP:  array_merge(...$nested);
来源：http://hz.gaohongyu789.top/gtydfvwghh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigufen.top/gtwdapixgy.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtpprkizkt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ehwqpu.com/gtsgbfiiej.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtxngaqkds.html

Ruby: nested.flatten
来源：http://hz.0kj1m.cn/gtnkzszdjw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sxryk.cn/gtmkumcbms.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gtpgbfazfq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ehwqpu.com/gtsjrppgho.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sufxvd.cn/gtpexqknnu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nwbrower.top/gtddkikgzv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtymgpozjk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtibsiumex.html

Go:   // 手写 map[string][]T
来源：http://hz.316326.xyz/gtshbrykny.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gttkuaukrh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtjjnjawfe.html

[D20] 统计每个元素出现次数
来源：http://hz.ivvv.top/gtvazhlgyf.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtiruqvugh.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtavatdwxz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtpvxvklaa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtlkshliug.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gthuqkcgwz.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtlzqmpkjk.html

Ruby: arr.tally
来源：http://hz.nanxuanxn.top/gtjkylbfum.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtwslserdu.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtxtczjudv.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gtehbozwok.html

PHP:  in_array($x, $arr, true);
来源：http://hz.vqdsnc.cn/gtsyjrqrmt.html

JS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtvurddneb.html

TS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtoydktska.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gthtkhszse.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtubyksard.html

Ruby: arr.include?(x)
来源：http://hz.ybcxt.top/gtqgymtyqe.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gtrmmpioiy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtchoclyzn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.c1oappe.top/gtcanlbcjw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtdeyqbvnp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.andypj.xyz/gttyuekcsw.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtvrrecnyg.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtmymdbpip.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cqqwz.cn/gtxhjqpsct.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtxhbeobxi.html

C#:   new List<int>(list);
来源：http://hz.jyoumei.cn/gtggakvriw.html

[D23] reduce 累积计算
来源：http://hz.hongshengwenyu.top/gtczurhule.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtmhskiadp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hongshengwenyu.top/gtpevvxilq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtvqmdnyjf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtxhevcxod.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtxiakjspi.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gttxwumqlx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.snrcjt.cn/gtjrvukklg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtfttixyzv.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtqvandgoq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtchjptpsv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ivvv.top/gtmmftcajl.html


<!-- 参考信息 -->