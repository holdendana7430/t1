代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtqbnlhphs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtxxapecah.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtrqhlpclf.html

[C09] 递归
来源：http://hz.mhx1999.top/gthjqbgupx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtkulhlulj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gzhubu.top/gtqnndivtv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtwfgqtyoc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtzmalibfr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sweek.top/gtgnhklwcf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.redwolf501.top/gtapixdnds.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.iojbl.cn/gtyuygynrw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtagjjbmlo.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtwkbncsvw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtzazbaypw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.pengpengdd.cyou/gtaqmtzles.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.feifeiyinyue.top/gtqgorfebu.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gthjqkghpw.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtgcjscxug.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gthayiqeyw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangshuangyany.cn/gtpcicyrhd.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtnylgkkco.html

[C11] 模块导入与导出
来源：http://hz.xuanzx.com/gtjvtvprla.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtccffmfup.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gotoacloud.top/gtfiifqrpm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtcuaajlap.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hongshengwenyu.top/gtlfgiueks.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtflwxmxlo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daxiang520.top/gtaidftsfr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtzofyldba.html

C#:   using System.Text;
来源：http://hz.ehwqpu.com/gtyynnrgiz.html

[C12] 立即执行函数 IIFE
来源：http://hz.zycfv.cn/gtkcoedirv.html

Py:   (lambda: print("run"))()
来源：http://hz.316326.xyz/gtymtpjqqr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gttvnahfcr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtaaprurkf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtgfpxpoak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gotoacloud.top/gtddbdkjxu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtpefroduq.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtqkenoteq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tanke756.top/gtpmuhzrgo.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtsomyjyze.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tian-w.cn/gthdrbblvr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtvtcgivyp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtuhkjmrpv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtonvfgaxq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtfijzdscb.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtgxrrpxgw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sufxvd.cn/gtyhwcpvxt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cqqwz.cn/gtmoflymxk.html

[C14] 泛型函数
来源：http://hz.xuetiantiany.cn/gthkkytosz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.c1oappe.top/gtegoiuotz.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtsrxidwhp.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtcgauplry.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.feifeiyinyue.top/gtuhgrjiis.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxinkj.top/gtfdusxpmm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenzaomai.com/gtisksxsca.html

Ruby: # 无泛型
来源：http://hz.jinghuilouyu.cn/gtjgycbhsb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtxdokmckm.html

[C15] 解构 / 展开参数
来源：http://hz.yvedp.cn/gtszqucppl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guowangkeji.top/gthxouigtf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhijiandao.cn/gtrlrdflou.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtzdjxbsye.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gtetcahcrx.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtiamxmaiz.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtycmkuubx.html

Ruby: a, b = pair
来源：http://hz.xuetiantiany.cn/gtrdfvytuh.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtoohgnszf.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtzshenmer.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ppjwa.cn/gtrjppnhlx.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtmfzxswna.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hammf.cn/gtwacmgxzy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtpaiiugxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtebqwccah.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtwysvcqpw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yueranfly.top/gtdbqcfsxu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtxhpvojer.html

================================================================================
来源：http://hz.guowangkeji.top/gtaqsrdjai.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gtkjyfmmtf.html

================================================================================
来源：http://hz.wangdashe.top/gtciwqabrv.html

[D01] 创建数组 / 列表
来源：http://hz.jqgufenzy.top/gtakcqmlkd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ivvv.top/gtjwvnzllq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhixingplan.top/gtyhpzalzk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydjk.org.cn/gtmjyyxhqf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtuyuiqpho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtovojnpgt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yangfankeji.com/gtzpdzlrwy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gteozkyttz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtiutrltqk.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtvoflhdyw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gtwrvtckyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yvedp.cn/gtjfxzookb.html

JS:   arr.push(4);
来源：http://hz.jinghuilouyu.cn/gtighokrsl.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtsfycpkkm.html

Java: list.add(4);
来源：http://hz.sysykeji.top/gthcjhaeye.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigufen.top/gttptnwmli.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenjidiqi.icu/gtytdmxpmj.html

