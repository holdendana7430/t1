代发 wailian999

[C10] 变量作用域
来源：http://hz.yvedp.cn/gtyeiznepl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtjnxvzkxv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtnirrrlqq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ehwqpu.com/gthzpvlwis.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtopruzhcw.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gtxadjqnbe.html

Go:   花括号块级作用域
来源：http://hz.dianchejie.cn/gtslcqrfag.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtayfefuvn.html

C#:   块级作用域
来源：http://hz.haohaochexian.top/gtospwtmnn.html

[C11] 模块导入与导出
来源：http://hz.shanyushiyangkeji.top/gtzezzsohc.html

Py:   from module import func
来源：http://hz.jlsjyb.cn/gtxxexaqhb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtpuzoownz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.iojbl.cn/gtsjrpjtuc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtbakpwfiw.html

Java: import java.util.List;
来源：http://hz.zhiwuduotai.top/gtvdhykfzj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258.top/gtpuehxdjk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenlongwang.top/gttgoarmfb.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gtzycdylvn.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtuekmiepa.html

Py:   (lambda: print("run"))()
来源：http://hz.bjfxy.top/gtpvicxhac.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yonumen.top/gtlpwkikdb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtxxthkuyc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtshnymupp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtnrowtnvk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jianghu66.top/gtdwswahod.html

Ruby: -> { puts "run" }.call
来源：http://hz.xinyue.icu/gtziiwuguw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gtllozszfe.html

[C13] 类型声明 / 类型注解
来源：http://hz.shangyingyoupin.top/gtulivvoyp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gtcztgzxgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtdkazsyie.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gttyldjrtv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtjuipbbyg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtkhysqmjg.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtrwtsibse.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtrqtycbgx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtpjokzcxv.html

[C14] 泛型函数
来源：http://hz.tanke756.top/gtcseivyrj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.snrcjt.cn/gtzabzeozz.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtnuaydzck.html

JS:   // 无泛型
来源：http://hz.c1oappe.top/gtucmyzjop.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gtwpjviles.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydjk.org.cn/gtjgoezqwo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daria6918.cn/gtarvxhhod.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtxtlypbjs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtbwyrrqfe.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gtvarpcyaf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yvedp.cn/gtrxmwgumu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gteistyzuu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtauwsxbgo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtygxpnqvr.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtrblarzeo.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtrompwqav.html

Ruby: a, b = pair
来源：http://hz.c1oappe.top/gtpuxukerl.html

C#:   var (a, b) = pair;
来源：http://hz.shzxlz.cn/gtjghjufuh.html

[C16] 函数 / 方法重载
来源：http://hz.wangdashe.top/gtkwfytpmf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aibaodan.cn/gtefltssca.html

PHP:  // 无重载
来源：http://hz.wangshuangyany.cn/gtkzzggdgz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtduerxqej.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gtfaybagkq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.quarkkingdee.top/gtesenfaez.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinghuilouyu.cn/gtkndicpzp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtzzdreths.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hywenlv.cn/gttngirshm.html

================================================================================
来源：http://hz.yueranfly.top/gtzrwjfcym.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gtfvjexdpf.html

================================================================================
来源：http://hz.fzhhl.top/gtcxqbvqhh.html

[D01] 创建数组 / 列表
来源：http://hz.iojbl.cn/gtfximvusn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.havefunace.top/gtamcwqgoy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gthiwgmpbm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.quarkkingdee.top/gtzcowzujy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuanzhike.top/gttusjlhfb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.bjfxy.top/gtfcccvcyu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtojnopixj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtlcvofshg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cqqwz.cn/gtgoksfvze.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtuzpgrlja.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.snrcjt.cn/gtgjxnnqkv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangdashe.top/gtwdeflhxj.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtyvetwsux.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtdgomcvgy.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtazgqzmtf.html

Go:   arr = append(arr, 4)
来源：http://hz.fengsongda.top/gtkzsktpzk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtvhalahmp.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtgjguxojm.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gtwdolbwki.html

Py:   arr.insert(0, 0)
来源：http://hz.yuanzhike.top/gtptfevwdx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gthtiqspqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtwtmonvya.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.mhx1999.top/gtubnqowxx.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtauacnazu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhiwuduotai.top/gtjawhtgbd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtciedjrcy.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtnqmivkki.html

