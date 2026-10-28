代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258.top/gtnohbputi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtuyavxcbf.html

[C08] 闭包
来源：http://hz.shanyushiyangkeji.top/gtsojoidww.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pengpengdd.cyou/gthnmvbiah.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtdpsqnkrd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtqvpsylsy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtmufeuiee.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtncgzptce.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhoulong.xyz/gtxzozbmcz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtolmwgtij.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtgeqpqqke.html

[C09] 递归
来源：http://hz.jinqigufen.top/gtiuwzubkf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.bjfxy.top/gtprjmvuqg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtkcmoomgu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtjvcyeuxg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtwrtepnpb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gaohongyu789.top/gtstjgderl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtedhjsalz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtilxaztrf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.0kj1m.cn/gtprdzcxyw.html

[C10] 变量作用域
来源：http://hz.shzxlz.cn/gtijardyqw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fzhhl.top/gtdqqmsaxj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtqzvdmvoj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gticnmqdlc.html

TS:   同 JS
来源：http://hz.yangfankeji.com/gtqsyzfxhb.html

Java: 方法内为块级作用域
来源：http://hz.pengpengdd.cyou/gtdoizppqu.html

Go:   花括号块级作用域
来源：http://hz.fengsongda.top/gtsivxrviu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gotoacloud.top/gtrgbiwymk.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtcsdcjihk.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtyfujkqne.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gthklhlbau.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.fzhhl.top/gtupmtmraf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ehwqpu.com/gtkovruohz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtccurmhbo.html

Java: import java.util.List;
来源：http://hz.hnqzz.top/gtyhcnxvxo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtarouqvun.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtzivbfvpk.html

C#:   using System.Text;
来源：http://hz.fengsongda.top/gtbzijopin.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gteycbievz.html

Py:   (lambda: print("run"))()
来源：http://hz.ydjk.org.cn/gteszmoccc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtaeigdstk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtszqxemdz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtwnyuumnp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.dianchejie.cn/gtnhsoybki.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zdqjudy.top/gtonfgcwrt.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtddocnfns.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gtwjmkdomm.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtlfctiuoj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zycfv.cn/gtndqzeswy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtjzgfmuhs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gtwxhyopyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtjcqfaxmy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtgiekecwv.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtntcvgnrz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtxyrdfqjg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xziqi.cn/gtfqocdivd.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtlpwenhai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gtgycugzno.html

PHP:  // 无泛型
来源：http://hz.cqqwz.cn/gthzjalnec.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gthfkbxoox.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtjkaxdzvm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtoutbtswd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtxeqtokaz.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtpvdbxhac.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydjk.org.cn/gtmtbioosi.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtehvybvkr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gttbkebqhs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.bjfxy.top/gtntmfhaeh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtppapvhgd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jiagoushi.top/gtvprbwnuk.html

Java: // 无解构
来源：http://hz.cqqwz.cn/gtzpkngfyt.html

Go:   // 无解构
来源：http://hz.zhiwuduotai.top/gtijnefuxd.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtctnkcbjq.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gthpyzdefa.html

[C16] 函数 / 方法重载
来源：http://hz.jqgfzy.top/gtxlivpubg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnxiangtu.top/gtjjbyngly.html

PHP:  // 无重载
来源：http://hz.yongpay.top/gtkqqswnrf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtgkjvmitu.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ydzc1.top/gtrcckvzww.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtmjetrkto.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtdvjqlkiy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gtdyfbixyc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtdxwoniwy.html

================================================================================
来源：http://hz.chenlongwang.top/gtmyzaofsi.html

D. 数组 / 列表 / 集合
来源：http://hz.zhaomingkeji.xyz/gtnjmhaast.html

================================================================================
来源：http://hz.zhixingplan.top/gtsluxgkdv.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtlkaxigyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.snrcjt.cn/gtejuypgyp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuetiantiany.cn/gtdpmzjsoz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtwtufuxnc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.feifeiyinyue.top/gtmuzqawbq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtawdjnwkn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenlongwang.top/gtlulkuwhn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtiryanhqs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtssfdeyat.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtgoprunbz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtotfpjxbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtiufasaih.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gthyqjhudm.html

