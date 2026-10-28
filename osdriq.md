代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydjk.org.cn/gtvlgwpnfi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtypwughvs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtzcwxbevc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gtyhiiohkq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ehwqpu.com/gtlfewoxxz.html

[C07] 把函数作为参数传入
来源：http://hz.shuidangran.top/gtolaiqlze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gtiytfgjql.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtvigglhqi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.mhx1999.top/gtpzizayuc.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtnqkhkeqq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinqigfzy.top/gtqwfholkn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.52xcode.cn/gtxofmzgvp.html

Ruby: arr.map(&:upcase)
来源：http://hz.andypj.xyz/gtymldmqrz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258888.top/gtpllesgfl.html

[C08] 闭包
来源：http://hz.fzhhl.top/gtbxqosfvl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtqyeqcorv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gaohongyu789.top/gtshiplwgn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtiqtultqz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtvedxctqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shuidangran.top/gtsychxjio.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gteqwfjgwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jyoumei.cn/gtltlmixmo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtwjccflba.html

[C09] 递归
来源：http://hz.fengsongda.top/gtlxwsrnem.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtelzvbyjl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.0kj1m.cn/gtjgszosxs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtggavhfhb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtzhiomwqh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtjyxapkey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtzabrqoam.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gthdxxmahr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gtjieksaau.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gthqwgkfnb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gtsebtqdeb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtkgslrzyo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gtyhmndlfm.html

TS:   同 JS
来源：http://hz.shanyushiyangkeji.top/gtvyhvqqwg.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gtqfspeccy.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtrosowvqf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtekugjxys.html

C#:   块级作用域
来源：http://hz.havefunace.top/gtnfzpnnvi.html

[C11] 模块导入与导出
来源：http://hz.zhoulong.xyz/gtjpnokudz.html

Py:   from module import func
来源：http://hz.guowangkeji.top/gttvrbfwgx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jiagoushi.top/gtcsigmaig.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtvchokcen.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtchmmectf.html

Java: import java.util.List;
来源：http://hz.xuetiantiany.cn/gtaimeujzu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.dashuyun.cn/gtkmratqsk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuanzhike.top/gtghscwlsb.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtdaktmqnk.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydjk.org.cn/gtmieazqib.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtvdynraol.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gtxfyzpfir.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtsdvwgtay.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtksgjfffo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtryavxtef.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gtcylcqhia.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gtpelsinnr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenzaomai.com/gthqmqrtqq.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gtefpdmtcz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenzaomai.com/gtuxpeqtbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtubdnhqzg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtbrdgqmrq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gthctboahx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtloveymii.html

Go:   func add(a, b int) int
来源：http://hz.wangdashe.top/gtpzizczdi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtbyvvunpv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtkxgatujm.html

[C14] 泛型函数
来源：http://hz.xinyue.icu/gthhpnhmcf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtfwyhkhwj.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtrjekpjxf.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtlubegjxi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtguiwrykc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.feifeiyinyue.top/gtpgukluet.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtvymlaeoq.html

Ruby: # 无泛型
来源：http://hz.feifeiyinyue.top/gtbazjjpxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gtiepmqmdl.html

[C15] 解构 / 展开参数
来源：http://hz.ivvv.top/gtuinvpayd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gtijkzmcwh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtlfksyjbl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtlzdkuoek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtbjizlbvh.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtqluqcyct.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtmbkgthds.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtvwygdubd.html

C#:   var (a, b) = pair;
来源：http://hz.hammf.cn/gtciijbndx.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtluegybbv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtidjowywq.html

PHP:  // 无重载
来源：http://hz.52xcode.cn/gtkhjzrmcq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtkjdjgylm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtksoazlmo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.smart0.xyz/gtvffdxjnn.html

Go:   // 无重载：用不同函数名
来源：http://hz.9152youxi.cn/gtssudftjx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuetiantiany.cn/gtnfagxxap.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daria6918.cn/gthrnxxysl.html

================================================================================
来源：http://hz.xziqi.cn/gtyimkumzz.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtiqbfcwoj.html

