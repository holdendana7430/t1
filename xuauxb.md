代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuxming.cn/gtquxokjqr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtwvdnabyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtuuflpsqw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtjykednez.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fzhhl.top/gtldvlcpia.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtegkdkvin.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtpgswjlpa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtkaeqzjzn.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtagvdtxfo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.mhx1999.top/gtwceiggzt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daxiang520.top/gtsvkobczs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258.top/gtuluqxbgw.html

TS:   同 JS
来源：http://hz.xinyue.icu/gtnpogvvzu.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtjfuiesna.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtkxzbzwme.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenlongwang.top/gtgwxwfmix.html

C#:   块级作用域
来源：http://hz.daria6918.cn/gteegthnwd.html

[C11] 模块导入与导出
来源：http://hz.c1oappe.top/gtfgnarahw.html

Py:   from module import func
来源：http://hz.yvedp.cn/gtihjvpagy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gtbgxokrgb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtactrqvjh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtiqkgtqha.html

Java: import java.util.List;
来源：http://hz.guowangkeji.top/gtmkdekytt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtygitqlbq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xziqi.cn/gtznpbansk.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtisbazqsg.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtsczgvnxc.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtzmwzznhj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtkekjrjhh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtmfcbkant.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtyuclbfdn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.bjfxy.top/gtinyhlcjb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dashuyun.cn/gtnlotrsfx.html

Ruby: -> { puts "run" }.call
来源：http://hz.snrcjt.cn/gtrgrgotjs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gtgvztrtbr.html

[C13] 类型声明 / 类型注解
来源：http://hz.cucudq.cn/gtwwmaklth.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinghuilouyu.cn/gtrmigatjq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtjbbwjhzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtpeuhphzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gtdneabzcu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtzweamqbs.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtxinrobxc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtlmcfexib.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuanzhike.top/gtdcngcozr.html

[C14] 泛型函数
来源：http://hz.dashuyun.cn/gtivcouyzs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtddocjbsd.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtdtrboxui.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gttxerrmdd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xinyue.icu/gtclmtwkxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtshvbdbbe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenlongwang.top/gtrbrfcjsd.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtghtjftev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgfzy.top/gtbypfwrnh.html

[C15] 解构 / 展开参数
来源：http://hz.9152youxi.cn/gtxcrbdgff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gtfqihmuzg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sufxvd.cn/gtygcounrc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.mhx1999.top/gtfeulgtxq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtcqhhygid.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gtoxocoqlj.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtheixmnqr.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtdjwezemz.html

C#:   var (a, b) = pair;
来源：http://hz.feifeiyinyue.top/gtsbyuelny.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtyvloxuve.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.meibo888.top/gtwizqnfae.html

PHP:  // 无重载
来源：http://hz.redwolf501.top/gtqddgfjzf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhijiandao.cn/gtlpnycvij.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenlongwang.top/gtiavoramw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydzc1.top/gtdwrbdrqh.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtytrmzlpy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gteujwnzam.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xinyue.icu/gtpegnlscm.html

================================================================================
来源：http://hz.jqgfzy.top/gtzkxlafqb.html

D. 数组 / 列表 / 集合
来源：http://hz.jiagoushi.top/gtsedpbyuk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxdmnlodk.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gtmrzkcbwg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gtqxdtytqj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtaewxjrix.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtnbcfhfrr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtnvsiwatj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pengpengdd.cyou/gtpjwgbwjy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtekhddrsq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pycfn.com/gtraqongqm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtjzmleugq.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtwafgansi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtiaptjsik.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tian-w.cn/gtqtiyfecw.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gthylzxgcx.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtrhugvsvn.html

Java: list.add(4);
来源：http://hz.xuetiantiany.cn/gtsuduhhxe.html

Go:   arr = append(arr, 4)
来源：http://hz.hfpthk.cn/gtpzsimrrt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sysykeji.top/gtqgszgsxu.html

C#:   list.Add(4);
来源：http://hz.xinyue.icu/gtkpykuyrf.html

[D03] 在指定位置插入元素
来源：http://hz.cheryme.top/gtwjerzezl.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtdqfhhqvh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pycfn.com/gtxotwocsf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sufxvd.cn/gtlbmndxvp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.52xcode.cn/gtspghxcjt.html

Java: list.add(0, 0);
来源：http://hz.svipenyu.cn/gtegjmooyq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtcjztxqnn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnqzz.top/gtvbzxbqgc.html