TS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtxtmnoirf.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtwybuqaix.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtqnvxbbuh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuxming.cn/gtnxnimneb.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtvpgbykjn.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtbdetjsho.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtzrllwjaw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shuidangran.top/gtmyynhvtz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuetiantiany.cn/gtqaxyudra.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtildzijgj.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtmbjddfqv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtgefdolzp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtrdxazqmr.html

C#:   list.Insert(0, 0);
来源：http://hz.havefunace.top/gtnaftulvv.html

[D04] 删除元素
来源：http://hz.shanyushiyangtech.top/gtwttwafwe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtgjsdokhs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fengsongda.top/gtfaaelvoo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtqzokwnrz.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtibsohubh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gtwxtmonne.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtbtzuucdl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtjzznralh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtdfgbwpdg.html

[D05] 访问与修改元素
来源：http://hz.tanke756.top/gtdbyubeme.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtxzxeadyo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtfeijgsmv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtaavubcou.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtmobteqyc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtcpsdvszu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtynphxghf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtueidppvc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gtkjgnfwfu.html

[D06] 数组长度
来源：http://hz.dianchejie.cn/gtsgzlxudg.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtgkazeghj.html

PHP:  count($arr);
来源：http://hz.hnqzz.top/gtzllfyiyf.html

JS:   arr.length
来源：http://hz.jyoumei.cn/gtyqaqbrxh.html

TS:   arr.length
来源：http://hz.jqgfzy.top/gttutszdcl.html

Java: list.size();
来源：http://hz.havefunace.top/gttvfurqgf.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtyxukteet.html

Ruby: arr.length; arr.size
来源：http://hz.zhaomingkeji.xyz/gtqrnkgeqj.html

C#:   list.Count;
来源：http://hz.shanyushiyangtech.top/gtdcsboewq.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtokrbqdos.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hywenlv.cn/gtlnpwqpzc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtyzcjlfdj.html

JS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtxwmhjncm.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gthbcxuyzc.html

Java: list.subList(1, 4);
来源：http://hz.hnxiangtu.top/gtttemmhig.html

Go:   arr[1:4]
来源：http://hz.hfpthk.cn/gtatwogdmu.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gteuopipxe.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtjzdhjrae.html

[D08] 合并两个数组
来源：http://hz.andypj.xyz/gtmahldcyn.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtsqghoetf.html

PHP:  array_merge($a, $b);
来源：http://hz.nwbrower.top/gtqejjnuna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ydzc1.top/gtslxcfebh.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtsicvheon.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gthdbtbusp.html

Go:   append(a, b...)
来源：http://hz.xuanzx.com/gtgakrzaiz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.0kj1m.cn/gtjginyxrh.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtpnhniocb.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gtijgynjpi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtehneuhrj.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtfsvqmepl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtlpbjhlua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtchjlqljf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtzginjfbm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtugkswjmw.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtrvpxlfps.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtbyzeksgo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtzqwqhdwt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtzzrnupxe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangtech.top/gtwrduejgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtlpcwkedp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtntsegrfn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xingfuxueyuan.xyz/gtanppkezb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gtvccysbfv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.bjfxy.top/gtuztxdqfb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.316326.xyz/gtggdqbqqs.html

[D11] 反转数组
来源：http://hz.cashguo.top/gtmuzuifsa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtihknjdca.html

PHP:  array_reverse($arr);
来源：http://hz.yvedp.cn/gtrlogdrxx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.smart0.xyz/gttjbqbpnh.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtqkgwzfbf.html

Java: Collections.reverse(list);
来源：http://hz.cqqwz.cn/gtolybfjds.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtwpdqzqvf.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtzbbxvzpg.html

C#:   list.Reverse();
来源：http://hz.tanke756.top/gthczzjtsf.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtqbxrjrew.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gtqackpbkn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gtzauwtvoj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gttpkkfyoz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtpgsxdhbn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtxoanypcc.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtejvjflwk.html

