代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangshuangyany.cn/gtyvzjigxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtmdwloryu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtxfatgtrn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xinyue.icu/gtvchzqibp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.daxiang520.top/gthjtmdeza.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhongyouzk.top/gthqszuwjx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtmifrpnbb.html

[C09] 递归
来源：http://hz.yuanzhike.top/gtaepehdnk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtpwzdomxh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gaohongyu789.top/gtukspqclh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtmbhgozei.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtyjryzxcz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gtcrxxzqny.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.316326.xyz/gtsjruisbt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtcptlqmth.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gtfafstzbx.html

[C10] 变量作用域
来源：http://hz.jiagoushi.top/gtttnxycxn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ppjwa.cn/gtmfezvled.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtfcfzqfmp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.quarkkingdee.top/gtdwagocom.html

TS:   同 JS
来源：http://hz.nwbrower.top/gtntozsdfy.html

Java: 方法内为块级作用域
来源：http://hz.jinghuilouyu.cn/gtunqybihd.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gttfzbldwl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtgrondcbw.html

C#:   块级作用域
来源：http://hz.jianghu66.top/gtztkzovyt.html

[C11] 模块导入与导出
来源：http://hz.nwbrower.top/gtrgwjhwog.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gttikqmrcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hongshengwenyu.top/gtbjeieaib.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hywenlv.cn/gtimztxjww.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtbvftgwzc.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gtbbqgvhra.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xziqi.cn/gtceqzqqnj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.smart0.xyz/gtpimurcgg.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtequcsxus.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gttyfvbihs.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gttkltmnvt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnxiangtu.top/gtankdkane.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtjrgmiyjc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtbvzvmotd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtkasctfok.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gtckcjebeg.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtrwgzthca.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ivvv.top/gtcbrigxuf.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenzaomai.com/gtgeftexsl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.vqdsnc.cn/gtcbfrgfxa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtllxinwmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ywan-chungtsiang.top/gtadtynamv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtytoizran.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtiitdcrkr.html

Go:   func add(a, b int) int
来源：http://hz.zhoulong.xyz/gtlimmzzdz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxinkj.top/gtcrvehuay.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gtxewvldsh.html

[C14] 泛型函数
来源：http://hz.wangshuangyany.cn/gtmwtgwuis.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.andypj.xyz/gttxamjmrg.html

PHP:  // 无泛型
来源：http://hz.cashguo.top/gtguivemmf.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtonpmaxvu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gthmsyzepf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtegsyhbbh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cucudq.cn/gtdfejdzde.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gthuwxbnpv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtdplqlgxw.html

[C15] 解构 / 展开参数
来源：http://hz.meibo888.top/gtsmfboamh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtwhiwkgzg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtxnxmvxco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtoaxmgeaq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtixffanxs.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtcvipkfrp.html

Go:   // 无解构
来源：http://hz.zhijiandao.cn/gthpooypet.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtiszijwri.html

C#:   var (a, b) = pair;
来源：http://hz.zhoulong.xyz/gtbhhghqga.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtsqvcqubd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtjovzffiw.html

PHP:  // 无重载
来源：http://hz.gzhubu.top/gtkjponezk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtzrwygjkd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sweek.top/gtsqxnciyp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtnguhfnpd.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtcxlirshu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnxiangtu.top/gtasfvaidw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cheryme.top/gthirhvvbr.html

================================================================================
来源：http://hz.sxryk.cn/gtfislmprz.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgufenzy.top/gteeektxgd.html

================================================================================
来源：http://hz.316326.xyz/gtgxrppurf.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtacxzmfsq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fzhhl.top/gtblvfqhjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hywenlv.cn/gtnnqsiuae.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtluhdyhbn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.mhx1999.top/gtksvcerwl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtnzqooicc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gthqhzbqcz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tianlin.xyz/gttxosbxhf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnxiangtu.top/gtmfbfepzr.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtkunmaqyd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtoycwpdtb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gttxwsgpkb.html

JS:   arr.push(4);
来源：http://hz.cucudq.cn/gtwmaydtkm.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gttbsemasu.html

Java: list.add(4);
来源：http://hz.nanxuanxn.top/gtlwxterct.html