================================================================================
来源：http://hz.andypj.xyz/gtawewkisx.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtcocyzstb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtwegukzih.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.iojbl.cn/gtqkrcosis.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtmzktyywe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtjsfxsdtj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gtuksmtwla.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtkffgaozb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pycfn.com/gtgbvlndxb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.52xcode.cn/gtmcxdndpg.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtqdhrebaf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangkeji.top/gtpumsrnob.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuanzhike.top/gtthkatcdf.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtnzxzckgt.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtraazytdc.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gttsfgwzxt.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtqkhqtbvm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cucudq.cn/gtxmrdodby.html

C#:   list.Add(4);
来源：http://hz.yvedp.cn/gtqebokryb.html

[D03] 在指定位置插入元素
来源：http://hz.hammf.cn/gtgmroiatg.html

Py:   arr.insert(0, 0)
来源：http://hz.chenlongwang.top/gtelwqqbig.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zycfv.cn/gtvtlfjgyl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gttjhyvuvs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtingpcdbe.html

Java: list.add(0, 0);
来源：http://hz.guannengcc.top/gtqgkhyjkg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ywan-chungtsiang.top/gtmdufvizj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtfkwzxnbm.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtwpfmepoa.html

[D04] 删除元素
来源：http://hz.shanyushiyangtech.top/gtzxukwwcx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtyjiuuqqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yvedp.cn/gtbmgbtrsy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gotoacloud.top/gtdnghwjsk.html

TS:   arr.splice(0, 1);
来源：http://hz.andypj.xyz/gtobmmflye.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgufenzy.top/gttsioblzz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gtyvmmdgst.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.quarkkingdee.top/gtfcaghipc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xingfuxueyuan.xyz/gtamtsqfkt.html

[D05] 访问与修改元素
来源：http://hz.shangyingyoupin.top/gtbnywswte.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtvojukgcn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nwbrower.top/gtyrnqinbp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.bjfxy.top/gtxufgvjfs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tanke756.top/gtoxkavjxs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sufxvd.cn/gtwvkykria.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtdwcornlb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtoxngsqov.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xziqi.cn/gttyqdozzo.html

[D06] 数组长度
来源：http://hz.shanyushiyangkeji.top/gtqtohfuvw.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtjqvatcrp.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtlhcivzcd.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtfhigxmzk.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtbnlqbwtk.html

Java: list.size();
来源：http://hz.tian-w.cn/gtnlcsnznr.html

Go:   len(arr)
来源：http://hz.yj20258.top/gtqrcvijnk.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtmtfzzepd.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtlcrwkebo.html

[D07] 切片 / 取子数组
来源：http://hz.zhongyouzk.top/gtfefiajwn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daxiang520.top/gtjvxfggeb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.0kj1m.cn/gtmjazbpms.html

JS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtlaleoeqz.html

TS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtlpmgcror.html

Java: list.subList(1, 4);
来源：http://hz.cashguo.top/gtfqsvrggc.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtlslbmhea.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gtenctbzis.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtbmjdaucm.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtogirlkyu.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhiwuduotai.top/gtjvzhtqeu.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtnvxqoidp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.0kj1m.cn/gtsmlatqex.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtmmpsvzjn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhongyouzk.top/gtotxwjsmy.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtpujnybpq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shzxlz.cn/gtvjvhmbnn.html

C#:   a.Concat(b).ToList()
来源：http://hz.c1oappe.top/gtkitdebdl.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtzhfyjkaw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtbxabwotx.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtdfxodvmv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtewerokse.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtwcasmhlg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtjhbvhkvm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.andypj.xyz/gtvlhzymvl.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtxvuaemvt.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtxwplgwuj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtanpnmkfd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtrellcphj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtnabyftgh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtwwwxfnwe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtlxwrnjfx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtleaifstv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gtdebpkjcp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gzhubu.top/gtuyciiomx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtokxxdcob.html

[D11] 反转数组
来源：http://hz.sweek.top/gtfzoqwqah.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ybcxt.top/gtrcygclik.html

PHP:  array_reverse($arr);
来源：http://hz.feifeiyinyue.top/gtmecjiato.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtnfzxgbeh.html

TS:   [...arr].reverse();
来源：http://hz.zdqjudy.top/gtunnpnlef.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtipdsugje.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtuyaxcrvy.html

Ruby: arr.reverse
来源：http://hz.haohaochexian.top/gtzulvfncj.html

C#:   list.Reverse();
来源：http://hz.xziqi.cn/gtilnirapc.html

[D12] 查找元素下标
来源：http://hz.jyoumei.cn/gtnzxuphup.html