[D04] 删除元素
来源：http://hz.feifeiyinyue.top/gtjbkjdfwb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtpppjwiua.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtduthhizk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shzxlz.cn/gtdfovvcdp.html

TS:   arr.splice(0, 1);
来源：http://hz.tanke756.top/gtwtouvxvt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.guannengcc.top/gtkkvgxpqf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tian-w.cn/gtfoapaypx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sufxvd.cn/gtqddccegx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgufenzy.top/gtdmvyuqni.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gtavplywsn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtbclnweld.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gtrhfcfrux.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtcxfkoflr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ehwqpu.com/gtfssupecd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shangyingyoupin.top/gtjfdggjqh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.9152youxi.cn/gttclskano.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtldbrwrvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guowangkeji.top/gtcramdvlr.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtagescvgc.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtlmbslxtr.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtsodqoubr.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtccrpeyfb.html

TS:   arr.length
来源：http://hz.mhx1999.top/gttbqdudvk.html

Java: list.size();
来源：http://hz.mhx1999.top/gtxhumjpyl.html

Go:   len(arr)
来源：http://hz.hammf.cn/gtkolveocr.html

Ruby: arr.length; arr.size
来源：http://hz.gogol.net.cn/gtqfmnffhz.html

C#:   list.Count;
来源：http://hz.daxiang520.top/gtdhzjhurk.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtnmzdjyhc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtzongekhz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtjugislow.html

JS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtxlmwfwcw.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtenqhcuvs.html

Java: list.subList(1, 4);
来源：http://hz.ydzc1.top/gtczodwdtb.html

Go:   arr[1:4]
来源：http://hz.xziqi.cn/gtfzytssqu.html

Ruby: arr[1, 3]
来源：http://hz.chenlongwang.top/gtebyjpxfe.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gtjrwgobxm.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtfxjdfcaq.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtwbvzhksd.html

PHP:  array_merge($a, $b);
来源：http://hz.yueranfly.top/gtjhjmafxp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenjidiqi.icu/gttmyhcpeh.html

TS:   [...a, ...b];
来源：http://hz.nanxinkj.top/gtycdbsvzi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtlrrhvkur.html

Go:   append(a, b...)
来源：http://hz.pengpengdd.cyou/gtammvqcxz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtdpfermsa.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtshtlnksd.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtrcmhvhne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtmezgwadv.html

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtkvqzpknk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aibaodan.cn/gtbjikvxju.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yongpay.top/gtdiuiarjz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gttxsskiit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtnpndyfyi.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtlvpcxtgw.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gtqulkaqio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gterntldak.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtxsedvnqi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtogysmbvj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtnpjgredr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtpbvcspjl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gthbmxzbxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.9152youxi.cn/gtowlrwrea.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtpzkrccab.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangkeji.top/gtqnxxgkfi.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtaeskczht.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtnhocyksi.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtzfnpldog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtmjpyjszr.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtaokgllmx.html

Java: Collections.reverse(list);
来源：http://hz.feifeiyinyue.top/gtoetmqoem.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtmmuuwoxe.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gthstcejoy.html

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtftvqgtfq.html

[D12] 查找元素下标
来源：http://hz.sweek.top/gtttuhqgkr.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtfnsujsej.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtqifpuenp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghu66.top/gtsvgnmxsc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtvemmsfzt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gthbszagwa.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtuqrblvow.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtexbzvitt.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtvjklqync.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgufenzy.top/gtvprwoyhf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fzhhl.top/gtbtenuqno.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gtuxsawbqv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtlztulshh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtjhqcvehv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jiagoushi.top/gtopvrkixu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtffutvipr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cucudq.cn/gtpllqlrsv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangkeji.top/gtnpoktift.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hongshengwenyu.top/gtaxsnfiwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shzxlz.cn/gtkasvpmsa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sxryk.cn/gtqufvasqk.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtreqqixzh.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtlynufwjx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtoszdywva.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtkpfbcqjq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtaslieiib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fengsongda.top/gtxigdqzsr.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtasnamsex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gttdydzgun.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtphakizgl.html

JS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtwpuvypoj.html

TS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtikrqelsl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gthauwybsp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daria6918.cn/gtrkkgkrgf.html