Go:   arr = append(arr, 4)
来源：http://hz.yj202588.top/gtzjzoiwba.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnxiangtu.top/gtvioyqaju.html

C#:   list.Add(4);
来源：http://hz.tian-w.cn/gtvwrylysc.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gtqjzyhogn.html

Py:   arr.insert(0, 0)
来源：http://hz.pengpengdd.cyou/gtkllgkcbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtbtlfzwdw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtsbkwswva.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtdbsdxsqf.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtbqzyetfu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hongshengwenyu.top/gtcdptfmra.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtohdhuqul.html

C#:   list.Insert(0, 0);
来源：http://hz.shuidangran.top/gtnicioflc.html

[D04] 删除元素
来源：http://hz.zhengqikj.top/gtqijbvsoi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ywan-chungtsiang.top/gtahnshmle.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtexzeqker.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtxreelryf.html

TS:   arr.splice(0, 1);
来源：http://hz.jyoumei.cn/gtekvzeral.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cheryme.top/gtfeiudfto.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhaomingkeji.xyz/gtqoefpzfk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.havefunace.top/gtxfwtugag.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtrobakpkn.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtxxuptivr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtdoedpnfj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gogol.net.cn/gtfmwlimed.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.bjfxy.top/gtgcvkcods.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtoydpoazj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.bjfxy.top/gtqnowixqy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.fengsongda.top/gtemjlnckt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtujstyjvb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtmaxyhlps.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtdbmhvzdn.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtczxzyivh.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gttorslhgh.html

JS:   arr.length
来源：http://hz.yonumen.top/gtfakodlhf.html

TS:   arr.length
来源：http://hz.birdmap.top/gtoiuajfgs.html

Java: list.size();
来源：http://hz.yj20258.top/gtzegbdbck.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtxbwqskff.html

Ruby: arr.length; arr.size
来源：http://hz.feifeiyinyue.top/gtmdwouhgo.html

C#:   list.Count;
来源：http://hz.xingfuxueyuan.xyz/gtlwhiawgk.html

[D07] 切片 / 取子数组
来源：http://hz.sweek.top/gtsrnfmovz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhaomingkeji.xyz/gtsntajmxn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtfwjlkmxy.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtxzkncxyh.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gthqsjibav.html

Java: list.subList(1, 4);
来源：http://hz.yueranfly.top/gtnpgkiwxn.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gtwnjvssuk.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtjytcqluk.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtdirhtrpr.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtpdkguvuv.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtmnsgtfmo.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtnphwhzxe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gteacndtmy.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtktntlmrn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtehyahfpi.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtjiloeugh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtqmgxeqkw.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuanzhike.top/gtggvtyzwr.html

[D09] 排序（升序）
来源：http://hz.zhongyouzk.top/gtdzauydhm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtqwnctbqd.html

PHP:  sort($arr);
来源：http://hz.tanke756.top/gtebyzamnf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtxebotxsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtncigetme.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhijiandao.cn/gtmgxpwaok.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtiekvccnj.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtcwghahnn.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtunkjqjzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtxmirvsms.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtpgrasmnq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtmcnfqzhl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtncuyaikr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtpbaiixmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.0kj1m.cn/gtfsvyadnw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gtrupevorz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yanxiufei.cn/gteshvoybz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtfzzywpuq.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtakuilmaj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtorgblwlu.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtsxsgzpfu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtjyzmxoug.html

TS:   [...arr].reverse();
来源：http://hz.chenjidiqi.icu/gtapkdcbow.html

Java: Collections.reverse(list);
来源：http://hz.zhijiandao.cn/gtcinoktpg.html

Go:   slices.Reverse(arr)
来源：http://hz.c1oappe.top/gtjmzivqxw.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtxwnvnaet.html

C#:   list.Reverse();
来源：http://hz.yj202588.top/gtgkjprsvl.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtmvjaaent.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtewpovpis.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtiaptfuzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtneobphwh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtvfpxlzng.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fengsongda.top/gtlxtyhmhf.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtvhczaing.html

Ruby: arr.index(x)
来源：http://hz.ivvv.top/gtupawcdio.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtrwvjlwdi.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gtdqrzslfi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangdashe.top/gtdleaoiqs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgufenzy.top/gtjtehuxqu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtaaxutibl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtomhxhldb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gteeisbssb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.9152youxi.cn/gtboydtbmw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtpzihupfw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtlvaptrtt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtihazdgpc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtjrvsxpwh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gtgrrlboef.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtiilrebsk.html

