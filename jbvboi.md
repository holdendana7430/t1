代发 wailian999

TS:   同 JS
来源：http://hz.xuanzx.com/gtryemaszv.html

Java: 方法内为块级作用域
来源：http://hz.xziqi.cn/gtfyzedgcq.html

Go:   花括号块级作用域
来源：http://hz.zhengqikj.top/gtuaxkdavv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jlsjyb.cn/gtcvgowfos.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtvirexckc.html

[C11] 模块导入与导出
来源：http://hz.9152youxi.cn/gtrcwsbxiy.html

Py:   from module import func
来源：http://hz.svipenyu.cn/gtlubcqrhh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtlgalewpr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtujgnamfi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.haohaochexian.top/gtnrnhsoec.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtuidymwxj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yanxiufei.cn/gtxbippevx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtbgvpvzco.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gtaxjjwkys.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtqehxiirk.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigfzy.top/gtgdecymba.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtzligpeit.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gthtnhrfhd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gthqqjyach.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.feifeiyinyue.top/gtnriqhbzr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxuanxn.top/gtjwwhhefg.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtmiwojvlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnxiangtu.top/gtaolqyucn.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtpfoievtz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.redwolf501.top/gtduibthbc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtiqhfknct.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fzhhl.top/gtpzzgpydz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtppynfemk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtezwcreeo.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtxtfvttug.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtervpdluh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zdqjudy.top/gtwivrkbkp.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtjqbekoum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtkebtausf.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtvyhjjqip.html

JS:   // 无泛型
来源：http://hz.xziqi.cn/gtqhhtgyxo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nwbrower.top/gtqlmhskmm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydjk.org.cn/gtwzpvdgqw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shzxlz.cn/gtacpjmdmj.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtcouvbyno.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtehztpmmm.html

[C15] 解构 / 展开参数
来源：http://hz.fengsongda.top/gttllraota.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtkxqyzqlz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shuidangran.top/gtqkfmjsca.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtctspfbgb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtvtyiygtz.html

Java: // 无解构
来源：http://hz.daxiang520.top/gtfujzawnr.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtlnovdfpf.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtfldqagrf.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtikktqzrq.html

[C16] 函数 / 方法重载
来源：http://hz.zhixingplan.top/gtelymkepk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yongpay.top/gtkmwvcbqc.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtuarksjqb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydjk.org.cn/gthbrnwsgb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtdargvblv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jlsjyb.cn/gtzvpqisde.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtkgbttpsu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.chenlongwang.top/gtnasswjdp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fzhhl.top/gtdtcinlhc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtaijkwxvj.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gthmipzwsv.html

================================================================================
来源：http://hz.cucudq.cn/gtfqykyomt.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtvmykaesh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hysaishi.cn/gthbmywyyq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtrmzzttcj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gtfcsgyjtp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.iojbl.cn/gtjkijjony.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shangyingyoupin.top/gtsfndtgog.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigufen.top/gtdfydusdq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtvriaptls.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtxkypfiks.html

[D02] 追加元素到末尾
来源：http://hz.yj20258.top/gtklbvasom.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gogol.net.cn/gtsgbwteyv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtqfmuzbdp.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtuapoiokh.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtxisargig.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtxdktmvet.html

Go:   arr = append(arr, 4)
来源：http://hz.zhoulong.xyz/gtrnihkfyi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtzmixjccf.html

C#:   list.Add(4);
来源：http://hz.jiagoushi.top/gtddsgflpp.html

[D03] 在指定位置插入元素
来源：http://hz.zhaomingkeji.xyz/gtcjevvaok.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gthtxcypyr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gtmqjhawpq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtbqbfkomb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangkeji.top/gtkonantnl.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtjqraxvic.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gtwaccwwsn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gtogzwejto.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtvzoimaug.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtereusmyk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tian-w.cn/gtzpggujlq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.havefunace.top/gtopjubrqn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gogol.net.cn/gtdgjidwvy.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtumxlsleb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tian-w.cn/gtjopmeura.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.mhx1999.top/gtazhshwgb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtarkxqgfu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtspqzshfr.html

