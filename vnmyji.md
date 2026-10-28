代发 wailian999

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gtiaequazd.html

Py:   square = lambda x: x * x
来源：http://hz.jinghuilouyu.cn/gtwvkiytoh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtrhlluuiu.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtauqmovoz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtcizcppsy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gteonokoes.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtrjqqnhiu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yangfankeji.com/gtpzilvoyq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xinyue.icu/gtmppouujd.html

[C07] 把函数作为参数传入
来源：http://hz.sufxvd.cn/gtdobfyudm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhiwuduotai.top/gtnjyeycnj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guannengcc.top/gtuelsyemo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gttvownhda.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtbiwvzwke.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtaomtyoef.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sufxvd.cn/gtsbtejznd.html

Ruby: arr.map(&:upcase)
来源：http://hz.guannengcc.top/gtwofvmwri.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aibaodan.cn/gtbtjwjrip.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtmgvwrjoi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenzaomai.com/gtuvmmymhe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtxrumtcgl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtkcczzlbu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtxdomxwmd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fengsongda.top/gtpzjfdljc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tanke756.top/gtreomusix.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.iojbl.cn/gtdvoxpjyf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtyhdakhsf.html

[C09] 递归
来源：http://hz.zhixingplan.top/gtxqxrcnly.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtqlolzvmy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cashguo.top/gttzhszdmh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtioshbaeb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gteorlxulr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtbnztskcu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gtgjovqfzc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.iojbl.cn/gtbnhserxi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtruanqxqn.html

[C10] 变量作用域
来源：http://hz.pengpengdd.cyou/gtwjhxddou.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtpahdgdsf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenjidiqi.icu/gthwgsvfmg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtokqxxkgd.html

TS:   同 JS
来源：http://hz.xylfe.cn/gtnvtyfxio.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gthhjbkhdd.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtzeyemvza.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ehwqpu.com/gtzsgfedog.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gtansogdlt.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtszdxlhua.html

Py:   from module import func
来源：http://hz.daria6918.cn/gtroukukyi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gtbxzlpear.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtwblthjep.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.kuanghao11.cn/gtmowemmps.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtikhowayw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtagwaljbx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtdedgfswt.html

C#:   using System.Text;
来源：http://hz.daria6918.cn/gtjspkneqa.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtykmghmdv.html

Py:   (lambda: print("run"))()
来源：http://hz.xylfe.cn/gtzyjwsfab.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hammf.cn/gtiihwducq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtqryqpype.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtggvdsrkw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtdbcadowo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtorzidake.html

Ruby: -> { puts "run" }.call
来源：http://hz.yvedp.cn/gtvojnnjuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtefpljsrw.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gthtbdylvg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtxfyyhbsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtngrgvhoe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtsycmvahh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtmerwtpax.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtccarjkhg.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtsxtdaldu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xylfe.cn/gtbuawuwen.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtamtxxztr.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtbmcwidrd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shangyingyoupin.top/gtmeyeaxcw.html

PHP:  // 无泛型
来源：http://hz.wangshuangyany.cn/gtwngpwyjm.html

JS:   // 无泛型
来源：http://hz.zhongyouzk.top/gtfgwhirfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.52xcode.cn/gtuqllgbqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhijiandao.cn/gtlrxrxvma.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cheryme.top/gtnbstdbmi.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gttwdvnuwo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sysykeji.top/gtmcqpgfcp.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gtkedrxwyc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtynukludv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cqqwz.cn/gtkcoxosca.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtuwixpnrf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtnydoalnc.html

Java: // 无解构
来源：http://hz.jqgufenzy.top/gtdciegnaf.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtpbchvdwn.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gteeihnunq.html

C#:   var (a, b) = pair;
来源：http://hz.shuidangran.top/gttfpibvhy.html

[C16] 函数 / 方法重载
来源：http://hz.sxryk.cn/gtxngvktpc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guannengcc.top/gtwfwnvyox.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gteanvthtu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tianlin.xyz/gtlmoqqinc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtvdzlkkdp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtmjlauwer.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtusrlpyac.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtrywfklpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtzwtycmvt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtokgqtchx.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtuiontxyj.html

================================================================================
来源：http://hz.hysaishi.cn/gtttqqjxkp.html

