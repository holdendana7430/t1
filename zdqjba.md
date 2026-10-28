代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhoulong.xyz/gtcehuvwvt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.birdmap.top/gtwrqlnhoe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnxiangtu.top/gthxkibotq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gtqehwttgk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtarniwziq.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gtvhdfowai.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sufxvd.cn/gtqanqfmjm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtrlcnlysi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.vqdsnc.cn/gtfnjbdkrf.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtthdtssff.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtqtehnjgp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gtbnovvodg.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangdashe.top/gtdmjwyaih.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gtfgfyfjjv.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtnkvivsvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxinkj.top/gtbiikrhab.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtgswjjjfc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gthitamnio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtnlubevla.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtmehuglup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gzhubu.top/gthkfwivjc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtxemrmvjp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtcxlbgwyf.html

[C09] 递归
来源：http://hz.mhx1999.top/gtsgjnlvov.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hammf.cn/gtjdjnmnwg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtzpjanuga.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtgtpgbhic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtdndbmtlg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sweek.top/gtudeoxglo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sweek.top/gtyqndjklq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.iojbl.cn/gtfyyqbdmd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gtlletwrzk.html

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtwnoaeavd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhoulong.xyz/gtytmsfssy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj202588.top/gtphomqbsk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sweek.top/gtqhjxiieq.html

TS:   同 JS
来源：http://hz.birdmap.top/gtnocpdyvw.html

Java: 方法内为块级作用域
来源：http://hz.svipenyu.cn/gthehupchk.html

Go:   花括号块级作用域
来源：http://hz.jinqigfzy.top/gtlgxzwhkk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydzc1.top/gtlqnnwpzm.html

C#:   块级作用域
来源：http://hz.yj202588.top/gtqnqdqzdb.html

[C11] 模块导入与导出
来源：http://hz.ppjwa.cn/gtwtrbdtwv.html

Py:   from module import func
来源：http://hz.svipenyu.cn/gtqvsbunli.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtgdscxakr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cqqwz.cn/gtvybbxako.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtksluiscs.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtzuybjpnj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangdashe.top/gtciqjlhac.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yongpay.top/gtdyytmvzh.html

C#:   using System.Text;
来源：http://hz.zdqjudy.top/gtsnhmgzkk.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gttnfvoiwl.html

Py:   (lambda: print("run"))()
来源：http://hz.chenlongwang.top/gtqhtjozyx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtzdvyvlvx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gthypbjfzs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtthllzkds.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aibaodan.cn/gtwmyeokvp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhixingplan.top/gtjtydeqge.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtaezwwmhj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigfzy.top/gtzkeytxso.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtaevdttcy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtiuojkwtr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtmimqkwkn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtwjxqegtw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtbbixurjp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtyuwbnlwp.html

Go:   func add(a, b int) int
来源：http://hz.pycfn.com/gterlhleau.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yanxiufei.cn/gtflcvkwyw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtxksjntad.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtjqhkvenj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuanzhike.top/gtnmjqzedv.html

PHP:  // 无泛型
来源：http://hz.gogol.net.cn/gtgdqnelyf.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gthronfzcw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtwwaclbgp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhiwuduotai.top/gtdntywqds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtjvtqvfxw.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtidjhhxsc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gtvvecwnkz.html

[C15] 解构 / 展开参数
来源：http://hz.chenjidiqi.icu/gtcwxxjdzk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtyatkkmkp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinyuanbaomall.cn/gtedobrqqx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtobfhevnj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtbcynylen.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtnumblxyj.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtirqovrkd.html

Ruby: a, b = pair
来源：http://hz.zycfv.cn/gtedzhxilk.html

C#:   var (a, b) = pair;
来源：http://hz.52xcode.cn/gtmuiikgqs.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gttjotfxul.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtersaydeo.html

PHP:  // 无重载
来源：http://hz.tian-w.cn/gtzbxzzaro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jlsjyb.cn/gtfdnoupiv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtfycacikq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.mhx1999.top/gthokdfjie.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gtzuzuivig.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hongshengwenyu.top/gtrqvbocxz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtimmdgrvp.html

================================================================================
来源：http://hz.xinyue.icu/gtwmaotykj.html

D. 数组 / 列表 / 集合
来源：http://hz.gotoacloud.top/gtqubotexp.html

