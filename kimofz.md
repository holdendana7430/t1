代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nwbrower.top/gtpdhtgzbi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gtpnubcqbv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtrloprbub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtccafwbmi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtmmznkfll.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.aibaodan.cn/gtygagxwfy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gthgqhtint.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtxetjmnty.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtpziwhfbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xziqi.cn/gtxywbrzfq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtuajekkhq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnxiangtu.top/gtydvodzop.html

TS:   同 JS
来源：http://hz.vqdsnc.cn/gtmppxoean.html

Java: 方法内为块级作用域
来源：http://hz.ywan-chungtsiang.top/gtwflbxyax.html

Go:   花括号块级作用域
来源：http://hz.chenzaomai.com/gtuonfetzf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sysykeji.top/gtdtoxxnqn.html

C#:   块级作用域
来源：http://hz.cucudq.cn/gtghoesckl.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtuimtvspj.html

Py:   from module import func
来源：http://hz.guannengcc.top/gtyngrxuln.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnxiangtu.top/gtunqlpsze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xylfe.cn/gtnritmjpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pengpengdd.cyou/gtcwbonypx.html

Java: import java.util.List;
来源：http://hz.nwbrower.top/gtmfftoqft.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tianlin.xyz/gttygynzle.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangshuangyany.cn/gttwocnhat.html

C#:   using System.Text;
来源：http://hz.ybcxt.top/gtjjltpgdn.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxuanxn.top/gthcotmbmj.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigfzy.top/gtokhvejzq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtmpmxdmtk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtqxtnwpiz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtbkrozyey.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.mhx1999.top/gtyrhvjagf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtvvtcitap.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtrvagzwrm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gthdaeyrjm.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhixingplan.top/gtkbzimaip.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtkxbtncaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gthtutpkhu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gotoacloud.top/gtavqumbhy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtxahpkquy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtlalydjnf.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtovxoivnq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tian-w.cn/gtxatjhkiw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yonumen.top/gtlqfiwbhd.html

[C14] 泛型函数
来源：http://hz.ivvv.top/gtjqkmuttv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtvybvfyud.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtvyvkyfrr.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtttliakib.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtyoxsqhcn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gttwlcswmb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuetiantiany.cn/gthqgeyoqs.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtmsbqloyo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigufen.top/gtovojayqd.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gtznhlwsxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtzanbwufd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtbdcspzkr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gthrfcyvqk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtapaoqahu.html

Java: // 无解构
来源：http://hz.jinqigufen.top/gtkgsphyow.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gthjntpbsh.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtslkylcvf.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtfvlvpwtg.html

[C16] 函数 / 方法重载
来源：http://hz.sxryk.cn/gtbcfvqcza.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtpnowrjmg.html

PHP:  // 无重载
来源：http://hz.zycfv.cn/gtjocpcurt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtswjmiyek.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtxdfovikt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtvaezjwmb.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtruzbxjrx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtdjrlnduc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.52xcode.cn/gtinyjobun.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtkpvubabe.html

D. 数组 / 列表 / 集合
来源：http://hz.ehwqpu.com/gtvmqhqzky.html

================================================================================
来源：http://hz.wangdashe.top/gthamdikly.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gthvrtpbix.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydjk.org.cn/gtdbtcqbuk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtzfryqvag.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hfpthk.cn/gtloistpyz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhijiandao.cn/gtqoiwxbqw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yanxiufei.cn/gthtrrovfg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.0kj1m.cn/gtjouitaba.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gtmngzhzqu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.andypj.xyz/gttefagajm.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtughzxeap.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigfzy.top/gtkxkrhydr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gteqpjdcrw.html

JS:   arr.push(4);
来源：http://hz.daria6918.cn/gtnolfvgbp.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gttasvnars.html

Java: list.add(4);
来源：http://hz.xziqi.cn/gtumskerjq.html

Go:   arr = append(arr, 4)
来源：http://hz.daxiang520.top/gtybyxmhas.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sysykeji.top/gtvgexmghk.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtpsrxtlwc.html

[D03] 在指定位置插入元素
来源：http://hz.hammf.cn/gttsocvaon.html