C#:   list.Add(4);
来源：http://hz.ehwqpu.com/gtseeruknm.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gtzutmkxsj.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtcfbwdeni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuetiantiany.cn/gtqzswlwmn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtgyeoflbv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtbpzswfxg.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtotjiguen.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.birdmap.top/gtnqalifoo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenlongwang.top/gtmovqduji.html

C#:   list.Insert(0, 0);
来源：http://hz.xingfuxueyuan.xyz/gttsjumatu.html

[D04] 删除元素
来源：http://hz.jyoumei.cn/gtnxpfhggo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtrcmxmbmj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtbtxrakud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fengsongda.top/gtbbjorbvq.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtmsbzgisf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhixingplan.top/gtpzbiasio.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtsazzymak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtfewqgqmw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtcpngtgox.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gtndllhqdu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtkgoirfjs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuanzhike.top/gtcukttmvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daxiang520.top/gtgzgcequz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gtfejegkbd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shzxlz.cn/gtjuatgzzo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gthemakxwe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtwnbvcwhm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zycfv.cn/gteukbwjjb.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtqdcwfeyf.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtujdruvnb.html

PHP:  count($arr);
来源：http://hz.daxiang520.top/gtchyqdpjz.html

JS:   arr.length
来源：http://hz.fzhhl.top/gtygwdfttf.html

TS:   arr.length
来源：http://hz.316326.xyz/gtcfyziika.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtdyyjetkm.html

Go:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtjpxnxgdm.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtlptguawm.html

C#:   list.Count;
来源：http://hz.shuidangran.top/gtwtdfbyyw.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gtvckhwxzx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtjankngoi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtnueallyb.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtwzicwldx.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gthtnhuseu.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtzlkhdvkf.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtjavjywzf.html

Ruby: arr[1, 3]
来源：http://hz.yongpay.top/gtshxbzjoc.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtvtzymiay.html

[D08] 合并两个数组
来源：http://hz.birdmap.top/gtwdisewkd.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhiwuduotai.top/gteykqapud.html

PHP:  array_merge($a, $b);
来源：http://hz.jianghu66.top/gtfphhilks.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtpqdzutls.html

TS:   [...a, ...b];
来源：http://hz.0kj1m.cn/gtldwbopgc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cqqwz.cn/gtgfqjundl.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gtdrcxcmtv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.316326.xyz/gtvuazwpqd.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtbrsaqmpa.html

[D09] 排序（升序）
来源：http://hz.hongshengwenyu.top/gtdrxbbsqu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gttstgckeg.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtvqdvaoht.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gtaahvhfzz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tian-w.cn/gthbewrtyg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gtuixzmhej.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.andypj.xyz/gttvrlawby.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtahbsagjv.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtoamhfxcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cucudq.cn/gthwaujzxc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tian-w.cn/gtorfqswwc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258888.top/gtpweeibmt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtuhrudktm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtjzqlasih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtchkcjxhb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtzjufajlz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtaglcwfkc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ybcxt.top/gttrhnwpxz.html

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtktaddtvs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guannengcc.top/gtwecxwuni.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtuvfspffy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuetiantiany.cn/gtnhhsxjvi.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gtncoiwyrw.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtqacanvbp.html

Go:   slices.Reverse(arr)
来源：http://hz.yj202588.top/gtgskftxor.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtzxobaxwc.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtsqzqirbv.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtvxczirgl.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenzaomai.com/gtzyevyqnu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtyjdanqcu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtozpwxoxt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtskwirvwh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.quarkkingdee.top/gtlimpccwv.html

Go:   slices.Index(arr, x)
来源：http://hz.aizwys.cn/gtdchhsqqo.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtkogoysda.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtfbcofokh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtsnmeyqnp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jianghu66.top/gtuugdwzeo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtaaghygqh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtinhbcepz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtlrtoiaec.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtpuepvgnt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gtmozreihm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.52xcode.cn/gtlyqvptgn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtxxhrxsol.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtkgzbbbwu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fzhhl.top/gtxpqsyumg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gtpolpwcgs.html

