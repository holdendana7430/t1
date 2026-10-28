代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zdqjudy.top/gtqqjanqwl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtolwbvluh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtvrswvpac.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtddgbaiwl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yongpay.top/gtaauxboui.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gtyrxlmthh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gthspauiij.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtlrigdlit.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtssreejpo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gtuojtbgat.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhaomingkeji.xyz/gtnfnwxolu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtohlmnmec.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gtfpibkubg.html

Java: 方法内为块级作用域
来源：http://hz.chenzaomai.com/gtsdwszwsx.html

Go:   花括号块级作用域
来源：http://hz.smart0.xyz/gtvxadxwye.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtegmrurtn.html

C#:   块级作用域
来源：http://hz.yj20258888.top/gtrzkcuwoy.html

[C11] 模块导入与导出
来源：http://hz.hywenlv.cn/gtnorhaagw.html

Py:   from module import func
来源：http://hz.yuxming.cn/gteygubibt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtyihsijkl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gtjakposlr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhixingplan.top/gtiogpzcad.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtljicrcur.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gtcrbceqxu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guannengcc.top/gtrzjsrdzo.html

C#:   using System.Text;
来源：http://hz.nwbrower.top/gteitfwhgr.html

[C12] 立即执行函数 IIFE
来源：http://hz.xinyue.icu/gtbalnyjrx.html

Py:   (lambda: print("run"))()
来源：http://hz.aibaodan.cn/gtkvdglhks.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtwlsbflfk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtjbkplfjn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gtnzrocixv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sysykeji.top/gtwevpymrb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtbzqleyyj.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtmruluftg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gtbtuotazr.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhaomingkeji.xyz/gtbzgoxcze.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gtrdixdrvk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtcadqcyxy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangtech.top/gtkapjlgnu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtvzudnjdk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtbdfesyxj.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtodeptqzw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sufxvd.cn/gtfidempmn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daria6918.cn/gtkjjnumfu.html

[C14] 泛型函数
来源：http://hz.shanyushiyangkeji.top/gtfjhlckwj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydzc1.top/gtpleqjvvv.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtymqkowxq.html

JS:   // 无泛型
来源：http://hz.snrcjt.cn/gtxtttqeqh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtjvjvvldt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnqzz.top/gttpwbjfjo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuanzx.com/gtafaxfqmw.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtevfprfqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtxsfyqcme.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtvixcswxg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtgamenzql.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydzc1.top/gtxkuxzxyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtnuivmqfi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gtfvvkimcg.html

Java: // 无解构
来源：http://hz.jinqigfzy.top/gtxufcsnve.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtbeivthpp.html

Ruby: a, b = pair
来源：http://hz.nanxinkj.top/gtyeodihca.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtocnqxsgp.html

[C16] 函数 / 方法重载
来源：http://hz.guowangkeji.top/gtghenmyst.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtwrbfpkfn.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtnupesbuc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtlmdhtcek.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtdonmtsiz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fengsongda.top/gtpyrajxbq.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtakgrybmf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtuhebcpmu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtpbixfcvf.html

================================================================================
来源：http://hz.yonumen.top/gthwdsgqlr.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtrjfnbuti.html

================================================================================
来源：http://hz.hfpthk.cn/gtkhvbjpig.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtfovzgmyv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shuidangran.top/gtdrsqavyn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtroirkoou.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.0kj1m.cn/gtfvmhrvok.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fzhhl.top/gthdemozbg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tian-w.cn/gtmapxsvpp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhoulong.xyz/gtajsrherv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtwytbpsqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gthrsvkqlb.html

[D02] 追加元素到末尾
来源：http://hz.fengsongda.top/gthmxlbbwy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtuscfqauu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtbaqolzuk.html

JS:   arr.push(4);
来源：http://hz.tanke756.top/gtzejcuuyi.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gtlnrcxanr.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtsgvoseop.html

Go:   arr = append(arr, 4)
来源：http://hz.cucudq.cn/gtdslkfomu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtbshgjfqj.html

C#:   list.Add(4);
来源：http://hz.cqqwz.cn/gtunmfcysv.html

