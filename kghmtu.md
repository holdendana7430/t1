代发 wailian999

TS:   同 JS
来源：http://hz.fzhhl.top/gtcxbxgkhw.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtzhwfpnnk.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtmteojygl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtwybzayhe.html

C#:   块级作用域
来源：http://hz.chenzaomai.com/gtrzlsjicv.html

[C11] 模块导入与导出
来源：http://hz.yangfankeji.com/gtojnhmceq.html

Py:   from module import func
来源：http://hz.shanyushiyangkeji.top/gtyvvpyrsd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.bjfxy.top/gtfbickpze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydzc1.top/gtqmofcgud.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hammf.cn/gtvlvcwhoe.html

Java: import java.util.List;
来源：http://hz.yuanzhike.top/gtseknduvy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtmakuzmwx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangshuangyany.cn/gtjazidqlc.html

C#:   using System.Text;
来源：http://hz.meibo888.top/gtlobrhadp.html

[C12] 立即执行函数 IIFE
来源：http://hz.c1oappe.top/gtkwrcjwpo.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtepfbgjsc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hongshengwenyu.top/gtvapjgjkr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtqiharkpp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtfkizcjlc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtfgaockld.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtuxkknuhx.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtvzqwudgy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtjdfwiehl.html

[C13] 类型声明 / 类型注解
来源：http://hz.feifeiyinyue.top/gtvxglmxib.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtodmjghmb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtmhsbdhiv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.c1oappe.top/gtvwsqawlz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtwssnbjqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtpunzvxby.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtvaeeeuiv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cashguo.top/gtmcqwdhok.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shzxlz.cn/gtmejjuvgq.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gthzsqskws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtjihdvabn.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtapdqygce.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtqauhrqnc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtlbnzqorl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtwksbaxse.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yangfankeji.com/gtwkrisvtf.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gthehplstt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtjiwsyzjj.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtussnnotn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtswkepwea.html

PHP:  [$a, $b] = $pair;
来源：http://hz.9152youxi.cn/gtxjjdlmsd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtnqtdyath.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtwiiojcui.html

Java: // 无解构
来源：http://hz.vqdsnc.cn/gtqcflbigx.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtsfbftzmf.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtqpmlfzxc.html

C#:   var (a, b) = pair;
来源：http://hz.snrcjt.cn/gtszpvhfdc.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtyfljrmur.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gotoacloud.top/gtychylees.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtktczwtfp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gteapuytoe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dashuyun.cn/gtedgsesxn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shuidangran.top/gttujmylri.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtymvfioea.html

Ruby: # 无重载：靠动态参数
来源：http://hz.mhx1999.top/gtnizzoznh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.guannengcc.top/gtctgefwqx.html

================================================================================
来源：http://hz.yangfankeji.com/gtaiorccef.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtnelmqkox.html

================================================================================
来源：http://hz.daxiang520.top/gtsrayuwnn.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtpzcwbpey.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtewehmxuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangtech.top/gtqbmffbxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gtphvyejse.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangkeji.top/gtdzqwsrru.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daria6918.cn/gtcqqxqrie.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.0kj1m.cn/gtonlqlaja.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtbpoyosbp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daria6918.cn/gtutyjizbt.html

[D02] 追加元素到末尾
来源：http://hz.tianlin.xyz/gttscebzkv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtvkgpqsjc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xylfe.cn/gtrzozlpdu.html

JS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtargzcbrb.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtmdwyoajg.html

Java: list.add(4);
来源：http://hz.ydzc1.top/gtjgokvzyf.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtmwcpuazm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangtech.top/gtcfjpdwif.html

C#:   list.Add(4);
来源：http://hz.yuxming.cn/gttergqqke.html

[D03] 在指定位置插入元素
来源：http://hz.iojbl.cn/gtlthtigtu.html

Py:   arr.insert(0, 0)
来源：http://hz.sweek.top/gtvxdptiqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.quarkkingdee.top/gtnvswvcjo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtnzrabvtl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtukuntmkr.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtqlpyqjiq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtnvczgnoi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fengsongda.top/gtygiryzsu.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtvtjpvfbb.html

[D04] 删除元素
来源：http://hz.316326.xyz/gtqxzvyqod.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigufen.top/gtoapoinsd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtkunqnlmk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.9152youxi.cn/gtihhuykse.html

TS:   arr.splice(0, 1);
来源：http://hz.316326.xyz/gtxbacwsaw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gtzojaqcve.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shuidangran.top/gtjfcykecf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tian-w.cn/gtiwicemqh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtmaiihjse.html

