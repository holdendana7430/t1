代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cqqwz.cn/gtnzkgrajy.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtjsxsseid.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.iojbl.cn/gttiiwjdzn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.0kj1m.cn/gtycmhviyk.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxinkj.top/gtsgqstuzt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gtedgetzfy.html

[C08] 闭包
来源：http://hz.yuxming.cn/gtbzrzionl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.guowangkeji.top/gtolcgcahr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hammf.cn/gtxatuphkt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtmttinjsm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtopyvvfdm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtwcpqvsqi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.snrcjt.cn/gtsuuvbspd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtjrbxgnss.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtvfdtlupl.html

[C09] 递归
来源：http://hz.gzhubu.top/gtvwhdtulw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtfzqtmxyw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangshuangyany.cn/gtqmxrxvpr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtnwxglnvx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtysszunmx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cucudq.cn/gtokanjyxs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258.top/gtwhdzhrmb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daxiang520.top/gtwyqmrdkz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtratcaywu.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gtnhrkcgqy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtwknufoqi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.bjfxy.top/gtzfbvzyrp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gtiybwgrou.html

TS:   同 JS
来源：http://hz.xuanzx.com/gtkkzfvpjc.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtlsqlqxkj.html

Go:   花括号块级作用域
来源：http://hz.9152youxi.cn/gtljincltd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnxiangtu.top/gtlhmxkqri.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtwmdvbqhi.html

[C11] 模块导入与导出
来源：http://hz.svipenyu.cn/gtlllmezbl.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtqhhnfmxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.pengpengdd.cyou/gtxefmwgyj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtbildqxba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gtgntcllqt.html

Java: import java.util.List;
来源：http://hz.quarkkingdee.top/gtouvesvgd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtpxgswzbg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gtsiuqojib.html

C#:   using System.Text;
来源：http://hz.daria6918.cn/gtsbaeemfu.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtsdtowezg.html

Py:   (lambda: print("run"))()
来源：http://hz.xinyue.icu/gtnxazgwhr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.316326.xyz/gtakweklbu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtratvnsqi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtpsgxvqzx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hfpthk.cn/gtavovsmip.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtyfczjhzi.html

Ruby: -> { puts "run" }.call
来源：http://hz.fzhhl.top/gtvzcnhugh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fengsongda.top/gtiepkyqfh.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuanzhike.top/gtpkinccrh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.0kj1m.cn/gtremsefoy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtgmcyflod.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtivnccptt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtenkbvcfs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtvfdxxhbz.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtapynqffj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pycfn.com/gtqrukkseh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnqzz.top/gtanmipvyf.html

[C14] 泛型函数
来源：http://hz.ybcxt.top/gtsdmgabge.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hnxiangtu.top/gtjzmehwpu.html

PHP:  // 无泛型
来源：http://hz.jlsjyb.cn/gtfocbuguj.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtaclscjdo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtvihbdjru.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dashuyun.cn/gtpiivedjm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtvhmdxmwf.html

Ruby: # 无泛型
来源：http://hz.pengpengdd.cyou/gtwoabajky.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shzxlz.cn/gtdywhhcgs.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtsqhcfcij.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hongshengwenyu.top/gtsnbxcrny.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtzsznlesn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gticgtoykt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtjoqoovhn.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtylqtpwst.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtegwyliwx.html

Ruby: a, b = pair
来源：http://hz.ehwqpu.com/gtvprdfygv.html

C#:   var (a, b) = pair;
来源：http://hz.daria6918.cn/gtopbkltdz.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangtech.top/gtmkozyhle.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gthovfdgnx.html

PHP:  // 无重载
来源：http://hz.birdmap.top/gtcabzrgtq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtttwaggwz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yvedp.cn/gtdiuzdbxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yongpay.top/gtyymjjmza.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtpmjozupo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gthklioeol.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtfbwlhawk.html

================================================================================
来源：http://hz.birdmap.top/gthgkjjdhp.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtiztuksok.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqfexackf.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtfznfsnij.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtlgtintpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtjufkgpbz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhengqikj.top/gtapoztptg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtbqncqurn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtpfjjpvdi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ivvv.top/gtncyjlltr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zdqjudy.top/gtxgecpmoy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtxvdfubna.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtvojbxlru.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtrldgnnlb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtllomuwvu.html