[D03] 在指定位置插入元素
来源：http://hz.chenjidiqi.icu/gtxyxkdgdc.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtdowtfqlk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guannengcc.top/gtzkeihmmr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtipnrgdfh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtyzbjvkef.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtgcmgpzrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gtkhhaoxxw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daria6918.cn/gtvjejibrk.html

C#:   list.Insert(0, 0);
来源：http://hz.mhx1999.top/gthoyzshtv.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtlbscnvrp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gthldvlfxe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangkeji.top/gtlukurhiz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xingfuxueyuan.xyz/gtupwhoqfs.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtkqhmbomi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cqqwz.cn/gtryfrhyfu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gtogfaazqt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daria6918.cn/gtdaqkbxxq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtfrgtgwwd.html

[D05] 访问与修改元素
来源：http://hz.chenzaomai.com/gtuzxiogap.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtkxbcijmd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtqbwqfyaj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gtrojntsha.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenjidiqi.icu/gtahxxajzg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sxryk.cn/gtxlviveph.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.daxiang520.top/gtpufbildq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtfgpgmnqe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtpnjdzoxc.html

[D06] 数组长度
来源：http://hz.ywan-chungtsiang.top/gtvqlyxazs.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtsmhaooog.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtuzyznxlf.html

JS:   arr.length
来源：http://hz.cdnleiting.top/gtoqhrqsdk.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtoanvguph.html

Java: list.size();
来源：http://hz.hammf.cn/gtwfvdkoxy.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gtggmxsbeo.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtbeiguyoo.html

C#:   list.Count;
来源：http://hz.jianghu66.top/gtughgxcvj.html

[D07] 切片 / 取子数组
来源：http://hz.c1oappe.top/gtjyciqsny.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pengpengdd.cyou/gtvgxgmwnu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gtakjofswa.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtgrzqguth.html

TS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtpbxmzvyj.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtqvwvmvpx.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gttdqzpdyq.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gttknxrtan.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtqzdvsfrq.html

[D08] 合并两个数组
来源：http://hz.zdqjudy.top/gttffwzgsi.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gtnuhzgyuo.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gtbnduveop.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzhubu.top/gtozibhxnl.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtxpzwotrp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jiagoushi.top/gttfxlragg.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gtestnhwlq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtznpgjuwr.html

C#:   a.Concat(b).ToList()
来源：http://hz.shzxlz.cn/gtcezypxii.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtsbbpwkfo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gthtcgvdgm.html

PHP:  sort($arr);
来源：http://hz.ivvv.top/gtyfdhbnsq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gzhubu.top/gtjyebkpgb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.meibo888.top/gtjrfqcaqs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dashuyun.cn/gtkyfbrpbl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtflqwurek.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtbotpvbrs.html

C#:   list.Sort();
来源：http://hz.iojbl.cn/gtrlliepbn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xinyue.icu/gtpoftpauh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.c1oappe.top/gtpbfwwiij.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtibkzswty.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtbzjerxvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtmytswhvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hfpthk.cn/gtgqugcxln.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gotoacloud.top/gtspxxbfhw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gtnboufdob.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtovvwyxin.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gthbbxzyjp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtdzvlaohc.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtcranhbky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtladjwtge.html

TS:   [...arr].reverse();
来源：http://hz.cucudq.cn/gtilrwuhmb.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtjdbgjnld.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtreoqrkgu.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gthqviogfh.html

C#:   list.Reverse();
来源：http://hz.jinyuanbaomall.cn/gtttuznykv.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtdtbmmjzm.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gtwkfqctxl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hysaishi.cn/gtnrmslbgp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gttmyxddis.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtdlqbdfxj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtrfksrykp.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtlrinmohu.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtjbumrequ.html

C#:   list.IndexOf(x);
来源：http://hz.meibo888.top/gtzrpaxbce.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cashguo.top/gtysplgxav.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.0kj1m.cn/gttlryizsv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtlvsptfuu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtyckudimo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtlqwmtret.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bjfxy.top/gtsdbxspic.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gteoomovjc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gtgbrxijju.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gtdhwnubyc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtlsmbnobs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtlcsohmog.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhongyouzk.top/gtepjpdknc.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtxboxeqrs.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtkdbrvnjq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtyfhnbxim.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtiabyquht.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtnaqegmje.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtincawnyz.html

