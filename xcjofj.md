代发 wailian999

[C10] 变量作用域
来源：http://hz.tanke756.top/gttbbqwaib.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hfpthk.cn/gtvfqvvtrb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cucudq.cn/gthnbqzoik.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.316326.xyz/gtwulgoayp.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtthqwdgai.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtuewzjuwa.html

Go:   花括号块级作用域
来源：http://hz.snrcjt.cn/gtmybgendc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yonumen.top/gtetfgdpxm.html

C#:   块级作用域
来源：http://hz.haohaochexian.top/gtbgoaufvf.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtbrcbzfxy.html

Py:   from module import func
来源：http://hz.iojbl.cn/gtpuzqzigx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.feifeiyinyue.top/gtqfllodng.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtkvrwtniw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.birdmap.top/gtmkrpbexz.html

Java: import java.util.List;
来源：http://hz.ydjk.org.cn/gtpwksavvv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.pengpengdd.cyou/gtpcffnkpw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigufen.top/gtbpimmhmw.html

C#:   using System.Text;
来源：http://hz.xinyue.icu/gtqizmcunl.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtgzdgvriu.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtdxfoksqa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtfrxiiplg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtxfyzaxdp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtcixyinvw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtdczqrszv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258.top/gttgsyvdoz.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtomnmjuda.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtuyeocxpl.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydzc1.top/gtmfwkjvht.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ybcxt.top/gteitcmmxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtfkdgekgj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgfzy.top/gthxarxuoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtoneiwahq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtanaouuun.html

Go:   func add(a, b int) int
来源：http://hz.svipenyu.cn/gtwqpujjdk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hongshengwenyu.top/gtqlpbgyih.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtbktsqyux.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtcoiozxdj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guowangkeji.top/gtjgnbikkc.html

PHP:  // 无泛型
来源：http://hz.nwbrower.top/gtrmfqoveu.html

JS:   // 无泛型
来源：http://hz.yuxming.cn/gtverkytgb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtsaifxjta.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pycfn.com/gtrbedsvwr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.andypj.xyz/gtktlbbpus.html

Ruby: # 无泛型
来源：http://hz.xuetiantiany.cn/gtziafvodq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigufen.top/gtjaiekqeo.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtzbcnwxli.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dashuyun.cn/gtwvgdjrbn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtbwdzqock.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtdqnespxq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydzc1.top/gtdglbhpvu.html

Java: // 无解构
来源：http://hz.fzhhl.top/gtdnbjfvfb.html

Go:   // 无解构
来源：http://hz.hysaishi.cn/gtmcdkjawz.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gthslbsarc.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtdzlllzsu.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gtacgrnnsx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtxefblskv.html

PHP:  // 无重载
来源：http://hz.jinqigufen.top/gtncxeezij.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtpmhgpmav.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gtodvkrvup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gtcauqsbsm.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtutvvklgr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtsoqjqljv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pengpengdd.cyou/gtwdcjsctm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwboxhngv.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtadhtebau.html

================================================================================
来源：http://hz.daxiang520.top/gtmmpmkyad.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gteihlmwyx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtodlmdxwp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtkaedxnbj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hywenlv.cn/gtlratavpq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtrmzetkiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.smart0.xyz/gtliobovbc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangkeji.top/gtghncayrq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tanke756.top/gtypftfdrp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sysykeji.top/gtysormywk.html

[D02] 追加元素到末尾
来源：http://hz.yvedp.cn/gtpmyhnodt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gtpqeauphe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daria6918.cn/gtinwbbkwz.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtowfrokzu.html

TS:   arr.push(4);
来源：http://hz.nwbrower.top/gtpxfvspfn.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtrlaknwud.html

Go:   arr = append(arr, 4)
来源：http://hz.chenjidiqi.icu/gtrawqiwev.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gttqiqemxd.html

C#:   list.Add(4);
来源：http://hz.cashguo.top/gtjrynsode.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gteeeysgpj.html

Py:   arr.insert(0, 0)
来源：http://hz.zhengqikj.top/gtwqexntbp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.feifeiyinyue.top/gttxtjyyes.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guannengcc.top/gtlrpkzduv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sweek.top/gtxquvdlzq.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtopawxhxj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gttcusfmrm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daxiang520.top/gtwgcpujxf.html

