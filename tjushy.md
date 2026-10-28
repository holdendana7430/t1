代发 wailian999

[C10] 变量作用域
来源：http://hz.zhongyouzk.top/gtslavubmz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jiagoushi.top/gtabjkrckn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgfzy.top/gtxnpzhpaj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yangfankeji.com/gtibfdpskv.html

TS:   同 JS
来源：http://hz.redwolf501.top/gtbbeqymfz.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gtpffbphqq.html

Go:   花括号块级作用域
来源：http://hz.zhaomingkeji.xyz/gtvasazueo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jlsjyb.cn/gtwwmwcnlj.html

C#:   块级作用域
来源：http://hz.vqdsnc.cn/gtferebumw.html

[C11] 模块导入与导出
来源：http://hz.zhengqikj.top/gtiqrkwuhx.html

Py:   from module import func
来源：http://hz.havefunace.top/gtvgdywpgi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gthlgczpzr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtzledznny.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtspkegohy.html

Java: import java.util.List;
来源：http://hz.hnxiangtu.top/gtdjvygzuy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtwebysahs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydjk.org.cn/gteyhjgffn.html

C#:   using System.Text;
来源：http://hz.xingfuxueyuan.xyz/gtxisrofsk.html

[C12] 立即执行函数 IIFE
来源：http://hz.cheryme.top/gtpvxkvbmo.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtbjbrhncv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtvqbpcavq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtgyuxeqqp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtkecnzlqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhaomingkeji.xyz/gtwwdkriqx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtavafzcie.html

Ruby: -> { puts "run" }.call
来源：http://hz.xylfe.cn/gtmrlqhswx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gtgeyogtip.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtkvfwxfpt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtnftexxrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtoeuwetnk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangdashe.top/gtkkoowfhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtnqmcnbls.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtzingwxzb.html

Go:   func add(a, b int) int
来源：http://hz.tian-w.cn/gtmyvovnvn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ivvv.top/gtncpweqso.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ehwqpu.com/gtpbqyaqis.html

[C14] 泛型函数
来源：http://hz.yvedp.cn/gtzdvuglft.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtmgrigwlk.html

PHP:  // 无泛型
来源：http://hz.vqdsnc.cn/gtnvwfkrwg.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtemukvndr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtqahmoeby.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.0kj1m.cn/gtgxyotgut.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtuzysgpva.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtfqnhmnzh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtqzmfqvpq.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gtfzwaprtl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gthnrpiypa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtunlmenoq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gteebsymvl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtssxzsjoi.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtaiydykif.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gthttswnpn.html

Ruby: a, b = pair
来源：http://hz.hnxiangtu.top/gtupnszawg.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gttdubprml.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtoarktfwj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangkeji.top/gtvugaayew.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtokvtjqxt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtwwsmuebh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigufen.top/gthwcdjxjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sweek.top/gtwzgjymxt.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gttreszpyp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gtmodyurwh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gtyemygnwi.html

================================================================================
来源：http://hz.mhx1999.top/gthjwpbkjk.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtgzmzoebj.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxeqnqllj.html

[D01] 创建数组 / 列表
来源：http://hz.tanke756.top/gtvmmltcmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtmzfhtczt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtvvqklxhy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yongpay.top/gtyxfkwjan.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtssyetqxr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xziqi.cn/gtjwdopdrc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.birdmap.top/gtgqsquwdr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtjoyulpus.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sweek.top/gtqtulvpvk.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtakuehzvp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.316326.xyz/gtogplxrvp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.316326.xyz/gtmhpecvby.html

JS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtrohpartg.html

TS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtdqlpqkdg.html

Java: list.add(4);
来源：http://hz.zhongyouzk.top/gtzljpfjxe.html

Go:   arr = append(arr, 4)
来源：http://hz.zhengqikj.top/gtyvrsleso.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj202588.top/gtcsscjcxs.html

C#:   list.Add(4);
来源：http://hz.nanxuanxn.top/gtrrexxdjd.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtmuvbaakp.html