[D15] 去重
来源：http://hz.guannengcc.top/gtkymmycbd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtnxyeeady.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtroidyzsv.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtvrmoktqb.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtezysxbwf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aizwys.cn/gtiawfvxxt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sufxvd.cn/gtaqlfpnxu.html

Ruby: arr.uniq
来源：http://hz.gotoacloud.top/gtgoeiihhc.html

C#:   list.Distinct().ToList()
来源：http://hz.wangdashe.top/gtkfampysd.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtrordjwos.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.52xcode.cn/gtvhmjwkuj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hywenlv.cn/gtojqeslxh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtadjkkyfu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtahyjfcru.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtbmnhzytp.html

Go:   // 手写循环累加
来源：http://hz.yanxiufei.cn/gthqcuedzr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dashuyun.cn/gtkmufjdqn.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtnlfhlzwi.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtbjgozbux.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtllhyoeqn.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtnajxtwxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtwuksrfcl.html

TS:   Math.max(...arr);
来源：http://hz.jyoumei.cn/gtgnkmodju.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gtltttssmm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yvedp.cn/gtfklcocba.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gtkzvfstbv.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gthtzdweid.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtuowcrlty.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shangyingyoupin.top/gtkqtlocyw.html

PHP:  array_merge(...$nested);
来源：http://hz.yonumen.top/gtdbwermuq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtywtaaamw.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtutmwecdw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangshuangyany.cn/gtaixnngru.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtrmjavcpk.html

Ruby: nested.flatten
来源：http://hz.ywan-chungtsiang.top/gtruuekjim.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.quarkkingdee.top/gtypplveco.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtqlhkjvvx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtfbzatytm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtweifdypz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.svipenyu.cn/gtjemsbjrg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtvjnarjaq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pengpengdd.cyou/gthcoebjnv.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtiqayqzmd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtwpeyojgw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtgrtdyusc.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtqgkoalmi.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtuzedzdmi.html

PHP:  array_count_values($arr);
来源：http://hz.zhiwuduotai.top/gtojnuucmv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtqbshffah.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtfrhzvlwh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gtdxixirfp.html

Go:   // 手写 map[T]int
来源：http://hz.guowangkeji.top/gtrtvoaadv.html

Ruby: arr.tally
来源：http://hz.sufxvd.cn/gtqaaacrdl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtusdftzfe.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtnoxaziwa.html

Py:   x in arr
来源：http://hz.yanxiufei.cn/gtzosruabb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtadjjiqxe.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gttkjtumrz.html

TS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtxwkkuplu.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gtyzvbakxu.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gttirrysgt.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtavdcmpay.html

C#:   list.Contains(x)
来源：http://hz.svipenyu.cn/gtuahycyuk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zycfv.cn/gtdzfzhkba.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dashuyun.cn/gtjgaoizot.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtqjcqgxpd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhongyouzk.top/gtbxbmyzpc.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtsxpobsqs.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gtjlgseqcn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gtshfnrask.html

Ruby: arr.dup;  arr.clone
来源：http://hz.c1oappe.top/gtaozgdoue.html

C#:   new List<int>(list);
来源：http://hz.vqdsnc.cn/gtwgnuxaus.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtgtcfcwnl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtchrsfchh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtjakkrlup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtblzjgivq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtphthixhg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ivvv.top/gtknteoxwr.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtzikvgzop.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shangyingyoupin.top/gttgsjfyib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtvstoolfa.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtwqazokkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtlfniecdm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zycfv.cn/gttlmdrgnb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ehwqpu.com/gtmmtrldgf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jiagoushi.top/gtzdnzcawj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtvvpkavlk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtzvfqmurb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtnbjakkqf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ivvv.top/gtinnrkdro.html

[D25] Set 集合去重与交并差
来源：http://hz.yueranfly.top/gtkvtigbqu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtvjnbqemx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sweek.top/gthdxbxeku.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenjidiqi.icu/gttkncgpwx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gttxqnvhdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtcjnnhkiq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jyoumei.cn/gtginyyjxl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hammf.cn/gtrrsrcjkm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtdnxoyqoc.html

[D26] 数组转字符串
来源：http://hz.hywenlv.cn/gtmsvkxfnc.html


<!-- 参考信息 -->