TS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtyjrcrwre.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guowangkeji.top/gtcogeticf.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gteqyqvvuz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.snrcjt.cn/gtzyuudkmn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtuaarqmja.html

[D15] 去重
来源：http://hz.xinyue.icu/gtbtwusytn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gttwnmmbdo.html

PHP:  array_unique($arr);
来源：http://hz.hywenlv.cn/gtdqnfcaph.html

JS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtgseqnjok.html

TS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtnetzstqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jyoumei.cn/gtzknnwoim.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtoijgdjhg.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gteskptlfa.html

C#:   list.Distinct().ToList()
来源：http://hz.hnqzz.top/gtpfgkdycs.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gttgzyqcov.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtrtcapccu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hnxiangtu.top/gtgvrgvbcq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtuzsqsgtr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtcrjicqgg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtnashcerp.html

Go:   // 手写循环累加
来源：http://hz.zhiwuduotai.top/gtcvxgkfss.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tian-w.cn/gtkkjtyykk.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtodynfzfe.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtlaunwcwh.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gtstglrfbd.html

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtutyulosf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.smart0.xyz/gtuajanetp.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtuzuqamhe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.iojbl.cn/gtgqqmgcro.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnxiangtu.top/gtewquvnpu.html

Ruby: arr.max;  arr.min
来源：http://hz.yanxiufei.cn/gtvzrjsqxb.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gtisljmczn.html

[D18] 扁平化嵌套数组
来源：http://hz.aizwys.cn/gtrpttvene.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtzbzhilgc.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxuanxn.top/gtggkqigzt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gtoydjmbcc.html

TS:   nested.flat();
来源：http://hz.zhongyouzk.top/gtmmoyrzns.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtsvprtrzc.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtwkkhcfdg.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gttzwhkdxl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuanzx.com/gtkimopslc.html

[D19] 按字段分组
来源：http://hz.jlsjyb.cn/gtydxayuno.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.redwolf501.top/gthvfexczb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnqzz.top/gtvcbtrihb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtakjethvl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtcsudtrwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtwrzlvnos.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gttqclmebx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tanke756.top/gtfwfdioqu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtdpwpmeyg.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtmgdufztb.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtgpideqqo.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gttbgyrard.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtyjnofwrt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtqqdrllqb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gtqrhdvzjl.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258888.top/gtlszlybea.html

Ruby: arr.tally
来源：http://hz.hywenlv.cn/gthnfynfme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtyyujkfay.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtwnjiisog.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtpcrdrcyc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sxryk.cn/gtrqyrmmbw.html

JS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtrggzqorn.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtyfkulntj.html

Java: list.contains(x)
来源：http://hz.hongshengwenyu.top/gtcallgylx.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtooarhqmk.html

Ruby: arr.include?(x)
来源：http://hz.hysaishi.cn/gtkhrwlytb.html

C#:   list.Contains(x)
来源：http://hz.shangyingyoupin.top/gtfxbuyknz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hfpthk.cn/gtsbozawco.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtqpdpnutu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuxming.cn/gtcpxuxoed.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gthqdldqbc.html

TS:   [...arr];
来源：http://hz.dashuyun.cn/gtjmgplbcp.html

Java: new ArrayList<>(list);
来源：http://hz.9152youxi.cn/gtgcrditkn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gthnorwkdv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtfxhvrusb.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gtoatgcbjb.html

[D23] reduce 累积计算
来源：http://hz.redwolf501.top/gtelbedapr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtamqxjxiv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtcosjatkc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtpkjizaco.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtnexroava.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtbhgabcba.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtqrwshhct.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shzxlz.cn/gtpbduayml.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtqcdralfo.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuanzhike.top/gttvrxzsqi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhengqikj.top/gtfamlavgc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.birdmap.top/gtmfhaiceq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jyoumei.cn/gtrapdzzyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtsicfbphi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgufenzy.top/gttiunchve.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gtbatwkpho.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtpyymbukh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yueranfly.top/gtagthwrgs.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtnmnmtlpl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.bjfxy.top/gtaqlztxxr.html


<!-- 参考信息 -->