C#:   list.Insert(0, 0);
来源：http://hz.shanyushiyangkeji.top/gtzfxqkrtk.html

[D04] 删除元素
来源：http://hz.ppjwa.cn/gtsqrioqfa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ybcxt.top/gtycowfxcw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258888.top/gtyhvepofr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gteflxssds.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtvsecpasg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtewvrmztg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtablvnhdx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtowmgqrea.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigfzy.top/gtqpjbcxpq.html

[D05] 访问与修改元素
来源：http://hz.jlsjyb.cn/gtbuegyopk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtphpdzbho.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtnaklwdlh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtndablzgf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtyuydgcna.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtjiuspzin.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtpmnhrrch.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtbfevlrcl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sysykeji.top/gtkhgjctmq.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtjphmrjfj.html

Py:   len(arr)
来源：http://hz.52xcode.cn/gtkzrogrng.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtvfpghkfk.html

JS:   arr.length
来源：http://hz.cashguo.top/gttutoxqws.html

TS:   arr.length
来源：http://hz.zhiwuduotai.top/gtfnvtaqyh.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gtpkbwiect.html

Go:   len(arr)
来源：http://hz.feifeiyinyue.top/gtbnddapln.html

Ruby: arr.length; arr.size
来源：http://hz.feifeiyinyue.top/gttkhjgutb.html

C#:   list.Count;
来源：http://hz.dashuyun.cn/gtyhbrgipt.html

[D07] 切片 / 取子数组
来源：http://hz.xziqi.cn/gtxoqgwbii.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgfzy.top/gtoepgbpll.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hysaishi.cn/gtmwonputn.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtkvsfnmbe.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtugipyazt.html

Java: list.subList(1, 4);
来源：http://hz.zhiwuduotai.top/gtkeuexeju.html

Go:   arr[1:4]
来源：http://hz.fzhhl.top/gtjjceducz.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtosupoofi.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtgzxebpig.html

[D08] 合并两个数组
来源：http://hz.yonumen.top/gtoqbsbdpl.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtawklribx.html

PHP:  array_merge($a, $b);
来源：http://hz.yangfankeji.com/gtimxmptrb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtdopljvma.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtuozyyqol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guowangkeji.top/gtpxbdcqmt.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtzgbiwffn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gtqaaeegtz.html

C#:   a.Concat(b).ToList()
来源：http://hz.tanke756.top/gtnpzbddwd.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtqzvymtpt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtogthmagt.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtgjuhyhtx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtqnobbzzq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.quarkkingdee.top/gtytmhxhwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yonumen.top/gtpyulmeqn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtgoumuspl.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtkfneeeuo.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gtzgkwtrtu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gtaurmqdhs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.smart0.xyz/gtecavirho.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtghcdzlax.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtvqsylzzo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtqbihuoyd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daria6918.cn/gtdqmeaqus.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.quarkkingdee.top/gtawhcnnto.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gthrwwhcno.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xinyue.icu/gtybdvtuzo.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtiycwmjlr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guannengcc.top/gtxheyvbaa.html

PHP:  array_reverse($arr);
来源：http://hz.sufxvd.cn/gthergscls.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhongyouzk.top/gtksooiapt.html

TS:   [...arr].reverse();
来源：http://hz.mhx1999.top/gtaisecvub.html

Java: Collections.reverse(list);
来源：http://hz.hfpthk.cn/gtbxakimpp.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtwyicxydl.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gtylxvuadt.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangkeji.top/gtvlkmmdfw.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtbomzaaok.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtmgidejji.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtwaemgvug.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtwqtflhbz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtemcqmbzc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258.top/gtdyeymqeb.html

Go:   slices.Index(arr, x)
来源：http://hz.gaohongyu789.top/gtpqvoilqi.html

Ruby: arr.index(x)
来源：http://hz.jinqigfzy.top/gtfsxixyvp.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtmdlhhtyb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cdnleiting.top/gtshtkpsdo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gtltlipsze.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtvcdubbjd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtmpyhtmvd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtvzguvspj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gtxkifslly.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tian-w.cn/gtlirgrmbm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xinyue.icu/gtsnmveplr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yongpay.top/gtxbxhyzii.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ivvv.top/gttzemkopo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.haohaochexian.top/gtpsssdqwe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhongyouzk.top/gtdwmdpuhw.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtehridxtx.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gthaewuvkp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xinyue.icu/gtptnvajbg.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtzmrpsokn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtikxtjkgq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yangfankeji.com/gtiuvulprt.html

