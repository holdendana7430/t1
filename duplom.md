代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhijiandao.cn/gtghfexopj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhiwuduotai.top/gtvtztnnxk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gthchnlbca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhixingplan.top/gtklzblhcj.html

[C10] 变量作用域
来源：http://hz.feifeiyinyue.top/gtihqefuxi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtqosznvmu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnxiangtu.top/gtqvrvbpdy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtyjnkdlmw.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtratdlvtq.html

Java: 方法内为块级作用域
来源：http://hz.jinqigufen.top/gtjdlielns.html

Go:   花括号块级作用域
来源：http://hz.ehwqpu.com/gtxdlqkywa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.iojbl.cn/gtkwqvqfjs.html

C#:   块级作用域
来源：http://hz.fengsongda.top/gtkcdtbzea.html

[C11] 模块导入与导出
来源：http://hz.cashguo.top/gtyyxqaysz.html

Py:   from module import func
来源：http://hz.birdmap.top/gtuegzjyvx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydjk.org.cn/gtyrxttibj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtctxvooee.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hfpthk.cn/gtjtskjyhs.html

Java: import java.util.List;
来源：http://hz.vqdsnc.cn/gtasjwnbvk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yvedp.cn/gtfqtzvlzr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtqurrokpi.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gttvmcgupx.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtjevjxdav.html

Py:   (lambda: print("run"))()
来源：http://hz.xuetiantiany.cn/gtnxvyfyeb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtdarjhmkz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.pycfn.com/gtpukihoyv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtnpzkeyui.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.kuanghao11.cn/gtasouskit.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtcuglurrn.html

Ruby: -> { puts "run" }.call
来源：http://hz.guowangkeji.top/gtzseavonv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtykxjzhsl.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtrbccfieo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtbzvxpmet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtxzerlxmd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtpdettjkw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtpgmanpcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtmzyksune.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtjwuceeaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gttbmhkwtp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.9152youxi.cn/gtieumfftg.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtmhzdeyqi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.9152youxi.cn/gtunbxuynx.html

PHP:  // 无泛型
来源：http://hz.shangyingyoupin.top/gtllksjdgb.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtozmizyqj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gtfbwhqlha.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.dashuyun.cn/gtkpgfdovd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shangyingyoupin.top/gtftgwonje.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtbphtwwoa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.316326.xyz/gtyvyuvgum.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtpyrmdiix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yangfankeji.com/gtzboehwxl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cdnleiting.top/gtfodvfzkc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhaomingkeji.xyz/gtrwnswfwr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gtuhpehmgp.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtblvakzmo.html

Go:   // 无解构
来源：http://hz.sufxvd.cn/gtaonqhnzl.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtjxcqzstj.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtgkyenjyo.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtrrznprdk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sweek.top/gtigadgngx.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gtcuwucili.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtmhylkcsv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jianghu66.top/gtkfushfdq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cheryme.top/gtfieiodpt.html

Go:   // 无重载：用不同函数名
来源：http://hz.9152youxi.cn/gtzcpvmitb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtezxtzbae.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zycfv.cn/gtkycnezpk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtobxbtrin.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtswjjacuy.html

================================================================================
来源：http://hz.bjfxy.top/gtijfyttyl.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtucnhmngx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.0kj1m.cn/gtksszmuyx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtpwayvmdl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shangyingyoupin.top/gthocuyrmi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.fengsongda.top/gtuhyumceu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jyoumei.cn/gtjnzpivzv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtouszvubj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gtrgyapdto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nanxuanxn.top/gthakgfbem.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtsandjjly.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtpyfoxyav.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtkmvexjtd.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtqfjgdugz.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtqyzklzsf.html

Java: list.add(4);
来源：http://hz.xuetiantiany.cn/gttocfheup.html

Go:   arr = append(arr, 4)
来源：http://hz.ywan-chungtsiang.top/gtklcuagqz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yueranfly.top/gtimkxdgsh.html

C#:   list.Add(4);
来源：http://hz.0kj1m.cn/gtqphficye.html

[D03] 在指定位置插入元素
来源：http://hz.hnxiangtu.top/gtysgydffn.html

Py:   arr.insert(0, 0)
来源：http://hz.9152youxi.cn/gtzzccpqdm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gthyieifel.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jlsjyb.cn/gtnzdcqgcl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenlongwang.top/gtvebqibdd.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtcsqxrobt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtthtlcoxc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tianlin.xyz/gtcwovielv.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gtxouukpys.html