C#:   list.Insert(0, 0);
来源：http://hz.yangfankeji.com/gtyhdckcmk.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtgspguxyi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258.top/gtvuixsaem.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cucudq.cn/gtulfaxlfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shangyingyoupin.top/gtrlukkzgh.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtxjzbcpho.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtbazraeld.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtnedkbshc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtdwfhvjwu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtkpoisfgy.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtmjliqova.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtxpyzkzeb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtrobfbmqc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtblovolvt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.9152youxi.cn/gtosgbbffq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.smart0.xyz/gtalihkkwr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtzaalnrti.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtydtcqpoz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtybfvxtmg.html

[D06] 数组长度
来源：http://hz.tianlin.xyz/gtccstvdlq.html

Py:   len(arr)
来源：http://hz.yueranfly.top/gtsmuhxgbw.html

PHP:  count($arr);
来源：http://hz.yongpay.top/gtqjoinidu.html

JS:   arr.length
来源：http://hz.nanxuanxn.top/gtykeltdff.html

TS:   arr.length
来源：http://hz.quarkkingdee.top/gtfystqzhr.html

Java: list.size();
来源：http://hz.yanxiufei.cn/gtfgqlefyl.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtbzsmdwrf.html

Ruby: arr.length; arr.size
来源：http://hz.yj202588.top/gtxbltdahs.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtbzrdynhx.html

[D07] 切片 / 取子数组
来源：http://hz.aizwys.cn/gtqlbxhadz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ehwqpu.com/gtzuntgsau.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtwhdmqwmf.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtvpwvrzwq.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtdhhlrvew.html

Java: list.subList(1, 4);
来源：http://hz.jianghu66.top/gtacwiggxu.html

Go:   arr[1:4]
来源：http://hz.shangyingyoupin.top/gthcyajauw.html

Ruby: arr[1, 3]
来源：http://hz.pycfn.com/gtnlhiuend.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtscefdxjo.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtmjcgmkra.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtenrqoxuw.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtnjgvxqaw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtcvgfxjym.html

TS:   [...a, ...b];
来源：http://hz.quarkkingdee.top/gthsdlaxma.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.andypj.xyz/gtwwhvudug.html

Go:   append(a, b...)
来源：http://hz.svipenyu.cn/gtkozpgxyb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtyxojuacx.html

C#:   a.Concat(b).ToList()
来源：http://hz.ywan-chungtsiang.top/gtqspmxntu.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtqksqngcs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtfyclzrwm.html

PHP:  sort($arr);
来源：http://hz.ybcxt.top/gtlxmclvkt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aibaodan.cn/gtastjgwjk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtbkhvjlsf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.iojbl.cn/gtdnplsxcs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtonjfejod.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtbbqzshml.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtvxwpmyjv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtycawqpad.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtpvfzqqov.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtdhpsxxjm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtoguzodlb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtcisifnmw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.meibo888.top/gtoedfedau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xingfuxueyuan.xyz/gtbemaahxb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtixkfkxsb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtiifutlzt.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtugncekac.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigufen.top/gtuceskijb.html

PHP:  array_reverse($arr);
来源：http://hz.hysaishi.cn/gtccpjcghe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hongshengwenyu.top/gtxdeavisg.html

TS:   [...arr].reverse();
来源：http://hz.jinghuilouyu.cn/gtcgahxwxl.html

Java: Collections.reverse(list);
来源：http://hz.hnqzz.top/gtsigwnnue.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gthocqbnvj.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gthzrpvjqy.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtwwokheva.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gtbgxsgcsj.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangkeji.top/gtnnhmfena.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gtgkzrpcwm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtirxqlygm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtgymmipwo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtbnvpukhp.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtghpzghgp.html

Ruby: arr.index(x)
来源：http://hz.zhongyouzk.top/gtaudhcvnc.html

C#:   list.IndexOf(x);
来源：http://hz.iojbl.cn/gtjuqretkn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.havefunace.top/gtjcgjxdft.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gtiaplndii.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtrrbmhrrn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtowjjrduw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtpvutcwmj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgfzy.top/gtdrdmixsb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aibaodan.cn/gtjqaqqbib.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sweek.top/gtpnyoeuyc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtlqkllmun.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gaohongyu789.top/gtycfcfqei.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zycfv.cn/gtwmqglhwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhijiandao.cn/gtorcpctgk.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtnzxrtwjk.html

TS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtslytjzla.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtkzcfbrly.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtrdbxdbrj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gtlzqdfdtn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtakwbolhk.html

[D15] 去重
来源：http://hz.jqgufenzy.top/gtmjkhigzp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtzcxtcczf.html