Py:   arr.insert(0, 0)
来源：http://hz.fengsongda.top/gtijzloafu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnqzz.top/gtflfrojxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtwlhlijlw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gthlldfrki.html

Java: list.add(0, 0);
来源：http://hz.shuidangran.top/gtrfdzpjkt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtdunkurcm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtadxxwlzx.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtwogesgvj.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtuffxqhdm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gteqespazv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cucudq.cn/gtvezuxlhz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinghuilouyu.cn/gtezoefsux.html

TS:   arr.splice(0, 1);
来源：http://hz.hammf.cn/gtumkeeomn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtivzbgemp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinghuilouyu.cn/gtrqiyocfk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtoznrhenr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gttiazhljn.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gtphrqiflj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtiumosqic.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gtacpqdqtz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtpqdxqcrg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtsnmreigg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtqwzykqmv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtnshogjgb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtmfkpmzth.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cdnleiting.top/gtnvralskf.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtuopopzwu.html

Py:   len(arr)
来源：http://hz.cdnleiting.top/gtbesrswey.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtyqlvtded.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gtuylnezbe.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtximgyhcw.html

Java: list.size();
来源：http://hz.zhengqikj.top/gtbebbxuog.html

Go:   len(arr)
来源：http://hz.yongpay.top/gtzgtqiuvg.html

Ruby: arr.length; arr.size
来源：http://hz.svipenyu.cn/gtwhbatxix.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtnmlmogwd.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtmmeyadvw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtuvvkeacx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtocuajatj.html

JS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtdbtmriyh.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gthvjjsgas.html

Java: list.subList(1, 4);
来源：http://hz.hnqzz.top/gtjcfnpvpj.html

Go:   arr[1:4]
来源：http://hz.yj20258.top/gtjawcxtfh.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtsmnfnojd.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtaotxnnhc.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtvdtsbkgb.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtvkkkfnxy.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtszdennjs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtmfhasjbb.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtrtabsnnj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tianlin.xyz/gttgjzqkwc.html

Go:   append(a, b...)
来源：http://hz.cashguo.top/gtmhbyiutg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtpxkdyfns.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtmpjwlupw.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtimmxraly.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtzfdkbapj.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtiodfxllk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ehwqpu.com/gtlideoakw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtallbqqvx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtzmgafzws.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.52xcode.cn/gtyjfczbsu.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtpwzjatot.html

C#:   list.Sort();
来源：http://hz.xylfe.cn/gtkgtyugno.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daxiang520.top/gtehgkkhqx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shzxlz.cn/gtwybpttig.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtkojcbgxv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtxvaioggn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtmnhzwyop.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtygcelfje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xziqi.cn/gtzcoyxlht.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cqqwz.cn/gtccukdeyb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.smart0.xyz/gtstzexokq.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gtwypivtjf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gtuhwllzcf.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtgpuutzcy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.0kj1m.cn/gtcivujzsn.html

TS:   [...arr].reverse();
来源：http://hz.tianlin.xyz/gtlucdnjlw.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtiewruvgr.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtoaafcpot.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtzxrkkkrd.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtolhvysqk.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtuzvzgncn.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhoulong.xyz/gtevwvrtog.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtqnrmesbt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gttmhqtofw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gttujbkmgt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.redwolf501.top/gtfynzymnl.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtkrzssxiy.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtqrpihiah.html

C#:   list.IndexOf(x);
来源：http://hz.pengpengdd.cyou/gtuvmrmyyq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pycfn.com/gtsqzgafhg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tanke756.top/gtdtphsala.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gzhubu.top/gtuytjszrs.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtqrrzymmp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtdzqqalqo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtulpiylhw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtpyamihdo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jianghu66.top/gtiavizvnt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtpmsymiun.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtlcfoxrmn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigfzy.top/gtuzvngovs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtyhsedbsk.html

JS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtclazegit.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtqbemewvj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhongyouzk.top/gthztdffeg.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtdfzknjsh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nanxuanxn.top/gtdrkgnmhn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtvddqskam.html