[D05] 访问与修改元素
来源：http://hz.hysaishi.cn/gtxpblpcgh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gthpvaqtft.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gtmatuvfwf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtfppocsbb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhaomingkeji.xyz/gtmxvcdrlz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtwlfzuqmm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtppeeozpg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtrcizaazs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jyoumei.cn/gtxmaynnmf.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtocyatehf.html

Py:   len(arr)
来源：http://hz.shangyingyoupin.top/gtxneiczor.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtknelsdwr.html

JS:   arr.length
来源：http://hz.bjfxy.top/gttyeamtoq.html

TS:   arr.length
来源：http://hz.jianghu66.top/gtpbzuckna.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gttxdaccfn.html

Go:   len(arr)
来源：http://hz.jinqigfzy.top/gtphtbfmjd.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gteuvzdzut.html

C#:   list.Count;
来源：http://hz.mhx1999.top/gtnctrihph.html

[D07] 切片 / 取子数组
来源：http://hz.kuanghao11.cn/gtympfogmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zdqjudy.top/gtckgmvdws.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xziqi.cn/gtvdkzrlga.html

JS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtfiwshvtp.html

TS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtujpdcynl.html

Java: list.subList(1, 4);
来源：http://hz.aizwys.cn/gtqcrgjbgm.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtaggqdgak.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gthgnlskuf.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gtirfzcqqs.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtkmsnprpl.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtqpciqxij.html

PHP:  array_merge($a, $b);
来源：http://hz.quarkkingdee.top/gthgrsmpac.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtrgqjzppa.html

TS:   [...a, ...b];
来源：http://hz.jlsjyb.cn/gtmgcxnlel.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtyufaumvh.html

Go:   append(a, b...)
来源：http://hz.jinyuanbaomall.cn/gtoxyhmuyl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtvhxnrvmj.html

C#:   a.Concat(b).ToList()
来源：http://hz.daria6918.cn/gtimbipluh.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gthxebpkij.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtvniwhkwc.html

PHP:  sort($arr);
来源：http://hz.cdnleiting.top/gtudgewrps.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.andypj.xyz/gtfznxpbqi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.52xcode.cn/gtjjqinyqf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yueranfly.top/gtbpcjoocb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daxiang520.top/gtsnchvcfj.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtjlhulqgu.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gtjccvcwmo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sweek.top/gtubyrqsnb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtjeyyplcq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtbnklycrq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtqilvwoza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtehfvqxvx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yueranfly.top/gttsyzwmot.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.bjfxy.top/gtbxmlztwp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtpwfyqpif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtfwlvmooo.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtcdziqqek.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pengpengdd.cyou/gtscxgenyw.html

PHP:  array_reverse($arr);
来源：http://hz.tianlin.xyz/gtxhrwotbp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtibuezsoq.html

TS:   [...arr].reverse();
来源：http://hz.hywenlv.cn/gtitfqrgjr.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtszkagcxn.html

Go:   slices.Reverse(arr)
来源：http://hz.zhiwuduotai.top/gtsdcxnvix.html

Ruby: arr.reverse
来源：http://hz.xuanzx.com/gtdrqwwony.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtmcaeikvr.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtyxmtprmm.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtlvohsvbs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shuidangran.top/gtbsrytfny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtnoqabwyw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtmbvanqmk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.havefunace.top/gtiszcealz.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gtjknotpik.html

Ruby: arr.index(x)
来源：http://hz.jinyuanbaomall.cn/gtvncphpfa.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtiqewdoyl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pycfn.com/gtlltgkyiv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shangyingyoupin.top/gtlybjtbwb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtpwhxyoiw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtkgrqvopk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gttaatcccp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtpkelchse.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtimwfsqlm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.feifeiyinyue.top/gttrtpvmsu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydzc1.top/gtfcpljxio.html

[D14] 映射转换（每个元素变形）
来源：http://hz.bjfxy.top/gtmwffrcoz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gtgasfribi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtghzaliuv.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtginvkclz.html

TS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtbtlcadip.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hywenlv.cn/gtimsyqnuh.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtkitohbwp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gaohongyu789.top/gtsptnpamt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.snrcjt.cn/gtpdtejyep.html

[D15] 去重
来源：http://hz.wangdashe.top/gteanpzmfp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gttkvvjnxm.html

PHP:  array_unique($arr);
来源：http://hz.yuxming.cn/gtctgktfxl.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtuygwcgkh.html

TS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gthrvxbrfb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtrbxdnigi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtissypbxb.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtzymzkcli.html