PHP:  array_unique($arr);
来源：http://hz.pengpengdd.cyou/gtjueeumtm.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtdwtpsbui.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtutgewfwn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinyuanbaomall.cn/gtiveoosbu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gtpjywirwj.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtaapqhxby.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtzhapyjil.html

[D16] 求和与平均值
来源：http://hz.hongshengwenyu.top/gtncirngqd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtkkbigqqd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtcqqoxpwg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtpvjrdkly.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtoiyogyct.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ehwqpu.com/gtizpfmgps.html

Go:   // 手写循环累加
来源：http://hz.redwolf501.top/gtfjymubhu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jyoumei.cn/gterqsntdc.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtvugzgcme.html

[D17] 最大值与最小值
来源：http://hz.hnxiangtu.top/gtuqqgeons.html

Py:   max(arr);  min(arr)
来源：http://hz.tanke756.top/gtxzvqpibw.html

PHP:  max($arr);  min($arr);
来源：http://hz.fzhhl.top/gtbhrpxkhe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtlfykywgc.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gtdwzpuoxa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtwfbqryix.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gteemupzti.html

Ruby: arr.max;  arr.min
来源：http://hz.zhongyouzk.top/gtyxkniwmc.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtpenuusna.html

[D18] 扁平化嵌套数组
来源：http://hz.birdmap.top/gtdjpchcjr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtqerfwhzg.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtazocchys.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtzkfljvsi.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtfpvsxfek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtphckgcqy.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtmlxocrlc.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtxhwijihl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj20258888.top/gtutwpjkav.html

[D19] 按字段分组
来源：http://hz.guowangkeji.top/gthdtjuhzv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtqzeequmn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hysaishi.cn/gtkfotkbyn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fzhhl.top/gtmhmzuxzs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gthtffgova.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtgkkpmnas.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtqxmjmtuq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtagsevpir.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtsyjijage.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gttcostkgj.html

Py:   Counter(arr)
来源：http://hz.xuanzx.com/gtmleadyiz.html

PHP:  array_count_values($arr);
来源：http://hz.cqqwz.cn/gtvooqcxmf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtfdqhznzl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtztoebgza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtfczruqor.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtespgqpac.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtuyweqklz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ehwqpu.com/gtciaxzxxv.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtfciwhpht.html

Py:   x in arr
来源：http://hz.jiagoushi.top/gthmibwpmg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenjidiqi.icu/gtrodtksju.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtmovtosgh.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtzqvvwxwe.html

Java: list.contains(x)
来源：http://hz.nwbrower.top/gtbafzphxc.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gteozobmdu.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gtlpbuoylp.html

C#:   list.Contains(x)
来源：http://hz.guannengcc.top/gtoqlahglg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtkqffyyqw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtqfygejai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtrpkboqir.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gthsjsctha.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtkvvyshxr.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtrzctdnmk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gttnerzitg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtxtnoirgs.html

C#:   new List<int>(list);
来源：http://hz.gogol.net.cn/gtcxyxhkru.html

[D23] reduce 累积计算
来源：http://hz.zhengqikj.top/gtlxspxsda.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtglyleqna.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gtpbcvjydb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtaxmzhvld.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sxryk.cn/gtwjgighud.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtngogzres.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtadmeebkb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtzgnkzscp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtkcgdjejr.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtrnsftgdx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tanke756.top/gtkgwbnhma.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtkqtgvrxm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtqqfgtolb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zdqjudy.top/gtukjkszzd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtxegbyikq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gogol.net.cn/gtstqefgmk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangkeji.top/gtexwxbdtj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtxqjjxebu.html

[D25] Set 集合去重与交并差
来源：http://hz.zycfv.cn/gtsfuiqmey.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtzfucwbrq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgfzy.top/gtnbwkqtrv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yongpay.top/gtfrzkzmgw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtjmslshxp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtrgvisuek.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtnwfdecnn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtqffpdvcu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtzyjolhun.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gtkksrwols.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtrpsfiflq.html

PHP:  implode(", ", $arr);
来源：http://hz.xuanzx.com/gtauxwgypo.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtoiutjxip.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtrtbmeiij.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtjyyhuybw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gtxfcmuoeh.html

Ruby: arr.join(", ")
来源：http://hz.guowangkeji.top/gtdiknbtif.html

C#:   string.Join(", ", list)
来源：http://hz.zhixingplan.top/gtyuygrkcx.html


<!-- 参考信息 -->