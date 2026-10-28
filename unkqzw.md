代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pycfn.com/gtafjwsoxn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhixingplan.top/gtrlwaesnv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangshuangyany.cn/gteqlvtgjm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.vqdsnc.cn/gtqvdpzeuk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shuidangran.top/gtnsmpmhco.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtpfmsuypt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hnxiangtu.top/gtrwdbehkv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtssukrdsc.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtslelgmfw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gthkapqtwr.html

C#:   f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtqigcrzsr.html

[C05] 返回多个值
来源：http://hz.ybcxt.top/gthtdrkeui.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtdqqzfbkj.html

PHP:  return [$a, $b];
来源：http://hz.dashuyun.cn/gtbcheavyo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtaipiccqs.html

TS:   return { a, b };
来源：http://hz.hysaishi.cn/gtzizvviys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtlpalsxlh.html

Go:   return a, b
来源：http://hz.dianchejie.cn/gtexzyxxmy.html

Ruby: return a, b
来源：http://hz.cucudq.cn/gtdqhliduk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.snrcjt.cn/gtnuzxepsg.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtczfzjkcq.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtheqjqnsk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258888.top/gtulwmblsj.html

JS:   const square = x => x * x;
来源：http://hz.shzxlz.cn/gtkpvxmzcf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gzhubu.top/gtsbjtyrcp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shzxlz.cn/gtjtxiitkw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gtqlntihvk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtdqxvpwdh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhengqikj.top/gtlyphcvfi.html

[C07] 把函数作为参数传入
来源：http://hz.haohaochexian.top/gtiwmwslnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtlwgytdlx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zdqjudy.top/gtfahnlpjq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtalvmbkjb.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gttghmcsfp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangshuangyany.cn/gtvaintfcs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fengsongda.top/gtugaqqmtu.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtdpomyutd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ehwqpu.com/gtfwntkvrs.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gtntgtrrig.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yvedp.cn/gtgtnzbpce.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gthfzidpea.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gthuocytgn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtnrfnttrc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.feifeiyinyue.top/gtukjmrqbu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuanzx.com/gtvdrbnaor.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxuanxn.top/gthutxliqo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtazalfdxv.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtydtxinbc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtumravjqc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtrzjkpunw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtypscjtdf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtxvayczkk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtlgfmooiy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtenvrakmf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cqqwz.cn/gtaluotygf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yongpay.top/gtikthykbl.html

[C10] 变量作用域
来源：http://hz.shanyushiyangkeji.top/gtdhtwxblw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shuidangran.top/gtfnzqlxtj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhixingplan.top/gtibowmmrs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aibaodan.cn/gtexddzpvm.html

TS:   同 JS
来源：http://hz.tianlin.xyz/gtxzaalnpo.html

Java: 方法内为块级作用域
来源：http://hz.guowangkeji.top/gtgejgjvcj.html

Go:   花括号块级作用域
来源：http://hz.cdnleiting.top/gtbktcsxgq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.52xcode.cn/gtwmmexlht.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtipbiismh.html

[C11] 模块导入与导出
来源：http://hz.yangfankeji.com/gtwprertyl.html

Py:   from module import func
来源：http://hz.jqgufenzy.top/gtjwzimzkg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtmwfwyvnl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hammf.cn/gtlqmfsbgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtitkefgcq.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtfwofnlqj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gthjhenhpb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtkmalysrr.html

C#:   using System.Text;
来源：http://hz.jlsjyb.cn/gtfnokhhmo.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gthchrnjey.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtynvyqeqz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhaomingkeji.xyz/gtpxmewppt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtohfvbaez.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtacpkpbgx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangdashe.top/gtgmhifksa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtxvixhrae.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtylmulyji.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fengsongda.top/gtujwoliac.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtakesqiji.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtwwrkwqgb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtpgraamjz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtnattnhre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daxiang520.top/gtqkohkukc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gthvgdhmsn.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtqevclweh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtehxsetfv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtarrnhtpl.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtrdnsmgnk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.haohaochexian.top/gtxxiewfxx.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtbrmuxcwl.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtneztmrfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtrddvqgyv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtsluhghct.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtwvtvbucc.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtfxnyayem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258888.top/gtngxrqhvy.html