[D01] 创建数组 / 列表
来源：http://hz.zhiwuduotai.top/gteuuttaru.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhengqikj.top/gtfhmhoqla.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhaomingkeji.xyz/gtorcvxdmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtldounekd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gttijgustx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangshuangyany.cn/gtarswbxbp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.havefunace.top/gtaxhpevsp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gthhfdmgzk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shuidangran.top/gtmrwpwmpx.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtzkrleguz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gthepoeuik.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yueranfly.top/gtmzhfahlt.html

JS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtllltlbto.html

TS:   arr.push(4);
来源：http://hz.cheryme.top/gtosqtntpo.html

Java: list.add(4);
来源：http://hz.meibo888.top/gtvpvecaks.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtslcmpvky.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhixingplan.top/gtillfxepg.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtjcmfhpeg.html

[D03] 在指定位置插入元素
来源：http://hz.jqgufenzy.top/gtvvikvcjn.html

Py:   arr.insert(0, 0)
来源：http://hz.svipenyu.cn/gtzvvfitqj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tianlin.xyz/gtvucexinm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtcyqdlrjl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gzhubu.top/gtpohczsep.html

Java: list.add(0, 0);
来源：http://hz.316326.xyz/gtgmwidifd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gaohongyu789.top/gtuuetvbnz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xylfe.cn/gtjdzevaea.html

C#:   list.Insert(0, 0);
来源：http://hz.yonumen.top/gthsmgzbze.html

[D04] 删除元素
来源：http://hz.sysykeji.top/gtuconghyu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangtech.top/gtgbmijpfm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtgpsjhmjp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gtdzwekoqb.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtsjjbhjuq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtrlfryucf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuxming.cn/gtrtyivpcu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jlsjyb.cn/gtitfkpova.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhijiandao.cn/gtbbkzdxdk.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtzezhrgpb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtgjyjtgut.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tanke756.top/gtkplkjinj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj202588.top/gtmnwbcndj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.9152youxi.cn/gtimplgwut.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtgafzsrpi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtjeqdzaos.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gtuwofyrxa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nwbrower.top/gtofqlhnfb.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gttdotvvha.html

Py:   len(arr)
来源：http://hz.hammf.cn/gtmwxwqngw.html

PHP:  count($arr);
来源：http://hz.smart0.xyz/gtfykajqdg.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtpmnsievf.html

TS:   arr.length
来源：http://hz.pengpengdd.cyou/gtvwapvfdj.html

Java: list.size();
来源：http://hz.birdmap.top/gtcchodkzl.html

Go:   len(arr)
来源：http://hz.chenjidiqi.icu/gtzoykqomh.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtwmsjxxxy.html

C#:   list.Count;
来源：http://hz.smart0.xyz/gtswbhimzh.html

[D07] 切片 / 取子数组
来源：http://hz.gogol.net.cn/gtwabgfxok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtvpcewqlg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtblsyvmvw.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtcssljjzn.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gteiavmuqk.html

Java: list.subList(1, 4);
来源：http://hz.nanxuanxn.top/gtkzxvavqq.html

Go:   arr[1:4]
来源：http://hz.nanxuanxn.top/gtuzrpwusu.html

Ruby: arr[1, 3]
来源：http://hz.zhiwuduotai.top/gtprxjnuss.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtgfdjwcef.html

[D08] 合并两个数组
来源：http://hz.gaohongyu789.top/gtamhqxufn.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtqonmwryv.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gttlswhtfy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gttuytrjrd.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtmxlsmhnw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtnudpogsh.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtzkkvelmz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cdnleiting.top/gtvgljeerz.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgfzy.top/gtmkwzelqu.html

[D09] 排序（升序）
来源：http://hz.shangyingyoupin.top/gthpjigijf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gttukzjgtk.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtewcbfmqn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.9152youxi.cn/gtwxohnfvu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sufxvd.cn/gturvtaeok.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtjhezrgmj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtqykkuisq.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gteopqkcjs.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtvikvwtlt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtbfzaghcf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cqqwz.cn/gtcwvomtej.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gthodqsdat.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtwlzdgmqo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtjpztrepv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtticjoqhq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.c1oappe.top/gtcxwxhmwy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pycfn.com/gtussyiqym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtbciepuae.html

[D11] 反转数组
来源：http://hz.hysaishi.cn/gtsdzlcogj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtumykdomo.html

PHP:  array_reverse($arr);
来源：http://hz.zhongyouzk.top/gtpygtcqvd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daria6918.cn/gtuynyrryu.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtgiuikpnc.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gttlmmvnlx.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtmbvpnfih.html