C#:   list.Distinct().ToList()
来源：http://hz.zhijiandao.cn/gtshzrbinw.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gtjqtsrxgx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtdkppdmjj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtpgzdvnre.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtfsbavpwc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gteymknsml.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shzxlz.cn/gtityyacej.html

Go:   // 手写循环累加
来源：http://hz.zhiwuduotai.top/gtwttzjlth.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtmqqxigte.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuanzx.com/gtcizvlary.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gttjoogodz.html

Py:   max(arr);  min(arr)
来源：http://hz.bjfxy.top/gtcbfndzyn.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtoflqzsql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtzufpwutd.html

TS:   Math.max(...arr);
来源：http://hz.xylfe.cn/gtwycnbozo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtlcuazhpw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pengpengdd.cyou/gtwdblywla.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtoyuusmnj.html

C#:   list.Max();  list.Min()
来源：http://hz.cashguo.top/gtvmetbypq.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtjkolgxnp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtaicrndkf.html

PHP:  array_merge(...$nested);
来源：http://hz.aibaodan.cn/gtygqdqznc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtmarauroe.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtkzahokjt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gttdrviyzs.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtjdnxofus.html

Ruby: nested.flatten
来源：http://hz.hnxiangtu.top/gtyyxmsqti.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtmgymuheb.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtrpqhvdtg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.0kj1m.cn/gtdnuodbjq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtpdkgyzcf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtfcfulhel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtzkqmkdsn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtwhtxrbge.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtvlrgcbzm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtigdrbsyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gteufbqzxf.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtlbjpvrgu.html

Py:   Counter(arr)
来源：http://hz.cucudq.cn/gtwerezphz.html

PHP:  array_count_values($arr);
来源：http://hz.jianghu66.top/gtmfzvntcs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtvbregmxl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtwbadwbwn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtdgyihpxw.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gtegsdugyl.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtqkszqfpf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtvahvuaey.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtqdromkzc.html

Py:   x in arr
来源：http://hz.zhaomingkeji.xyz/gtjdsbemgb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtqcgkjgmv.html

JS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtntzydceq.html

TS:   arr.includes(x)
来源：http://hz.snrcjt.cn/gtdhiqgiwc.html

Java: list.contains(x)
来源：http://hz.shanyushiyangkeji.top/gtnjpdmyup.html

Go:   slices.Contains(arr, x)
来源：http://hz.quarkkingdee.top/gtywtcecly.html

Ruby: arr.include?(x)
来源：http://hz.hnxiangtu.top/gtklsfvnqp.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gtffqyvyvi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sweek.top/gtvvxgjzco.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gtshjhtuwj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtaeytmpqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtrduekmob.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtzeilfojx.html

Java: new ArrayList<>(list);
来源：http://hz.nanxinkj.top/gtmmqgqwrb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtupxlrwcn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgufenzy.top/gtqvppjavt.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtqbascask.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtvgblkuwv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangtech.top/gtjvijigpl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenzaomai.com/gteqgacjbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtmjunwmiu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtxmrpgcmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxinkj.top/gtkfbxivur.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtfnyjdgwv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtfykoxzuv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtyksfffpv.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gtkhekibeo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtrvflujye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.svipenyu.cn/gtqhpczslw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.vqdsnc.cn/gtxmcwodds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtuchirjer.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtwugprslt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gttfacmvcd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gotoacloud.top/gtujutggwz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtickpvwpw.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtfgstcqip.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtmpzwyykn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yanxiufei.cn/gtcpxkqvnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtgjtodtqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtpubjreid.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtrakpuaxt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangshuangyany.cn/gtltsxgijl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gtdgkciwox.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jyoumei.cn/gtjdrpyzbr.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtpkxlrfei.html

Py:   ", ".join(map(str, arr))
来源：http://hz.snrcjt.cn/gtphdgrvox.html

PHP:  implode(", ", $arr);
来源：http://hz.tanke756.top/gtkwwhpxgu.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtnucbanpq.html

TS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtpmhkreoe.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtzvvutrxg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtvkbvpddu.html

Ruby: arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtulnvtuxs.html

C#:   string.Join(", ", list)
来源：http://hz.cqqwz.cn/gtsjclvvry.html

================================================================================
来源：http://hz.jiagoushi.top/gtcewotled.html

E. 字符串处理
来源：http://hz.fzhhl.top/gtzhvrocub.html

================================================================================
来源：http://hz.iojbl.cn/gtkykvdglh.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gtndpnirac.html


<!-- 参考信息 -->