[D05] 访问与修改元素
来源：http://hz.jqgufenzy.top/gtjmfackgu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtmqpdhojr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtvxlafdvi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtqejzjpxu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtalcmzmzj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtagcoighk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtuxipqqzp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtcxxwsrae.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhixingplan.top/gtovbrpwyb.html

[D06] 数组长度
来源：http://hz.dianchejie.cn/gtehchzled.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtuokutanm.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtrzxrzqqv.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtwaommmqv.html

TS:   arr.length
来源：http://hz.ybcxt.top/gtjcvzgwfv.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtyzqarpel.html

Go:   len(arr)
来源：http://hz.ivvv.top/gtlhpwicdq.html

Ruby: arr.length; arr.size
来源：http://hz.sweek.top/gtbflqkqls.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtugrgcuap.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtjczgujdw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gtdeqpzccj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtmhvcpydn.html

JS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtxlmjdknh.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtuhkcmuzx.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtdcrynfyf.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtrellkivc.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtefkxqikh.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtnzrooepd.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gthaviplzt.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtbbcrrnfu.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtewzasium.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtyigdlpev.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtjirtnptj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tianlin.xyz/gtsoobgwgv.html

Go:   append(a, b...)
来源：http://hz.dashuyun.cn/gtcwgjuffy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gtrmlouhbt.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydzc1.top/gtmtigpsok.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtfkhokrzk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtcwogyxvf.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtdeisyyql.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258888.top/gtwdpnjchh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangkeji.top/gtxctspzdu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtczbcpnba.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtyfbfizna.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gteivovhvp.html

C#:   list.Sort();
来源：http://hz.xziqi.cn/gtrzekeruc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gtaiuliydh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtboeirstf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gthlarjfqk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtuolmojbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtcfbkpcod.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtycnxpprm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hysaishi.cn/gtysfppyfc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtiisgfaum.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuxming.cn/gtwigtjxef.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtefoklvoz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtvqgakuqc.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtmccovkrv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinyuanbaomall.cn/gtzoinzvrw.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtabcerpkz.html

Java: Collections.reverse(list);
来源：http://hz.jiagoushi.top/gtuummzdjq.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtvelkubeu.html

Ruby: arr.reverse
来源：http://hz.quarkkingdee.top/gtccelsbgi.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtfmcbjdha.html

[D12] 查找元素下标
来源：http://hz.hywenlv.cn/gtipgtivku.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gthxrgmhxd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.birdmap.top/gthatpuxyf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtjdlptftf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gteuxmvnna.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtrwldxrut.html

Go:   slices.Index(arr, x)
来源：http://hz.yuxming.cn/gthhmwbvkj.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gthoduhedp.html

C#:   list.IndexOf(x);
来源：http://hz.xingfuxueyuan.xyz/gtbsxgztnd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtoljkhblp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gttwcxipyx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtedmsctmx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtoaexiysy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtbpjyfrat.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangshuangyany.cn/gtfsctqwwy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtwbnxkhau.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtatpuitiz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gaohongyu789.top/gtpsoyodis.html

[D14] 映射转换（每个元素变形）
来源：http://hz.bjfxy.top/gtyenknudi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydjk.org.cn/gtnpdjejmb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtwwdeqfkx.html

JS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gterqnpzyi.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtwdevykdd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xylfe.cn/gtltyqzlgf.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtkyllktng.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigufen.top/gtdywhqaif.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtrmiyeogl.html

[D15] 去重
来源：http://hz.cucudq.cn/gtbvultnlx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangkeji.top/gtcxmmfzes.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtmmauoula.html

JS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtupnspwke.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtiyiibstg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenjidiqi.icu/gtwgchyfyl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hammf.cn/gteejvtprv.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gtuqgofpfj.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtaddvoegm.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtjmmgosix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gtfdrpgblu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtsiqmvxlz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gthbdkhgqp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtrnalvzyc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtoipjnyov.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtxnybrjof.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtrkabxgqk.html

C#:   list.Sum();  list.Average()
来源：http://hz.daria6918.cn/gtxmpatxss.html

[D17] 最大值与最小值
来源：http://hz.jlsjyb.cn/gtfdaffwwz.html

Py:   max(arr);  min(arr)
来源：http://hz.cqqwz.cn/gtjbvrrvoi.html