Py:   arr.insert(0, 0)
来源：http://hz.tianlin.xyz/gtvcukdjlu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jyoumei.cn/gtmnwepyse.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gthiaqljoa.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.c1oappe.top/gteyadlwwv.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtocmlhyzc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zycfv.cn/gtpypjimls.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gtqlpzrzfo.html

C#:   list.Insert(0, 0);
来源：http://hz.iojbl.cn/gtvetnugsv.html

[D04] 删除元素
来源：http://hz.sxryk.cn/gtjkwmzzwl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtjbckskru.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dashuyun.cn/gtwqocenkh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuetiantiany.cn/gtkmfidbop.html

TS:   arr.splice(0, 1);
来源：http://hz.ydjk.org.cn/gtlfnuojaz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258.top/gtukjgvypf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtttuvdywi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtdhermhum.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgufenzy.top/gtkeufopoz.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtprnsbive.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtrxzdndna.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gttsgyqtad.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cucudq.cn/gtcskwlkzk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gttskyqekh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangshuangyany.cn/gtpwvvhscj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtplpnbdcb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtsomirhja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.meibo888.top/gteouuxeqq.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtcnldpjty.html

Py:   len(arr)
来源：http://hz.yongpay.top/gtbmbhzeot.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtnuqnaorw.html

JS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtigqtuaqf.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtxwgutmqt.html

Java: list.size();
来源：http://hz.tanke756.top/gtnkydjzga.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtwnjuvnog.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtjcmzmbbn.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtoqgzzqrh.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gtqezlznms.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.svipenyu.cn/gtoduwqwny.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtitqalduh.html

JS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gthfuvzxzj.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtjdpberji.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtvqfezvrp.html

Go:   arr[1:4]
来源：http://hz.yanxiufei.cn/gtlyvgqynb.html

Ruby: arr[1, 3]
来源：http://hz.havefunace.top/gtkgdpreuw.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuanzx.com/gtypwzzcba.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtjyilpyae.html

Py:   a + b;  a.extend(b)
来源：http://hz.52xcode.cn/gtrclgybbv.html

PHP:  array_merge($a, $b);
来源：http://hz.chenlongwang.top/gtzpyttddg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gtiyowwhyk.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtqrlaakeb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtbusrlrmm.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtfxvrrbui.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gtwszpcpag.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtodvytrqv.html

[D09] 排序（升序）
来源：http://hz.andypj.xyz/gtdzqkwusl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtrrebqhiv.html

PHP:  sort($arr);
来源：http://hz.yueranfly.top/gtqrnbqzzd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hywenlv.cn/gtezwkkzsu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gogol.net.cn/gtpfzbjlcc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jianghu66.top/gthztfkzzc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xziqi.cn/gtowiiyafa.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtkrwifkld.html

C#:   list.Sort();
来源：http://hz.jqgfzy.top/gtggxavanl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tian-w.cn/gtszotojxe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtkerzrmqk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtdtqxpjgv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gtnowlnlgb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtyngsjumf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hysaishi.cn/gtjrpraijc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtzctpwdyz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangdashe.top/gteofdistw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xingfuxueyuan.xyz/gtwpwnszmg.html

[D11] 反转数组
来源：http://hz.ywan-chungtsiang.top/gthjlunlxc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gaohongyu789.top/gtqlfbdxzk.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtzvmxybpm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.havefunace.top/gtbpdfjdrk.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtyhrmmfhr.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtoqfhkivy.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gthoyfzdqf.html

Ruby: arr.reverse
来源：http://hz.yvedp.cn/gtgxtpzoof.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtcntlysmv.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtmwavjnfe.html

Py:   arr.index(x);  x in arr
来源：http://hz.guowangkeji.top/gtwslyiwab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtoamfnowi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtbjmidghi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtvwhiqaxj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ybcxt.top/gtistdoraw.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gteviidngu.html

Ruby: arr.index(x)
来源：http://hz.xziqi.cn/gtcywbyrmf.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtawguzing.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gtnbrvmumf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtuegszbja.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtjjmsdjab.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtyxrvawsc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtwzbfqbuj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangshuangyany.cn/gthtihjoid.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtorpqkjmo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pengpengdd.cyou/gtplfasslr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxuanxn.top/gtvftyicpp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtnttzjmgc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gtdydgbhcy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gthxkptolj.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gteaqrrsej.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtgmhaipmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtzbjyvzpp.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtkrzgrzhb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gttucgtilq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtrmqouuze.html