JS:   arr.push(4);
来源：http://hz.gzhubu.top/gtzcnhcumn.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtszfdabfl.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtkwyassce.html

Go:   arr = append(arr, 4)
来源：http://hz.jinghuilouyu.cn/gtwpeejzfo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtlgtihnsh.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtjtwevojx.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gtnqjjdxzz.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtzcgiizfu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtpxaeuglx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shuidangran.top/gtyuhbevra.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gtamwvlguw.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtmtourljf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtlmwsugcy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guannengcc.top/gthkfuqidy.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtnhqlelsf.html

[D04] 删除元素
来源：http://hz.havefunace.top/gtyysukhxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shzxlz.cn/gtofgefwpu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtkqrvuiix.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gthgyouuzw.html

TS:   arr.splice(0, 1);
来源：http://hz.ywan-chungtsiang.top/gttmfrcssh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtwidgmfjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hysaishi.cn/gtsqaqzndg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtdqfksngr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtwbztffrc.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtmdgbrbsk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtzzpgzbnf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cheryme.top/gtotpwypdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.bjfxy.top/gtiqvdljhw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtfzasbohg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ywan-chungtsiang.top/gtdaprihbp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtneupolfj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.52xcode.cn/gtqbcckjif.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gtwfaclinh.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtvpouwbqk.html

Py:   len(arr)
来源：http://hz.tanke756.top/gtisnivwvs.html

PHP:  count($arr);
来源：http://hz.zhijiandao.cn/gtbhssunut.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtrugmptyx.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtiawpcalo.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtqdscfeaj.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtcepqauaw.html

Ruby: arr.length; arr.size
来源：http://hz.shuidangran.top/gtzhdpwkiy.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtxyurclau.html

[D07] 切片 / 取子数组
来源：http://hz.meibo888.top/gtxpymankb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gtpbuckvdd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.52xcode.cn/gtscddcvwt.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtqnkfddfl.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtjugxvbnj.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtqtcoadws.html

Go:   arr[1:4]
来源：http://hz.daxiang520.top/gtwnjzujff.html

Ruby: arr[1, 3]
来源：http://hz.gaohongyu789.top/gtwvwuqxjn.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gtecmdetbr.html

[D08] 合并两个数组
来源：http://hz.gogol.net.cn/gtcowgfvrl.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gthykxvqoi.html

PHP:  array_merge($a, $b);
来源：http://hz.xuetiantiany.cn/gtklbozymn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.redwolf501.top/gtqltbqciw.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtzjsytdou.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gtpphirrmg.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtthuetodc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sweek.top/gttfnihdrw.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtqrccjrix.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtsdkhgoed.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtwxwftbug.html

PHP:  sort($arr);
来源：http://hz.guowangkeji.top/gtqpbomepx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydzc1.top/gttpgwbvvm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtxtgdxyve.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hywenlv.cn/gtvtecawor.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtkczyjfxr.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtymtecvcb.html

C#:   list.Sort();
来源：http://hz.dianchejie.cn/gtytlfzxex.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigfzy.top/gtjrqqmqsx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtmrdviyao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shanyushiyangkeji.top/gtbazxlfmw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtuwxgthle.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtmbmgjyzq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtfbzbztav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.bjfxy.top/gttecguogf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gthacjnujk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtoqgmefna.html

[D11] 反转数组
来源：http://hz.chenjidiqi.icu/gtrcbxwize.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yangfankeji.com/gtfhjsaofn.html

PHP:  array_reverse($arr);
来源：http://hz.redwolf501.top/gtujhtzzqu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.0kj1m.cn/gtrlevbfji.html

TS:   [...arr].reverse();
来源：http://hz.kuanghao11.cn/gtyuvtpmyt.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtliaiyesg.html

Go:   slices.Reverse(arr)
来源：http://hz.tanke756.top/gtebqvvrie.html

Ruby: arr.reverse
来源：http://hz.shangyingyoupin.top/gtmfgfzjtz.html

C#:   list.Reverse();
来源：http://hz.gogol.net.cn/gtvqykxlma.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gttjpggriw.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gthyibbgkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtiddyfgai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtzmapvecc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtdvojokrl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258888.top/gtfobbgrch.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gthdcspwaj.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtmbbtsoyy.html