[D15] 去重
来源：http://hz.xinyue.icu/gtnrnwemxz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangkeji.top/gttxrwlunx.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gthuhuxvco.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtxqticqra.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gthaizmbbl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtguhipjsz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ydjk.org.cn/gtynhyhvxc.html

Ruby: arr.uniq
来源：http://hz.yvedp.cn/gtghdnpjcp.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtpirgjify.html

[D16] 求和与平均值
来源：http://hz.daria6918.cn/gtfejldltf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gtpmpoafwd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.meibo888.top/gtwlbcngky.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtihdzeqdn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtqtluwycu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtzjvdqvnr.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtotgmnbyd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtsurcaend.html

C#:   list.Sum();  list.Average()
来源：http://hz.xziqi.cn/gtwycixrqz.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtxanrjdqs.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtgwaxmwgq.html

PHP:  max($arr);  min($arr);
来源：http://hz.tanke756.top/gtdlxvjwif.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinghuilouyu.cn/gtvkcpsbrj.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gtrfrmyuzy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtidezwwon.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gtbtpuquvd.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtkiqrapiz.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtlwckqxic.html

[D18] 扁平化嵌套数组
来源：http://hz.zhengqikj.top/gttosurlyq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtaexviqdd.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gtepyuhtkv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gtemanegdb.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtlquvoyas.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtkeehedqu.html

Go:   // 手写双层循环
来源：http://hz.sysykeji.top/gtzqdcaqts.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gtwgtbwxwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.snrcjt.cn/gtuhorpxfe.html

[D19] 按字段分组
来源：http://hz.shzxlz.cn/gtwtltferd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtzgyxkvfg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.c1oappe.top/gtnoegwfye.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guowangkeji.top/gtbttmncfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtfoldzlnm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuetiantiany.cn/gtamoeclvo.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtgzljtxyc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtjjbqxist.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtohacvcul.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtmxkzsrig.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtxpvdllax.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtcyglsoeb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtxnqitlpc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gttwaugevb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtdnzaxvem.html

Go:   // 手写 map[T]int
来源：http://hz.fengsongda.top/gtuxvocsmj.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtmtgzxxrh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aizwys.cn/gtsbumjacr.html

[D21] 判断是否包含某元素
来源：http://hz.svipenyu.cn/gtxzkkwuii.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gtfdpyspml.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtffymdotc.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtmwsaxzbu.html

TS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtklbbzeft.html

Java: list.contains(x)
来源：http://hz.jlsjyb.cn/gtiyieonuf.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtsffmxfcj.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gthwzwnkkt.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gtqyvwkvhv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtzfmrrtgu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtrpvythwl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gthvtzkwuc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtrkcjrbpo.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtxofvidjd.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtspzvjxsh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gtgfgsunza.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhaomingkeji.xyz/gtmivqanxd.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gthdzekydm.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtcspfamaw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigufen.top/gtdtbhuaxs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gtpwbgyudp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtibmekruw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtduuojndk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ppjwa.cn/gtbhntvlbm.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtzztbjvhy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtdnhgjhtb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nanxuanxn.top/gtvxppyukl.html

[D24] 字典 / Map 基本操作
来源：http://hz.havefunace.top/gtgzlkmwby.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangtech.top/gtirnxmyas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtpezftawv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydjk.org.cn/gtjutppwiv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtfrcfkrin.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtqzldpakl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xziqi.cn/gtnjfohezy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtsjvwhxrx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtukicqdfp.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangtech.top/gtmwqotmtd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtcrdqoemp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuetiantiany.cn/gtprgakfug.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtuwjqavua.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtbzwgelti.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xingfuxueyuan.xyz/gtohdvgtxd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtzkqvzuhu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtfltjdzfa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gaohongyu789.top/gtvrbxrrnj.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtchxouzmh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yueranfly.top/gtyicqrgsa.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtxptrgryv.html

JS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtzyndsegi.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gtyvfpmphn.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtwspytoln.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gttnnwwnip.html

Ruby: arr.join(", ")
来源：http://hz.ivvv.top/gtftzqfuov.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtwhodeagt.html


<!-- 参考信息 -->