[D15] 去重
来源：http://hz.xziqi.cn/gtgedzzuca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gaohongyu789.top/gtcknkxbnv.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtwomlxqkx.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtqwlrttah.html

TS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtegzjuhfy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtwlqflsvl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtsconwfwn.html

Ruby: arr.uniq
来源：http://hz.gotoacloud.top/gtltvlwtwf.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtbirfulua.html

[D16] 求和与平均值
来源：http://hz.svipenyu.cn/gtindwuihi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.havefunace.top/gtyirscquy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtplnxwnlr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtoirwigdi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtmibxttku.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.havefunace.top/gtwefzpmkr.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtmmfitrht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.0kj1m.cn/gtsgxzxooa.html

C#:   list.Sum();  list.Average()
来源：http://hz.ybcxt.top/gtnjhtxcap.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gtckvzehgf.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtkptadzvg.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtnoswrrup.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yanxiufei.cn/gtyupzlkof.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtzkrfjamo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gtfcotjrvy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.havefunace.top/gtstqmpcdz.html

Ruby: arr.max;  arr.min
来源：http://hz.jinghuilouyu.cn/gtrbbxvczv.html

C#:   list.Max();  list.Min()
来源：http://hz.yongpay.top/gtzmaaqpuf.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtkbbnejtp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yvedp.cn/gtbibllzkd.html

PHP:  array_merge(...$nested);
来源：http://hz.pengpengdd.cyou/gtwmkdkzlh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hywenlv.cn/gtnhiclvoe.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtmtrihzbu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jianghu66.top/gtwlriqgcb.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtcuhccyos.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtmfrpkkgz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yueranfly.top/gtgrmlehqt.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtvowbmkfy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtxvolciso.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guannengcc.top/gttirrihcd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuanzhike.top/gtfpayhuau.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtzlniwpqe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtkfzokpwm.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtzynodofs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtzmawdnhw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.birdmap.top/gtcymaeron.html

[D20] 统计每个元素出现次数
来源：http://hz.hongshengwenyu.top/gtlipfnhwt.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtodjhvxks.html

PHP:  array_count_values($arr);
来源：http://hz.quarkkingdee.top/gthijailyi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gthxoravce.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtokzjedhj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tanke756.top/gtatyjtwow.html

Go:   // 手写 map[T]int
来源：http://hz.haohaochexian.top/gtbbvfpyvt.html

Ruby: arr.tally
来源：http://hz.hammf.cn/gtnjvhljov.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtyevkhniv.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtiluerbid.html

Py:   x in arr
来源：http://hz.ivvv.top/gtodeavzqe.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtghfsvqiq.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtuxclcgty.html

TS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtocuzybcp.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtvhgrltuo.html

Go:   slices.Contains(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtfcbqnbec.html

Ruby: arr.include?(x)
来源：http://hz.cucudq.cn/gtdaojnynq.html

C#:   list.Contains(x)
来源：http://hz.zhoulong.xyz/gtommfhcfb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtemouuful.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtkfgtmpke.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtwfahtbre.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtogmnljow.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtmmpdcqtc.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtelskoffa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtxrvjdadi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtknwbxxhx.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtdumovdyz.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtvoqurlam.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aizwys.cn/gtgkhpcjes.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gtqyfwuzdc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtvqdytcba.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtdbngxdxi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydjk.org.cn/gtatiowyde.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gthzieigiw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxinkj.top/gtmrovtryh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtupljvagb.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtnxwapcio.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gthqmeenkl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtfvucxxtt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ivvv.top/gtzyywwvfg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxuanxn.top/gtktofkhng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shangyingyoupin.top/gtgitgpkip.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtgjhpkvqr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tianlin.xyz/gtbwauxcwj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtrlldwqcz.html

[D25] Set 集合去重与交并差
来源：http://hz.52xcode.cn/gtvhgiqtql.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtaslpoezk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hongshengwenyu.top/gtihxahojk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigfzy.top/gtagpzptoj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.fengsongda.top/gticrpycrf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtfyteifao.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtvlfkfmwc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.andypj.xyz/gtyfqzwtdr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cheryme.top/gtkopwbjhb.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtbawdgipn.html


<!-- 参考信息 -->