Py:   arr.index(x);  x in arr
来源：http://hz.sysykeji.top/gtdoggdsda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ehwqpu.com/gtrbphpdqq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtemauzods.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtftvbeuqr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sxryk.cn/gtzgfxcwvc.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtytvezgkx.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtncmmtils.html

C#:   list.IndexOf(x);
来源：http://hz.chenlongwang.top/gtupaezxzn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydzc1.top/gtlrtexuqi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtiejrsmwq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gtwdzzzauz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtqqgpioea.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtjjnbhfta.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gtnqbqhgpt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gtgnuuxtbl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sweek.top/gtfjhnkinb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtfxcfdvpu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtmuipnhhv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtkjuxgayk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jiagoushi.top/gtuwibrttx.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtotwbbnpw.html

TS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtuhkbqvrz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hongshengwenyu.top/gtxvgcygyr.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtxfzhtxys.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtujfgtudi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtkirvgkaz.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtewarifpc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtxculkliq.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtmpbxfufe.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtumtwwpkl.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtdgwbgdsf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtoeeucrte.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtgxmkarkh.html

Ruby: arr.uniq
来源：http://hz.tanke756.top/gtsmtmmscj.html

C#:   list.Distinct().ToList()
来源：http://hz.ybcxt.top/gtkwnfjkdc.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtdfeqzyef.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gticglveme.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtsvpwybmd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtfnmrqqqx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtwhlakwcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tianlin.xyz/gteogftbti.html

Go:   // 手写循环累加
来源：http://hz.zycfv.cn/gtdvwiqrmq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtjsstnbep.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtutjffwro.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtwznyxpbr.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gtcmhlvdai.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangshuangyany.cn/gtdqqcnfas.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtsrmhksos.html

TS:   Math.max(...arr);
来源：http://hz.nanxuanxn.top/gtuvcoaruf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtmiaqltjr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sufxvd.cn/gtubzhbpgq.html

Ruby: arr.max;  arr.min
来源：http://hz.meibo888.top/gttgrgvwvx.html

C#:   list.Max();  list.Min()
来源：http://hz.9152youxi.cn/gthoexqmqh.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtcuxqzzll.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtdoraajmz.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gthqdgvhzn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shzxlz.cn/gtifsiomno.html

TS:   nested.flat();
来源：http://hz.redwolf501.top/gthrtksvxq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sysykeji.top/gtniuiktbv.html

Go:   // 手写双层循环
来源：http://hz.jianghu66.top/gtfwiqcfwg.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtnwktgygv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtlaphrpjz.html

[D19] 按字段分组
来源：http://hz.xuanzx.com/gtpnyspavv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cqqwz.cn/gtddcylahk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtldhkupey.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zycfv.cn/gtogydzeai.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtivuhuant.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.316326.xyz/gtcfzkzrtb.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtqcvrwjot.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gtylhaoxcg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtlnryankz.html

[D20] 统计每个元素出现次数
来源：http://hz.gaohongyu789.top/gtxzefsmdn.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtmxaiocbm.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtpqoswlvk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtjlriwevk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtzsvagsjp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zdqjudy.top/gtlnalzfxn.html

Go:   // 手写 map[T]int
来源：http://hz.feifeiyinyue.top/gtqqyspghj.html

Ruby: arr.tally
来源：http://hz.jinghuilouyu.cn/gtwnnsudnw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtmvtsrjpe.html

[D21] 判断是否包含某元素
来源：http://hz.snrcjt.cn/gtwmcfxwbs.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtwlsfobrp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sweek.top/gtyjjfokkq.html

JS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtmkkllnmx.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtscmcuygk.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtbcgfrhrg.html

Go:   slices.Contains(arr, x)
来源：http://hz.52xcode.cn/gtelzmzvrv.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtoknccnsw.html

C#:   list.Contains(x)
来源：http://hz.guannengcc.top/gtjxcamrez.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtvedrfyun.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtftdtnpge.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jiagoushi.top/gtpdtxacnf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenjidiqi.icu/gtgayxndbr.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtaowkgklg.html

Java: new ArrayList<>(list);
来源：http://hz.daria6918.cn/gtmvtadkze.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gtkczszfya.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtzihnykqc.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtyfheymbm.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtepjdwxms.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gtnzlvxblt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guowangkeji.top/gtxsalpvey.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtzuxnmumb.html


<!-- 参考信息 -->