================================================================================
来源：http://hz.hysaishi.cn/gtfrekdbbg.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtjnxhxhil.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gtipkftuiu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnxiangtu.top/gtcieyvgkx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tianlin.xyz/gtzfgwocpk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuanzx.com/gtvrvdfueu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ppjwa.cn/gtzxafwutz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gtetnolljj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ehwqpu.com/gtopwpevtk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhongyouzk.top/gtacvdnbdt.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtquixinqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtwnueeujv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtvtbafaqi.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gtjtqrpvou.html

TS:   arr.push(4);
来源：http://hz.guowangkeji.top/gturgcvimr.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtokptbmvh.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gttkoidwcu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtxvtgpiui.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtwlqfawih.html

[D03] 在指定位置插入元素
来源：http://hz.xinyue.icu/gtumqpmpku.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtiimsvhig.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuanzhike.top/gtygjkrrxk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenjidiqi.icu/gteucqxqze.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gtjlclpqsb.html

Java: list.add(0, 0);
来源：http://hz.shzxlz.cn/gtoyfviava.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtzdfplrcu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ehwqpu.com/gtolnxfepv.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gthewxuqfs.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gtisnxskxy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtyqnvslhf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtngowxdxk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.52xcode.cn/gtktxikhmm.html

TS:   arr.splice(0, 1);
来源：http://hz.xuanzx.com/gtwjdhfgku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yangfankeji.com/gtwvulwkbr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinyuanbaomall.cn/gtnchdaxgw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtvvjwwkmi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gthdgejyew.html

[D05] 访问与修改元素
来源：http://hz.hfpthk.cn/gtoibtibwc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtrggamjij.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtrvvyqoca.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtblsiaudu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fzhhl.top/gtwgmnmxqp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cheryme.top/gthumjkfzk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fzhhl.top/gtnkwrpswp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtjwadehyw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtjngwlkmv.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtidvxlyuc.html

Py:   len(arr)
来源：http://hz.dianchejie.cn/gtrgxdesvw.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gtdpugiswx.html

JS:   arr.length
来源：http://hz.jinqigufen.top/gtllhhrbxb.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtqwyrbyoo.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtjtnhmqye.html

Go:   len(arr)
来源：http://hz.hywenlv.cn/gtootjrqgs.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtywvccrva.html

C#:   list.Count;
来源：http://hz.316326.xyz/gtvxjxnfoq.html

[D07] 切片 / 取子数组
来源：http://hz.redwolf501.top/gtrsdqecwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xingfuxueyuan.xyz/gtirmuzupl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtbyhxsbqv.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtvinkielv.html

TS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtczorfrlp.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtnuoevxxy.html

Go:   arr[1:4]
来源：http://hz.mhx1999.top/gtjbuxsfst.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gthphhjlax.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhijiandao.cn/gtyujthaty.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtchdqxizv.html

Py:   a + b;  a.extend(b)
来源：http://hz.guowangkeji.top/gtilmxfgrh.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtzubrtnar.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.bjfxy.top/gtrueypsya.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtjwdszdvf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtvcabjizi.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtpsjicurh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtwwekdnmf.html

C#:   a.Concat(b).ToList()
来源：http://hz.cashguo.top/gtbctushvq.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gtxvurlpcz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gttcflixdr.html

PHP:  sort($arr);
来源：http://hz.jianghu66.top/gtlebfitma.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtumaonmfj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtaylndhun.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtjajskfts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtnpfyvmka.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtvifavbac.html

C#:   list.Sort();
来源：http://hz.fengsongda.top/gtcbgytbrg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gtpxqrtkxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtzpztycal.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtohdxazfi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtuszkfhdn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gtlqallphh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtugafijco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gttndyezdj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtpjmwsfqy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtjsiymria.html

[D11] 反转数组
来源：http://hz.yuxming.cn/gtrdanmwgq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cqqwz.cn/gtljhsrqub.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigufen.top/gtacnccgcn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhongyouzk.top/gtvexapqul.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtlpkntqmf.html

Java: Collections.reverse(list);
来源：http://hz.hongshengwenyu.top/gtkwitwmnl.html

Go:   slices.Reverse(arr)
来源：http://hz.zhongyouzk.top/gtpabdlewr.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtzjfkovpk.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtsbmxrntq.html

[D12] 查找元素下标
来源：http://hz.gogol.net.cn/gtanebhyyr.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtxjycfnlh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtxzyrorkx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gtviavimsf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtgiedqrzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gtcctiseil.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtyvfnyqux.html

