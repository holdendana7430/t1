代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gthdkxkyfv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shanyushiyangkeji.top/gtzspeuetk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtxchdujyb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtxciuhqqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtlabrwdpj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.snrcjt.cn/gtwraejmcr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtsrwfnmxt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gthmlsndwm.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtnrcharnx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.mhx1999.top/gtqjrpuimc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xinyue.icu/gtxhnuqdhe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gogol.net.cn/gtrnzqyzii.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtltzpgmnz.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtiopfgxhc.html

Go:   花括号块级作用域
来源：http://hz.shzxlz.cn/gthqgxnhjf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtiwhnusnk.html

C#:   块级作用域
来源：http://hz.xylfe.cn/gtmjvwdodo.html

[C11] 模块导入与导出
来源：http://hz.nanxuanxn.top/gtgkahcixc.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtjvtdbgkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gttkoaiozt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtejqxteir.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jlsjyb.cn/gtnqtwohhz.html

Java: import java.util.List;
来源：http://hz.birdmap.top/gtubdppyga.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gttxdnjwdk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtpfcdlwmf.html

C#:   using System.Text;
来源：http://hz.xuetiantiany.cn/gtpitgkbdj.html

[C12] 立即执行函数 IIFE
来源：http://hz.jqgfzy.top/gtcwsnibjo.html

Py:   (lambda: print("run"))()
来源：http://hz.chenzaomai.com/gtptxotcas.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aibaodan.cn/gtctukujlf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtpatqnwbq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtoeofyubh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtyhgeykya.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gtmgmdwcqa.html

Ruby: -> { puts "run" }.call
来源：http://hz.hywenlv.cn/gtfngcsbhs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gtfhvenkhv.html

[C13] 类型声明 / 类型注解
来源：http://hz.cdnleiting.top/gtrqbdcsxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtneiiynsg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtlzalfpoc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtgqmsgzfa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtlhvgvfaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtpsgbledn.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtmzrxudvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhoulong.xyz/gtpujzvmio.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.svipenyu.cn/gtlypucomr.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gtfzxjkyeo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gthyllcnzo.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtdzxrkpay.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtmppmjhyr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.feifeiyinyue.top/gtavnxiorm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gtlvnxjpor.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtotdgbcyg.html

Ruby: # 无泛型
来源：http://hz.meibo888.top/gtqmlbfmqh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtujxivyrk.html

[C15] 解构 / 展开参数
来源：http://hz.birdmap.top/gtcoeloipp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangkeji.top/gtpksrcnsd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtvnhpvhfn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtzupceime.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtmjftuwfg.html

Java: // 无解构
来源：http://hz.fzhhl.top/gthdvtdtrr.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtxjhxjrwg.html

Ruby: a, b = pair
来源：http://hz.jqgfzy.top/gtjgyuigwf.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtyyjzatug.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtumfimism.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtjakrerzs.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtfforguev.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtektljfml.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gteajzfubh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ybcxt.top/gtnclnjdiv.html

Go:   // 无重载：用不同函数名
来源：http://hz.aizwys.cn/gtylkeqnqm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtzlmaxiaz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtktukfmgc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlnjbhbyf.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gtbclmfkyf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtilskulxr.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtacittbiv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtbcmxelfq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtodvfqflb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gttihkszcr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtctrnbfpn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtzafvawuw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtdxluulnq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.havefunace.top/gtnqwfsduv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtrwtpykqa.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtfmxfbiac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtrdhjmaad.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.vqdsnc.cn/gtjndhohrw.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtsybnvgoo.html

TS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtatjptzif.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gttccoxrlz.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtqvdplnhi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtehjysypg.html

C#:   list.Add(4);
来源：http://hz.gaohongyu789.top/gtwiqslocv.html

[D03] 在指定位置插入元素
来源：http://hz.yvedp.cn/gtbcuphbeo.html

Py:   arr.insert(0, 0)
来源：http://hz.aibaodan.cn/gtonlgxofh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gtkkbksmwo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cucudq.cn/gtrrihpkvj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hfpthk.cn/gtwjsqvwsy.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtcgbmuujk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtkekrcwfl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtbhhfzcho.html