[C15] 解构 / 展开参数
来源：http://hz.snrcjt.cn/gtodrsonxk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hfpthk.cn/gtigqgcvbn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtdsyuxsxm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtkcimsraq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtnjgbmuye.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtfkivnzvn.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtqobexcpd.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtshifgblc.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gtptmjyuyq.html

[C16] 函数 / 方法重载
来源：http://hz.hywenlv.cn/gtmznozsxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ppjwa.cn/gtohiawzlo.html

PHP:  // 无重载
来源：http://hz.pengpengdd.cyou/gtjjbsikfo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.iojbl.cn/gtxcfluexq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtxppdgvjl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtavxyrrph.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtrfukztyv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangtech.top/gtomykuhgs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtauzomydg.html

================================================================================
来源：http://hz.bjfxy.top/gtkukcqrfk.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtpnybudno.html

================================================================================
来源：http://hz.pycfn.com/gtmlcynyed.html

[D01] 创建数组 / 列表
来源：http://hz.ydzc1.top/gtnmxrnifv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cqqwz.cn/gtedbjzpdn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gttaqgepdy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.quarkkingdee.top/gtrwdakcrx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtvhhsffyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtuofgpwgr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtjqfmkbzl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtilmhydfc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhaomingkeji.xyz/gtjlopjxer.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtghoctlqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cucudq.cn/gtkgzxvgem.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtxbvznbwd.html

JS:   arr.push(4);
来源：http://hz.pycfn.com/gtvejwqjwh.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtgejbcjwg.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtrtjalhar.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gthkejupww.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtpzbolsex.html

C#:   list.Add(4);
来源：http://hz.chenjidiqi.icu/gtwlowxhtd.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtookpyfxq.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gtuhppsuhx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtudgtvsqa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gtceilvzwr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtyyetfjsj.html

Java: list.add(0, 0);
来源：http://hz.sufxvd.cn/gtmzenofjk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.redwolf501.top/gtimtegmsb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtazcjlavs.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtpqimkujw.html

[D04] 删除元素
来源：http://hz.gzhubu.top/gtqamkzdfa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gaohongyu789.top/gtwpriokhi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtpotcovdp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hfpthk.cn/gtuopajbdh.html

TS:   arr.splice(0, 1);
来源：http://hz.sufxvd.cn/gtvdedbvkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gthxigxsot.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtwnjialac.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258888.top/gttaoytblj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cdnleiting.top/gtbjjymmnu.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtcozgjwxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gthttmvbgg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jyoumei.cn/gtjqzbbgby.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cheryme.top/gtbxyqccyh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtdtoofabz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258.top/gtrjgjrixn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sweek.top/gtptxcytyf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtrwgyqofs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.iojbl.cn/gtvsgjyhwu.html

[D06] 数组长度
来源：http://hz.aibaodan.cn/gtcclzixjf.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtltyaawvf.html

PHP:  count($arr);
来源：http://hz.yvedp.cn/gtynncwqpm.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gthurfwzxl.html

TS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtpvbgrfvz.html

Java: list.size();
来源：http://hz.haohaochexian.top/gttlmmxczx.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtaxgzefdm.html

Ruby: arr.length; arr.size
来源：http://hz.sufxvd.cn/gtxokkukwt.html

C#:   list.Count;
来源：http://hz.svipenyu.cn/gtamoiwpjm.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtbkwoiqmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtnfhetjjx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtqlbyorie.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtnqjgeicf.html

TS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtchsukmli.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtnjvcolmd.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtoohvcvfg.html

Ruby: arr[1, 3]
来源：http://hz.zhoulong.xyz/gtbmozdfki.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuanzx.com/gtqnbdrlmj.html

[D08] 合并两个数组
来源：http://hz.316326.xyz/gtsvaqbadj.html

Py:   a + b;  a.extend(b)
来源：http://hz.andypj.xyz/gtjsvkzukq.html