[D15] 去重
来源：http://hz.hammf.cn/gtldadjpeh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtobqvvjca.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtdnwpgapw.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtwyuhenzb.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gthxfcqtlp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgufenzy.top/gtltwflhbm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtgacuhgyi.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtvotclccp.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gtjjcayszm.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtfvdeaall.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtneeumrva.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtqtgdjqzs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtglusbvod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtvugqhjdd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.iojbl.cn/gtxdxtktet.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gthvbndwfv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtpantfmiq.html

C#:   list.Sum();  list.Average()
来源：http://hz.ppjwa.cn/gtiuiyayxb.html

[D17] 最大值与最小值
来源：http://hz.vqdsnc.cn/gtlgydompv.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtzrljnedb.html

PHP:  max($arr);  min($arr);
来源：http://hz.pengpengdd.cyou/gtocvaenwm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtztanbouh.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtzyaolzwo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhengqikj.top/gtbrucfdvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtxxeaolcr.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtwscouzxg.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtuhfnmuvu.html

[D18] 扁平化嵌套数组
来源：http://hz.shzxlz.cn/gteattzebs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gtbbpaqiao.html

PHP:  array_merge(...$nested);
来源：http://hz.yongpay.top/gtvuycggfv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydzc1.top/gtcwfooino.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtvxbppdmq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtyfiqvgyj.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtrbfjemge.html

Ruby: nested.flatten
来源：http://hz.jianghu66.top/gtcklmdaxr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.wangshuangyany.cn/gtcuffdawn.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gtczqxdmzc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtyhsapzcf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gttlubtoav.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtbjjwgsws.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtzcgwoulx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtbqcdecvb.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtkjwswwic.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtegtzkcde.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtpfavwxrd.html

[D20] 统计每个元素出现次数
来源：http://hz.cdnleiting.top/gttxmsccrk.html

Py:   Counter(arr)
来源：http://hz.yj202588.top/gtkigihdlf.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtuxymmhzj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtxtdutdby.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtdynnbymn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sysykeji.top/gtqikmzuea.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gttzhzqlbs.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtdgywsnxp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dianchejie.cn/gtwvdgjfer.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtjsudxhdh.html

Py:   x in arr
来源：http://hz.hysaishi.cn/gteykxzrgu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigufen.top/gtgolctqqm.html

JS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtvtnsfhci.html

TS:   arr.includes(x)
来源：http://hz.yj20258.top/gtcodnmwlr.html

Java: list.contains(x)
来源：http://hz.shanyushiyangkeji.top/gtsrrsftun.html

Go:   slices.Contains(arr, x)
来源：http://hz.sxryk.cn/gtknolscqk.html

Ruby: arr.include?(x)
来源：http://hz.yuanzhike.top/gttxrkfnpd.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtljjktupk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yangfankeji.com/gtnwawneyy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gttwhmheql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtdcyqtyzb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtifztyjcn.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtejfgdapq.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtllyzjoom.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtkpkvouxt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gttcimkmsd.html

C#:   new List<int>(list);
来源：http://hz.yj20258888.top/gtcsabqoti.html

[D23] reduce 累积计算
来源：http://hz.ywan-chungtsiang.top/gtghtlcewc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fengsongda.top/gtxeilijpa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuanzx.com/gtujkhftfl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtbnjfjucf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtoqjxnkev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtuaxbzrio.html

Go:   // 手写循环
来源：http://hz.smart0.xyz/gttzyfrqez.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtyphhcotq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtaemarrka.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gtcxqagjzs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gtdurubkph.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxinkj.top/gtntoxefyt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtlvbavvau.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.bjfxy.top/gthjvrdqgp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtdpicnmuw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtyopaihmf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gtjiosecfy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xziqi.cn/gtzksnbymn.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxinkj.top/gtbdsidxfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xingfuxueyuan.xyz/gtcyesslbv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yanxiufei.cn/gtdilaheil.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zdqjudy.top/gttysikmfg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.smart0.xyz/gtcyquzmyz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtbuydauey.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangtech.top/gtkdsmkwmg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtgxnbabpf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aizwys.cn/gtjkvlluaq.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtvtokidgq.html


<!-- 参考信息 -->