Ruby: arr.reverse
来源：http://hz.tian-w.cn/gtkphszmqh.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtxrusspjx.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtdklkydos.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtxyvwueqr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangdashe.top/gtltnheecz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtsetyqjan.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gthwpkpndm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtvigkgajr.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtxcdimkyo.html

Ruby: arr.index(x)
来源：http://hz.havefunace.top/gtounjxvwl.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtuzvhnyey.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuetiantiany.cn/gtmihhnuad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtirxeqoez.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtqieyocai.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtkjbiyoer.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtrxxvkqex.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtudgcakjv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtdednxyde.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhongyouzk.top/gtcmferakz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnqzz.top/gtkoumoiso.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydzc1.top/gtoiflwshl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtixakpqtq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gotoacloud.top/gtbnugteim.html

JS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtelxthlbd.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtsiywhpth.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnxiangtu.top/gtyflokkmy.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtcqkpvjfu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yongpay.top/gtmleazigr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtlmnypavg.html

[D15] 去重
来源：http://hz.daxiang520.top/gtvheiitqe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtjtovlhei.html

PHP:  array_unique($arr);
来源：http://hz.yj202588.top/gtszwuxoav.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtfvnlnyoq.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtoiomwzbw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtjcapyecp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hongshengwenyu.top/gtbrlfwgli.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtdrucmsrz.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangkeji.top/gtgvlfvbzy.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gtuhwllqub.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtfpzvddwf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sysykeji.top/gtliudwxek.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtbvtmhstt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtiflgcsyb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ppjwa.cn/gtplagtkvb.html

Go:   // 手写循环累加
来源：http://hz.hnxiangtu.top/gtviftmsit.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shuidangran.top/gtanxhoqgh.html

C#:   list.Sum();  list.Average()
来源：http://hz.guannengcc.top/gtvgdldvgx.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtqhskncqp.html

Py:   max(arr);  min(arr)
来源：http://hz.zdqjudy.top/gtazdmcxip.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhijiandao.cn/gtfnpmdavc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gtbdefambg.html

TS:   Math.max(...arr);
来源：http://hz.havefunace.top/gtjzakcmrv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtazdteruh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fengsongda.top/gtbmppqtqa.html

Ruby: arr.max;  arr.min
来源：http://hz.ivvv.top/gtfpmvpjhr.html

C#:   list.Max();  list.Min()
来源：http://hz.dianchejie.cn/gtwtejtyuq.html

[D18] 扁平化嵌套数组
来源：http://hz.zhixingplan.top/gthwvqkykl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hysaishi.cn/gtwaziydov.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigufen.top/gtfxuvceav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtjnszbqrg.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gttuuohmci.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cdnleiting.top/gtnpypdmox.html

Go:   // 手写双层循环
来源：http://hz.gotoacloud.top/gtodnxwocc.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtcmjemwhi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtvjfqbdsd.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtygkcjrrw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shangyingyoupin.top/gtqmfwwngn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtoucylsbt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xziqi.cn/gtosnwktep.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtpcarxoik.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.52xcode.cn/gtuyfgofqu.html

Go:   // 手写 map[string][]T
来源：http://hz.ivvv.top/gtjgiwwkjh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtsrpcqsug.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtgjdqjvlm.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtpvygnfty.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtdmsdugew.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtorxvxpkq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtjjfqlvmu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtxbgdrmra.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258.top/gtixotdjah.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258.top/gticbncvvu.html

Ruby: arr.tally
来源：http://hz.yangfankeji.com/gtsjvxmczv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtthtzqcww.html

[D21] 判断是否包含某元素
来源：http://hz.shangyingyoupin.top/gtgqiqajwr.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtsmgepaiy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtglrbqqnb.html

JS:   arr.includes(x)
来源：http://hz.haohaochexian.top/gtnbdkpben.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gteplbgsqp.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtokoskskk.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtdmuddufe.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtzfswjqhs.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtzxdzxcqn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtlvnrvkxc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtlozwrkwi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yonumen.top/gtloyhyrfg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtttouruld.html

TS:   [...arr];
来源：http://hz.shanyushiyangkeji.top/gtyltlujiw.html

Java: new ArrayList<>(list);
来源：http://hz.mhx1999.top/gtoooxvmdl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.9152youxi.cn/gtfnyixknq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtioeiqerx.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gtfzgqbdrf.html


<!-- 参考信息 -->