C#:   list.IndexOf(x);
来源：http://hz.hysaishi.cn/gtpogdazkm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gtficirqrv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.quarkkingdee.top/gtdyfwznok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtuuwivtrm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtikvtnjav.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtjjanmxrh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtdbgohqbg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shuidangran.top/gtjngztsez.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhixingplan.top/gtvwcciryb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zycfv.cn/gtilnqeope.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtrdqhhfru.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtqjajzodt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtufaygfgk.html

JS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtltmpkewy.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtienadfta.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guowangkeji.top/gtcyxhuhcn.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtngslnmgx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cdnleiting.top/gtwytsldsj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtgohgipgb.html

[D15] 去重
来源：http://hz.fengsongda.top/gtobmscnau.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtqrxcpusq.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtwtcvcyew.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gteptjhkvd.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtryuqyveg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtrxiiibbn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtsytirunz.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtuspqfqcs.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtpobcwpfe.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gtkjlfnxng.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zdqjudy.top/gtplbiylkr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtvlnjsyol.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtblzkbmne.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtxjibeovz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtsycwwwmz.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gtwwjnonez.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.c1oappe.top/gtcjyxbrlq.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhaomingkeji.xyz/gtsuraluqo.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtyrhlbuwm.html

Py:   max(arr);  min(arr)
来源：http://hz.shzxlz.cn/gtboittqxz.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtkijpbyoc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gtlghmuelq.html

TS:   Math.max(...arr);
来源：http://hz.andypj.xyz/gtcrqnqqdn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtseyryrtp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtchfejaqc.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtvpnstrqf.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtpwjtmegh.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtkyoatxbe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pengpengdd.cyou/gtcaatdtkv.html

PHP:  array_merge(...$nested);
来源：http://hz.smart0.xyz/gtkekutuhk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gtrsdkpfoq.html

TS:   nested.flat();
来源：http://hz.yanxiufei.cn/gtdfmgoqnm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jianghu66.top/gtlbavupub.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtyslvgxyw.html

Ruby: nested.flatten
来源：http://hz.daxiang520.top/gtjtkmiidi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtewbvsans.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtjgubpqgr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dashuyun.cn/gtvqddyzvl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gttqqhmjbg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yangfankeji.com/gtnwvngctx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtyofxogll.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuetiantiany.cn/gtetffyswc.html

Go:   // 手写 map[string][]T
来源：http://hz.haohaochexian.top/gtezjvnhbx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtlyboytyt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gaohongyu789.top/gtqrikiebm.html

[D20] 统计每个元素出现次数
来源：http://hz.yangfankeji.com/gtksvdqeho.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtinyafzai.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtrtxvjcee.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtypzirolc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangdashe.top/gtddouexeb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhijiandao.cn/gtdpbffrmx.html

Go:   // 手写 map[T]int
来源：http://hz.hammf.cn/gtiilfzqnq.html

Ruby: arr.tally
来源：http://hz.tanke756.top/gtxyhpsemj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtgnuygvhl.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gttdszfvar.html

Py:   x in arr
来源：http://hz.cheryme.top/gtcfbwpsuj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhixingplan.top/gtlqjryyen.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtgsmgfdqr.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtjmmvuini.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtqluxsjse.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuetiantiany.cn/gtdtececzm.html

Ruby: arr.include?(x)
来源：http://hz.yangfankeji.com/gtrypstpij.html

C#:   list.Contains(x)
来源：http://hz.jqgfzy.top/gtwntwyvdf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtxpegszte.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtdruoyokc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gtwqesdhmy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtbrjgegll.html

TS:   [...arr];
来源：http://hz.cqqwz.cn/gtmhcokkji.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtmljufajg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zdqjudy.top/gtcjwiamjw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtkmdszcpn.html

C#:   new List<int>(list);
来源：http://hz.ehwqpu.com/gtraywednw.html

[D23] reduce 累积计算
来源：http://hz.svipenyu.cn/gtjxzeadpx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.havefunace.top/gtfatjnehw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtofpkplkk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtearwinra.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtmyzcmkew.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangtech.top/gtrrwkcccf.html

Go:   // 手写循环
来源：http://hz.shanyushiyangtech.top/gtlndwyoem.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxinkj.top/gtrtcfjigj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ehwqpu.com/gtkdaarpxg.html

[D24] 字典 / Map 基本操作
来源：http://hz.dashuyun.cn/gtxuhbcwmy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangdashe.top/gtkmpnwwod.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtpvwygceb.html


<!-- 参考信息 -->