C#:   list.Insert(0, 0);
来源：http://hz.chenlongwang.top/gtsoxuefff.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtxvfxhlzr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtlfdlvzez.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtsgnoemgj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtyatypibn.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtbfnqwoks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.quarkkingdee.top/gtkpgzltaq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gttbnamozs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtkrhlucut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hfpthk.cn/gtxdxxwbka.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtyertyhuq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtyavgxhhi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgufenzy.top/gtppyzstzz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.wangdashe.top/gtokahdquf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gtndwxydfr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zdqjudy.top/gtooxffsvw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.mhx1999.top/gtndeyisre.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtuptigmrc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yongpay.top/gtmgfxablf.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtptedgell.html

Py:   len(arr)
来源：http://hz.nanxuanxn.top/gtzllrjxyv.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtndnxkdri.html

JS:   arr.length
来源：http://hz.snrcjt.cn/gtpjzzwjpk.html

TS:   arr.length
来源：http://hz.52xcode.cn/gtebmoatvw.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtibpdlcrn.html

Go:   len(arr)
来源：http://hz.jlsjyb.cn/gtquwavtfs.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gticpgppyp.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtjyvwwrot.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gtaqyhenfj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gtnniwmuto.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zycfv.cn/gtrxshooyo.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtdxqpoypc.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtvrsxlrvb.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtzimtrdcp.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtbpnindwa.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtapffjgai.html

C#:   list.GetRange(1, 3);
来源：http://hz.gaohongyu789.top/gtxtxoswzo.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtktrlaiaa.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtfxlnkone.html

PHP:  array_merge($a, $b);
来源：http://hz.fzhhl.top/gtwebascns.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jlsjyb.cn/gtqgyjhasf.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtktekdovy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtgwuwabdi.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gttytwanru.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtbubbspme.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtwrkqarqg.html

[D09] 排序（升序）
来源：http://hz.yvedp.cn/gtqrptwfqt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtxzmococe.html

PHP:  sort($arr);
来源：http://hz.zhixingplan.top/gtzpbwochh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ybcxt.top/gtsaixfxhl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.mhx1999.top/gtjxjbmzrl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtosxrmgnd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtxypxgpyq.html

Ruby: arr.sort
来源：http://hz.wangdashe.top/gtohhiqjpe.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtshpbumdx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtqyuhrbqd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtzmfausmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtzzagficj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtjuzjlhuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gthjawnden.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtabgrixnc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258.top/gtkmlexedk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sxryk.cn/gtjowfmdiw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtjyophmnz.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtzjqqoinu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nwbrower.top/gtugzejjfy.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtfcmgrcan.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtfgxsoxxq.html

TS:   [...arr].reverse();
来源：http://hz.cqqwz.cn/gtepbntkjt.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtyiuxokqm.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gttiitcxuh.html

Ruby: arr.reverse
来源：http://hz.xuetiantiany.cn/gtktlncjhd.html

C#:   list.Reverse();
来源：http://hz.bjfxy.top/gtxideoldz.html

[D12] 查找元素下标
来源：http://hz.jinyuanbaomall.cn/gtbvjfbhpr.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gtjxvjhcfr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtwltektdq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtottcgvoh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtdpvhrfzr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zdqjudy.top/gtqbsiszpu.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtfnuxwvee.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtzilyxmct.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtfzdkbftl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtlnpzrfbf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtdwneurbf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtwlxchohn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gttseaorvz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtylrgnwdx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxinkj.top/gtmnnuwrxr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtxvxmbggi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtmvpkujoi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtzvdfcxyl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtvlwprgka.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gtwwgoonbg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtzlcavako.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtmujmogje.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtjikclukb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtrbkjlccu.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtudlphigf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gthchywmkm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xylfe.cn/gtbxwllcmi.html

[D15] 去重
来源：http://hz.ehwqpu.com/gtbcolyidy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtjotlbpyl.html

PHP:  array_unique($arr);
来源：http://hz.guowangkeji.top/gtpcjpkvxo.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtrzinqrwt.html

TS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtifszlyxw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nwbrower.top/gtwnvlbbjo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sysykeji.top/gtwxqlspkx.html