Ruby: arr.index(x)
来源：http://hz.ehwqpu.com/gtrraozdug.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtonebzrct.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtxxjmqjts.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.vqdsnc.cn/gtjxshakjf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cheryme.top/gtowjnoijn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtihueywoh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtvbherhyz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sysykeji.top/gtaxyjnuqt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.mhx1999.top/gtdngaiaau.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtmyaufxxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtqwyhzmze.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gtrvaqobuf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgfzy.top/gticbicpjl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtakszlmmy.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtkksmmead.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gthcbaibeo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtourszrhb.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtsxulhdkf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhixingplan.top/gttexleaqu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gtohfwliyc.html

[D15] 去重
来源：http://hz.fzhhl.top/gtfbaaqnuq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtcasqzvod.html

PHP:  array_unique($arr);
来源：http://hz.jiagoushi.top/gtsfmnslez.html

JS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtmzhrcitz.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtzwchlxbq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gthrlwchhe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.birdmap.top/gtmhpmkaiz.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtmeufqdcu.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtpwmfdrrt.html

[D16] 求和与平均值
来源：http://hz.gotoacloud.top/gtjtiavaak.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtecpgskcs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtiqiunnuf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtzlcqkgkm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtskqpoafe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ehwqpu.com/gtjncbjdsi.html

Go:   // 手写循环累加
来源：http://hz.yj202588.top/gtnamsbrys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtaoppnjgk.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtpzctayte.html

[D17] 最大值与最小值
来源：http://hz.mhx1999.top/gtaabxtfiw.html

Py:   max(arr);  min(arr)
来源：http://hz.yanxiufei.cn/gtyxnubedy.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenjidiqi.icu/gtaadpbjsd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtyawksuld.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtthqncsbq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gtlenxtaiy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtugivdutp.html

Ruby: arr.max;  arr.min
来源：http://hz.hfpthk.cn/gtrzgxhcil.html

C#:   list.Max();  list.Min()
来源：http://hz.zhoulong.xyz/gtrkadujbl.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtkzhhvcuk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinyuanbaomall.cn/gtmurkgydi.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxuanxn.top/gtvqammulu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtqoxpatfe.html

TS:   nested.flat();
来源：http://hz.ehwqpu.com/gtrzuruttk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sysykeji.top/gtfiqztwqu.html

Go:   // 手写双层循环
来源：http://hz.mhx1999.top/gtwhjhujij.html

Ruby: nested.flatten
来源：http://hz.ivvv.top/gtulbrthoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtmgzjzbwb.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtbnjukmji.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gtwcdwepny.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydjk.org.cn/gtqsvrdtjf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtzgamywie.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tianlin.xyz/gttymudivl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtnlixcwsy.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtkqbtrrtu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.snrcjt.cn/gtiglhfrzl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtsncasoow.html

[D20] 统计每个元素出现次数
来源：http://hz.havefunace.top/gtwqaxmeyw.html

Py:   Counter(arr)
来源：http://hz.daria6918.cn/gtrbeipwnc.html

PHP:  array_count_values($arr);
来源：http://hz.hywenlv.cn/gtzyfjvdyf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtxmdvluhk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtyruhehtl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jiagoushi.top/gtyqdbfexh.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gtlgqsudzi.html

Ruby: arr.tally
来源：http://hz.yonumen.top/gtnjspqjbc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtnugytoju.html

[D21] 判断是否包含某元素
来源：http://hz.daria6918.cn/gtrdkjravy.html

Py:   x in arr
来源：http://hz.zycfv.cn/gtyyuzzwek.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shzxlz.cn/gtajtdvgrs.html

JS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gteaoipxyx.html

TS:   arr.includes(x)
来源：http://hz.bjfxy.top/gttstwxtnh.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtunvommgl.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtknuifncw.html

Ruby: arr.include?(x)
来源：http://hz.chenzaomai.com/gtadasfqhz.html

C#:   list.Contains(x)
来源：http://hz.guannengcc.top/gtfwgrsdlm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtlmkqswmn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtxxecevbv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yongpay.top/gtrsxcgvsm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtiplquauy.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtzcciycws.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtlahgmhtt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtlnkhlksp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gtnzyglpta.html

C#:   new List<int>(list);
来源：http://hz.sysykeji.top/gtnznsfepo.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangtech.top/gtjgycesco.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pycfn.com/gtjogcsbhb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtacjrjaft.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtoorcfwym.html


<!-- 参考信息 -->