Ruby: arr.uniq
来源：http://hz.cucudq.cn/gtqhtpkdry.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtmfvoozpy.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtjowejbcd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtqvlxawil.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtgzgucbxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtkxvhssis.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtjtjarooa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtllgibqvp.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gthanzjdbw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenzaomai.com/gttjxnfcsw.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtmcaviwbi.html

[D17] 最大值与最小值
来源：http://hz.cashguo.top/gtinpsijrg.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtizrqaylw.html

PHP:  max($arr);  min($arr);
来源：http://hz.fengsongda.top/gtrvhpounx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sufxvd.cn/gtxwjxlyal.html

TS:   Math.max(...arr);
来源：http://hz.zhixingplan.top/gtwmxkcucr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gttzstkcsz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ywan-chungtsiang.top/gtgssmqhxg.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtpfkkigui.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtdhdldktd.html

[D18] 扁平化嵌套数组
来源：http://hz.feifeiyinyue.top/gtzugailxg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gtsfblnwxu.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gterqeatzm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gtfzvaxvka.html

TS:   nested.flat();
来源：http://hz.yonumen.top/gtnqxtcbnc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gtlkpthmrd.html

Go:   // 手写双层循环
来源：http://hz.nanxinkj.top/gtgqvkloar.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtojoevwgj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtntljetwg.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtyngocnsk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xinyue.icu/gtkccqixai.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gtxlrxbguj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.svipenyu.cn/gthrpqayqe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtjahoousm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuanzx.com/gtnfddemvt.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtudrenodt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtmotjmgoy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtxqhszuug.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtoubmgbud.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangtech.top/gtcchuekkk.html

PHP:  array_count_values($arr);
来源：http://hz.jinghuilouyu.cn/gtmizqfvio.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtqyhwhugg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtoqqmzzsp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenlongwang.top/gteaprvhjs.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtrhbgqzyx.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtklgqubfj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtbebmfyaf.html

[D21] 判断是否包含某元素
来源：http://hz.chenzaomai.com/gtjcmhujrk.html

Py:   x in arr
来源：http://hz.jianghu66.top/gtprvuiucv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtwkxephrq.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtotysflav.html

TS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtxqwuyyud.html

Java: list.contains(x)
来源：http://hz.yangfankeji.com/gtaoobneeb.html

Go:   slices.Contains(arr, x)
来源：http://hz.sxryk.cn/gtjteipakz.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtmpxlqiux.html

C#:   list.Contains(x)
来源：http://hz.daria6918.cn/gtihnyehjy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.bjfxy.top/gtgjfyijpz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtmnxqgszr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhaomingkeji.xyz/gtcnerappq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gthllpretp.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtkpruvejz.html

Java: new ArrayList<>(list);
来源：http://hz.iojbl.cn/gtjbzkwzop.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuanzx.com/gtggpjbmzm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtayhitptj.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtslankkme.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtcpusdvjq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtwuaydtgj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtehlhwidd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtjndscnrw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtrwdafdhh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dianchejie.cn/gthcuscpzp.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtjskogqeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xinyue.icu/gtvsiswvyz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydjk.org.cn/gtqckxqkhu.html

[D24] 字典 / Map 基本操作
来源：http://hz.cdnleiting.top/gtbtreftxx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtlxpzwcku.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtsnwqlfqr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtoogepgsd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtsbbjxlhv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aizwys.cn/gtdxcurnys.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtirugvexb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gtwewqypfc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hysaishi.cn/gtmrivuizf.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gtkwjyhtsw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydjk.org.cn/gtsscsqdth.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtqhpgkjaw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtxeowwmbx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shzxlz.cn/gtnbgrhvlg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtbsyocfai.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtqvpuaweu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aibaodan.cn/gtrhbhubzf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gtyfhipbfc.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtwrnzloec.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtrubwqgnw.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigfzy.top/gtuotyfzct.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtdmfjlmdm.html

TS:   arr.join(", ")
来源：http://hz.daria6918.cn/gttcytxrjc.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtauhexblq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtjgsyefny.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtfkvvqezx.html

C#:   string.Join(", ", list)
来源：http://hz.hongshengwenyu.top/gtyskampls.html


<!-- 参考信息 -->