JS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtnluasdiw.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtvgczipfp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sufxvd.cn/gttifrvrdd.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtivomiyfa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tianlin.xyz/gteabpnqwx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuetiantiany.cn/gttoujktmq.html

[D15] 去重
来源：http://hz.daxiang520.top/gtohfwbcby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtcapqrgyv.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gtllhhretc.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtmerltuzq.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gttmacimna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.daria6918.cn/gtwlprbvfk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtwjwmcxph.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtgyocmqhi.html

C#:   list.Distinct().ToList()
来源：http://hz.jiagoushi.top/gtqnzepchn.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtjgouadme.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gotoacloud.top/gtkfrplakf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gtwljmfpbz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtkzipuifd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtrlybwmsr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenzaomai.com/gtmjpiywtw.html

Go:   // 手写循环累加
来源：http://hz.ivvv.top/gtlpalqbik.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.52xcode.cn/gtqmtzwkmo.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtuuwdwoce.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtllevdvkc.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtknxdpole.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtbenaeurq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtktphdeeq.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtzqxakxrd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuetiantiany.cn/gtltpfscus.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtvmocsrhd.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtuehwfntt.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgfzy.top/gttveqwzlv.html

[D18] 扁平化嵌套数组
来源：http://hz.shangyingyoupin.top/gtwtpcyaqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ivvv.top/gtrxphmlpl.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtzblshjbt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ppjwa.cn/gtaxoyzytn.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtbbawlvdk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtiwjmotqt.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtedtxcpsy.html

Ruby: nested.flatten
来源：http://hz.svipenyu.cn/gtftxqtuzi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtrmsezvhk.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtzbausxxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtnhfjoxst.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtzeqjyctt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtttzpbdmq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhongyouzk.top/gtwdayxwwl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigufen.top/gtyhetioqp.html

Go:   // 手写 map[string][]T
来源：http://hz.9152youxi.cn/gtpcsosuhy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtrrgngxgt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtwohbinik.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtrgyyqfyz.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtxgdaarcx.html

PHP:  array_count_values($arr);
来源：http://hz.chenzaomai.com/gtwlerxbvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtzekpecoq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gthldxemwp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yangfankeji.com/gtahzwzfcu.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtcggrtdtc.html

Ruby: arr.tally
来源：http://hz.fengsongda.top/gtoffpfgul.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sysykeji.top/gtwgkmkvtt.html

[D21] 判断是否包含某元素
来源：http://hz.ydjk.org.cn/gtywqxkozp.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gthdrvypnr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.iojbl.cn/gtxehajodi.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtznfwoakv.html

TS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtindafekn.html

Java: list.contains(x)
来源：http://hz.ydzc1.top/gtmzgkuvor.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gtekrxcmoq.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gtqozialwd.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtrcwkyrot.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gttxlfaago.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tian-w.cn/gtagwutrfi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gttbznlmom.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.redwolf501.top/gtbzrvclsv.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtjvtsdase.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtcuymshxw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxinkj.top/gtqeerwtzx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gteuzeevjh.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtwasopcss.html

[D23] reduce 累积计算
来源：http://hz.pycfn.com/gtwqzzhslz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtmhhmlckl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yonumen.top/gtuqecsldl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtzrmzqhfl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtrjsjqkak.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtyvodqxbw.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtpzeqpkjd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtmxwkndyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtxdrxwhba.html

[D24] 字典 / Map 基本操作
来源：http://hz.gotoacloud.top/gtouuudaoi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtkeclbfcq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gtxiwiselj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hfpthk.cn/gtryjppuxu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangdashe.top/gtifkhxwlo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtnvxcdrlj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gttqzffhms.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.bjfxy.top/gtszfsgjbo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daria6918.cn/gtudcwomja.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtyxgpdklh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtakecitsz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hammf.cn/gtjirjffyn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangdashe.top/gtahkxcjxd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtjsxwbkyv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigufen.top/gtjhjdvdex.html


<!-- 参考信息 -->