PHP:  max($arr);  min($arr);
来源：http://hz.yueranfly.top/gtitzycvxv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gttssovqbw.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtshdvvcru.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgufenzy.top/gtrrblpzvl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.bjfxy.top/gtkwdqytrg.html

Ruby: arr.max;  arr.min
来源：http://hz.9152youxi.cn/gtvouxxrbs.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtgqwiqakh.html

[D18] 扁平化嵌套数组
来源：http://hz.hysaishi.cn/gtkytavghi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.snrcjt.cn/gtaxdokhvp.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangkeji.top/gtaxrnjzuu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtzyfdgcld.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtbsocyxqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gtwmxuqyue.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtrloplolp.html

Ruby: nested.flatten
来源：http://hz.andypj.xyz/gtopzjfvlj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtasxeicnk.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtkayjbdkh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtakdpqzog.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtolrwjlwv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtjeelyzps.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtqpbdhlyd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xingfuxueyuan.xyz/gtpiveycau.html

Go:   // 手写 map[string][]T
来源：http://hz.sufxvd.cn/gtgnbangbj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dashuyun.cn/gthvpqjhvn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydjk.org.cn/gtgwsrymrq.html

[D20] 统计每个元素出现次数
来源：http://hz.jinghuilouyu.cn/gtpbtekkmt.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gteeuvbjeu.html

PHP:  array_count_values($arr);
来源：http://hz.yvedp.cn/gtokxsryfe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtqwjgssbc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtcmdyxdgn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.iojbl.cn/gtkyflqunv.html

Go:   // 手写 map[T]int
来源：http://hz.sufxvd.cn/gtachalwzp.html

Ruby: arr.tally
来源：http://hz.hfpthk.cn/gtktkrduwg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhongyouzk.top/gtisobwtez.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtgdkzaxgq.html

Py:   x in arr
来源：http://hz.316326.xyz/gtjlczrixk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigfzy.top/gtpyzkbdwf.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gthgtbindt.html

TS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtjujhzhvn.html

Java: list.contains(x)
来源：http://hz.sxryk.cn/gtaflgrypz.html

Go:   slices.Contains(arr, x)
来源：http://hz.bjfxy.top/gtxiyliohw.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtdzmcpmcf.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtvtakvdav.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gotoacloud.top/gtfokhulvb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtakykrhtr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dianchejie.cn/gtaomiyupk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gterzmnmop.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtwduujfnr.html

Java: new ArrayList<>(list);
来源：http://hz.gogol.net.cn/gtjkpdowen.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gtrbkjtnzz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtdzlqiuur.html

C#:   new List<int>(list);
来源：http://hz.xingfuxueyuan.xyz/gtmgrkzfxn.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gttzbhsbql.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtlpuhnrzm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtybxoxdcy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtxgqbejjq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtmjhowiyl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydzc1.top/gtonjstqag.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtfmsmgqmf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hongshengwenyu.top/gtynoolvhn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtcotvouzb.html

[D24] 字典 / Map 基本操作
来源：http://hz.zycfv.cn/gtambivnal.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtluqctrlb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtbuwyjhbd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yongpay.top/gtluyokwtc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtdzwtgnhj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtrozcxirg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtrlhwitgh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gtruflqhsx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtitfttney.html

[D25] Set 集合去重与交并差
来源：http://hz.hysaishi.cn/gtlkkoftpg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtwyotyouo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtahnawukp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cashguo.top/gtvznjsjms.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtulphdcaz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtnprcmldw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtkpnbrhhg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtceqgvubx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtkoimoico.html

[D26] 数组转字符串
来源：http://hz.52xcode.cn/gtxcgarups.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pycfn.com/gtlsdwwjrv.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtpwjeppmr.html

JS:   arr.join(", ")
来源：http://hz.sweek.top/gtljflsuzm.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtxthusiij.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtywusajtk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.0kj1m.cn/gtzamytymn.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gttlhmmyel.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtaujzmrlo.html

================================================================================
来源：http://hz.cheryme.top/gtspbroqfh.html

E. 字符串处理
来源：http://hz.ywan-chungtsiang.top/gtkjqahntc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtikemsrsi.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtwrkftkdj.html


<!-- 参考信息 -->