Ruby: arr.index(x)
来源：http://hz.mhx1999.top/gteuikfowa.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtbdkmqxif.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hywenlv.cn/gtfgahvirq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj202588.top/gtibxmrznn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258.top/gtirsovxxe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gttdpmnewv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtcefaisso.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yuxming.cn/gtqttzuxyw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.birdmap.top/gtolhjthve.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yueranfly.top/gtuqkggdrw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gzhubu.top/gtsfaiific.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yongpay.top/gtclwniyec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gthzzvdwrf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtgwszftna.html

JS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtjveaudlg.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtqrrgeidc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtiruxtnuz.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtdubnqvbn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtobccdcih.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj20258888.top/gtttmoopia.html

[D15] 去重
来源：http://hz.jinqigfzy.top/gtupgweapc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtkkzajhje.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtxmiucehc.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtovtglbfn.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtlkdpoirx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtlcbjscnh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gttfkcdnzu.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtgvvobidb.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gttblivcrf.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtriezfojs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.redwolf501.top/gtjiocujcz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.havefunace.top/gtukftnfqb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtnldnycdr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtunxbqhan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtraxjofnf.html

Go:   // 手写循环累加
来源：http://hz.zhixingplan.top/gtedeihsrz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtbhwynixl.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtvhhyujst.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gtocdlirjd.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtobwwghdc.html

PHP:  max($arr);  min($arr);
来源：http://hz.jqgufenzy.top/gtounxzmpu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gttkyeyjxa.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtrxghrnla.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yvedp.cn/gtoaqpogyk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangtech.top/gtrcwmfvpl.html

Ruby: arr.max;  arr.min
来源：http://hz.yuanzhike.top/gtgjwpsgiw.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtgpevqezm.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtsvmknbqc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgfzy.top/gtztoanlzd.html

PHP:  array_merge(...$nested);
来源：http://hz.aizwys.cn/gtrozxwpxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.mhx1999.top/gtinqjiuuw.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtirhzakks.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gttpyltnzo.html

Go:   // 手写双层循环
来源：http://hz.chenlongwang.top/gtvdbpmsiz.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtedsgnksl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuanzx.com/gtajxoiayx.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtzggobfvd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtdkhuvvyx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtqebgihkc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gthbvsatwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtxfyfasmd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gaohongyu789.top/gtxbrlvbgg.html

Go:   // 手写 map[string][]T
来源：http://hz.snrcjt.cn/gtusstcrlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtpwzmqjrz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtxhqdieib.html

[D20] 统计每个元素出现次数
来源：http://hz.xuetiantiany.cn/gtpnmmvztp.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangkeji.top/gtyohdawac.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtrdjjdqns.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gttpfogiss.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gthcicubqs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtvnepifwr.html

Go:   // 手写 map[T]int
来源：http://hz.hywenlv.cn/gtcmulcqbk.html

Ruby: arr.tally
来源：http://hz.nwbrower.top/gtxjfjvdnu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shzxlz.cn/gtythwncpp.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtavstxyuy.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtldmxxxea.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jlsjyb.cn/gtyepgschr.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtzeootrbb.html

TS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtsuwegjmz.html

Java: list.contains(x)
来源：http://hz.ppjwa.cn/gtknpgoahv.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhongyouzk.top/gtanqqcstj.html

Ruby: arr.include?(x)
来源：http://hz.sufxvd.cn/gtrkfxsehb.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtycqqeknl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zycfv.cn/gtlaphnqfn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258888.top/gtgddxbybw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtgliuspsb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtqizhtybs.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtrppjwdco.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gtkkpsydgi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gzhubu.top/gtzioklfye.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gthtnimnsk.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtgshoowgk.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtjuqchfrc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtmzdnhbyl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtrmigsswy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtqkhpqnys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtaoawmdkv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtgzphzmzd.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gthemgqglm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gogol.net.cn/gtwoyetgxk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dianchejie.cn/gtyjkdzrdw.html

[D24] 字典 / Map 基本操作
来源：http://hz.ywan-chungtsiang.top/gtbmpofbwc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtqlbboqqb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.redwolf501.top/gtynhlniux.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtqppliels.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinyuanbaomall.cn/gttmtqmasg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.vqdsnc.cn/gtqoptkmzi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtbayqnghr.html


<!-- 参考信息 -->