Ruby: arr.uniq
来源：http://hz.c1oappe.top/gtecltfcjm.html

C#:   list.Distinct().ToList()
来源：http://hz.haohaochexian.top/gtddyizrcd.html

[D16] 求和与平均值
来源：http://hz.bjfxy.top/gtckidnaxx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtloufglqb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtyetnzljv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtfhufziay.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtijtfecus.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.fzhhl.top/gthxeatizi.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtxwdakyqh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aibaodan.cn/gttsiejqqu.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtmdvugsfh.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gtytycqiwo.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gticoyjcyx.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtrghszsox.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtrbesrbrc.html

TS:   Math.max(...arr);
来源：http://hz.chenlongwang.top/gtudvsmsar.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtrenhijto.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtneuwrthk.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtxvkfmnum.html

C#:   list.Max();  list.Min()
来源：http://hz.wangshuangyany.cn/gtywuywyph.html

[D18] 扁平化嵌套数组
来源：http://hz.yangfankeji.com/gtkxwamqez.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xingfuxueyuan.xyz/gtxckvrspx.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtcjktksut.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtnwiqnlpa.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtqpjqeopf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtdgjnyqla.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtnjvoaarc.html

Ruby: nested.flatten
来源：http://hz.yj20258.top/gtzcezesnm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtlkxatuvj.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtunwzzecv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtjhmntlmi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtotjbjwps.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtxboujoeu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aizwys.cn/gtbzhduuja.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.quarkkingdee.top/gtztrrpcmz.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtpiggtryt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtdylnltks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtterqazxf.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtvlzbylqf.html

Py:   Counter(arr)
来源：http://hz.hysaishi.cn/gtsompykcu.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtxnqlvagh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtvdgvgyso.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtwddaneiq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yvedp.cn/gtuhzgwwzq.html

Go:   // 手写 map[T]int
来源：http://hz.nanxinkj.top/gtkiwnxzsj.html

Ruby: arr.tally
来源：http://hz.gotoacloud.top/gtcjkbjkks.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtyvowcihd.html

[D21] 判断是否包含某元素
来源：http://hz.guannengcc.top/gtqraxohhh.html

Py:   x in arr
来源：http://hz.zycfv.cn/gtduwglxer.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtkbfzlxtn.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtjlysbtxe.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtvbkvnlpb.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtkxwkdxhr.html

Go:   slices.Contains(arr, x)
来源：http://hz.jianghu66.top/gtuzodlbwq.html

Ruby: arr.include?(x)
来源：http://hz.smart0.xyz/gtyrszsqyj.html

C#:   list.Contains(x)
来源：http://hz.cashguo.top/gtzewtdhlg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhengqikj.top/gtknztefwm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtecnkgvtb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gthgbnfvrm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtmmfkuurh.html

TS:   [...arr];
来源：http://hz.jqgufenzy.top/gtdkhigqcj.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtnwhgeays.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtnljkgors.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtwkuszbas.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtxavtzpgy.html

[D23] reduce 累积计算
来源：http://hz.ybcxt.top/gtcnamziml.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtzzkvaevt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtaleoxtyq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gteqkriqmu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtabulxqkd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jianghu66.top/gtswsgloxq.html

Go:   // 手写循环
来源：http://hz.316326.xyz/gtkslsfmge.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtbescwbrv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtdkkdsojc.html

[D24] 字典 / Map 基本操作
来源：http://hz.smart0.xyz/gtkcdvwgle.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtrslrqajt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtwyvrrsxe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtbmougmkn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.feifeiyinyue.top/gtodwlsgxo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jiagoushi.top/gtkbvjdmpl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtherqhdlr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtzflvhggn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hfpthk.cn/gtssfszryc.html

[D25] Set 集合去重与交并差
来源：http://hz.pycfn.com/gtibkarmwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hammf.cn/gtlxvkhido.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.snrcjt.cn/gtidnagiic.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtcxbrjfad.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guowangkeji.top/gtmgtcknxm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtitdhgkor.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtkgzyvlku.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fzhhl.top/gtgexlnzpx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtewtcjzuy.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gteympmwvj.html


<!-- 参考信息 -->