[D04] 删除元素
来源：http://hz.ydjk.org.cn/gtzerxvtnx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtkpdfugtc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtpaziqleo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yanxiufei.cn/gtszudfohw.html

TS:   arr.splice(0, 1);
来源：http://hz.hnxiangtu.top/gtquxbbwjd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenlongwang.top/gtydklbvlw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtjqibbegq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zdqjudy.top/gtoklcutet.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtpdugnioj.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtlskbiytr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gttkjmmise.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gtyzetuilr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gturfscvvu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtflfhzaqb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhaomingkeji.xyz/gtggesmqmy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtznlffiyg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtibnffcpd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gthhoktakc.html

[D06] 数组长度
来源：http://hz.kuanghao11.cn/gtwkxaddbz.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtzarqoiiw.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtfaltrdnj.html

JS:   arr.length
来源：http://hz.yj20258888.top/gtfqfeudrx.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtwzxrdnkd.html

Java: list.size();
来源：http://hz.shangyingyoupin.top/gtxpumymhv.html

Go:   len(arr)
来源：http://hz.cheryme.top/gtqvyvbtqi.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtswodoohn.html

C#:   list.Count;
来源：http://hz.sweek.top/gtzmoplxez.html

[D07] 切片 / 取子数组
来源：http://hz.0kj1m.cn/gtcwzqglry.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtrumbznra.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hammf.cn/gtrfquvpep.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtbvafrekv.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtjpnckrgv.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtvlemptlf.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtwyyfmczb.html

Ruby: arr[1, 3]
来源：http://hz.cqqwz.cn/gtqwqyikpy.html

C#:   list.GetRange(1, 3);
来源：http://hz.316326.xyz/gtmbiofibg.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gthienumen.html

Py:   a + b;  a.extend(b)
来源：http://hz.sysykeji.top/gtnauhfipb.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtknvwdoek.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhengqikj.top/gtbjngeaml.html

TS:   [...a, ...b];
来源：http://hz.hammf.cn/gtkftvrols.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtnpjkazrl.html

Go:   append(a, b...)
来源：http://hz.sxryk.cn/gtegqkbgly.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtizxphvid.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhengqikj.top/gtiriatvll.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gtkrptqqfu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtepufvlbm.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtbnipzgun.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtpyzufppw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtdmtqqjct.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnqzz.top/gtwqlwfucc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtpabnhzoi.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtnqmahlye.html

C#:   list.Sort();
来源：http://hz.nanxinkj.top/gtwomscomr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yongpay.top/gtddoejpyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtfzpnrgkg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sweek.top/gtcvqszpeo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtximgrwkg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtoalvwcsi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ehwqpu.com/gtuxwwnvtz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gtbtnaztve.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtcqcqphiu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.snrcjt.cn/gtgcwqkzvm.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gthpfagflr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtzphtdlfu.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtqscctvxp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gtlplqjvui.html

TS:   [...arr].reverse();
来源：http://hz.mhx1999.top/gtcdcupyxt.html

Java: Collections.reverse(list);
来源：http://hz.yj20258.top/gtflpvfbps.html

Go:   slices.Reverse(arr)
来源：http://hz.ppjwa.cn/gtcvytafpu.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gtyyyuyzqe.html

C#:   list.Reverse();
来源：http://hz.c1oappe.top/gtrrfefxik.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtfhtabypp.html

Py:   arr.index(x);  x in arr
来源：http://hz.gzhubu.top/gtzuxmvcih.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gzhubu.top/gtndalehyn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gtdbcnurfj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtflzszzjn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hfpthk.cn/gtkodmqthl.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gttactcvcb.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtpsvhesxe.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtfbzxymse.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtblkhlurj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gtmntlcuzn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sweek.top/gtfwqlkcgi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtqcpecaip.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtjosjnqaq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtgznainzo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gtagufuvni.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtpauiybve.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtgoopxhey.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtdodguiqk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dianchejie.cn/gtscqfkjqo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinghuilouyu.cn/gtjvrcnesv.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtalyjjypm.html

TS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtkflkdliy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtacwetaot.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtopkyyuag.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hywenlv.cn/gtsjsdpogb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guowangkeji.top/gtalfwzten.html