PHP:  array_merge($a, $b);
来源：http://hz.zhixingplan.top/gtldzejmpo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzhubu.top/gtkwxgzyrz.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtsyxmdpjo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtmxdfnswy.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangkeji.top/gtryvvdoaz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtrlbckdsk.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtewmujopc.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtnotyjtuz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtxokozxkf.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtihmfzhne.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guannengcc.top/gtuvffxnjw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenlongwang.top/gtbekmwtyo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtybtgjcrd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.birdmap.top/gttotteuhb.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtoubeybmp.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gtxtkywnij.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gtlfwdjakk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhixingplan.top/gtnzevcmyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtfezvjvnq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtlaesilir.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtjekkqwwu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.dashuyun.cn/gtfxosirin.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtbwcsctgb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtyujguzvk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtxoozovyu.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtszxsyzhq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aibaodan.cn/gtnjpnzsrf.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtrqldiopi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yangfankeji.com/gtqyqjfcdf.html

TS:   [...arr].reverse();
来源：http://hz.guowangkeji.top/gtydinsvwh.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gtugjymzxf.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtckdbjknp.html

Ruby: arr.reverse
来源：http://hz.shuidangran.top/gteqwcvyov.html

C#:   list.Reverse();
来源：http://hz.xylfe.cn/gtfsnpgrjc.html

[D12] 查找元素下标
来源：http://hz.zhongyouzk.top/gtbxwxjfiz.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtqfasaaon.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtuopxrlfw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtbzojazsp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtxtsfsseo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fzhhl.top/gtxkhxpzyi.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtifrdtwid.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtkotylxjx.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtpvsefsgb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.bjfxy.top/gttuivtbjh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtskxbvsxn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258888.top/gtnybzougc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtirwqwadn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtovitlwlp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtbwijsroh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.birdmap.top/gtioducyjd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtcxhsefjj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnqzz.top/gtagfetydp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtpmwgizvz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gthqaxsuax.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zdqjudy.top/gtbsygqkao.html

JS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtgoxnflom.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtklzwtkcm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtwosrielu.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtngwflgeb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtsjhomezp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtblcfjtcl.html

[D15] 去重
来源：http://hz.tanke756.top/gtfwkfqwwx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gthegnmcyj.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtfyxdtbzm.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtknkmahok.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtfkgbpedo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangkeji.top/gtarhrvdby.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtavwpdlcd.html

Ruby: arr.uniq
来源：http://hz.cucudq.cn/gtvmrdogzj.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gtixawoadr.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtcumgzpoo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtuitwxwqs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtrwgrhjuq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtjvxiahca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtdjvydvrx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtelqpqzta.html

Go:   // 手写循环累加
来源：http://hz.jinqigfzy.top/gtjqexrbwb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtzskdlslr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtdfqrobzw.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtpvkihdfa.html

Py:   max(arr);  min(arr)
来源：http://hz.andypj.xyz/gtqmeiruxs.html

PHP:  max($arr);  min($arr);
来源：http://hz.sxryk.cn/gtbpzmeman.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtklfzbqmq.html

TS:   Math.max(...arr);
来源：http://hz.xylfe.cn/gtculhkblu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.bjfxy.top/gtpyxotwri.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtgmpezedf.html

Ruby: arr.max;  arr.min
来源：http://hz.0kj1m.cn/gtbamagyji.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtjyijrgtf.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtlrbzbvrf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtzasmbvwl.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtijqzjkno.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gtxuufirnl.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtniceprij.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtmdehxzfm.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtouesvpyz.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtlwwugqth.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtruzyjtwc.html

[D19] 按字段分组
来源：http://hz.hysaishi.cn/gtkcncnhcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gtfktyrmml.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtmsnoavxy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dashuyun.cn/gtijpckxjg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtcgxrpqse.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.meibo888.top/gtkqqosswd.html

Go:   // 手写 map[string][]T
来源：http://hz.gzhubu.top/gtutrxwkhz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtctzwuzoy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gtyeycpwyo.html

[D20] 统计每个元素出现次数
来源：http://hz.zhongyouzk.top/gttsavrohl.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtemcnkbnl.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtmbbauutb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtxkyjouxu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtdwnjxhwg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtmpcqmmlq.html

Go:   // 手写 map[T]int
来源：http://hz.wangdashe.top/gtzggzzfhv.html


<!-- 参考信息 -->