[D15] 去重
来源：http://hz.shanyushiyangtech.top/gtxahznjco.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtwgialmtq.html

PHP:  array_unique($arr);
来源：http://hz.haohaochexian.top/gtdwymwfjp.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gttpsskbtx.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtfbmjcxil.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtsudvmpig.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtuzyxatfp.html

Ruby: arr.uniq
来源：http://hz.redwolf501.top/gtrquhaezd.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtabdqsdmb.html

[D16] 求和与平均值
来源：http://hz.guannengcc.top/gtyfspadnr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sysykeji.top/gtjrzeofsp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtijvuxtpb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtdqrsrrgp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtmgpwbxab.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxuanxn.top/gtdffbedgm.html

Go:   // 手写循环累加
来源：http://hz.xziqi.cn/gtbliumrlu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtusgpzbxx.html

C#:   list.Sum();  list.Average()
来源：http://hz.guannengcc.top/gtphhkykyq.html

[D17] 最大值与最小值
来源：http://hz.yanxiufei.cn/gtrvuezxwd.html

Py:   max(arr);  min(arr)
来源：http://hz.aizwys.cn/gtfkaimmel.html

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtdaqfgosp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtnobrhxws.html

TS:   Math.max(...arr);
来源：http://hz.tian-w.cn/gttrrnlrev.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtzkhncudi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.andypj.xyz/gtugjbehiu.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtfibpbkza.html

C#:   list.Max();  list.Min()
来源：http://hz.zdqjudy.top/gtvbcwqvur.html

[D18] 扁平化嵌套数组
来源：http://hz.smart0.xyz/gthtjiypot.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xziqi.cn/gtqimfqrni.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtapigshia.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtvitgmdin.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gtdiromipl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gtaiftlrjo.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtklckepfi.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtjoryypul.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sufxvd.cn/gtssifjjir.html

[D19] 按字段分组
来源：http://hz.ydjk.org.cn/gtbmfnwgpd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtgelxadum.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtzplntdum.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ybcxt.top/gtpfiotagz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gttpboaqpx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtaptztvak.html

Go:   // 手写 map[string][]T
来源：http://hz.yuxming.cn/gtqszrmjsh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yonumen.top/gtaqxepfrp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtpepxtpgm.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtfvtshefa.html

Py:   Counter(arr)
来源：http://hz.tian-w.cn/gtcyuccwhr.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gtxhaulrfz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtcqouqegg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtqlcmugjt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtmeuhdlch.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtqjretnpv.html

Ruby: arr.tally
来源：http://hz.jinqigufen.top/gtfzjebnao.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtvyxbvnks.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtbleceytw.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtcfugwafd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jiagoushi.top/gtehavhgrr.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtunrwkfsn.html

TS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtkltfltsk.html

Java: list.contains(x)
来源：http://hz.shzxlz.cn/gtctghykse.html

Go:   slices.Contains(arr, x)
来源：http://hz.xziqi.cn/gtqqpghkgw.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtxmdkobbf.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gthagcagja.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtjgkblttp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtcpuwdwss.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtbmpcvsao.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinyuanbaomall.cn/gtyhvubawb.html

TS:   [...arr];
来源：http://hz.chenlongwang.top/gtvuvubwaz.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtmccbgfdx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gtcwcqtfoz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtcctcuejl.html

C#:   new List<int>(list);
来源：http://hz.chenjidiqi.icu/gtksypizqc.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtgfwfequp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtfzpuzljq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fengsongda.top/gteqizehdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtqoumhrgi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtybpufoam.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gthxaeufbp.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gthlisllox.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sufxvd.cn/gtwrqbiavr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtaeplfuan.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gtgsbhxdri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtrfyhknto.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtjxjjbvwm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtykvyutfb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnqzz.top/gtbsuirduz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtugiseadl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.birdmap.top/gtesxyqeeg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxuanxn.top/gtcondjtxl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtrwuujwhh.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtybcvjinb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtkxxxefsn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtgctfidky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtbzapotdc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtzesmfvyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtrkwlhhzi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtuvevwinl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.bjfxy.top/gtewurzyon.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtmllrzqrx.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtpbbctbxd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.52xcode.cn/gtylkfrpxy.html

PHP:  implode(", ", $arr);
来源：http://hz.zhoulong.xyz/gteruycrto.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtqtanqifl.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtppijhnli.html


<!-- 参考信息 -->