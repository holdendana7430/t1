代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtekgckmca.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gtnthxoofl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtrjznfmyq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtzcxmxqsu.html

[C10] 变量作用域
来源：http://hz.sufxvd.cn/gtnpjmkhdk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nwbrower.top/gtormzvdvy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtmvbuepop.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtvzudhpao.html

TS:   同 JS
来源：http://hz.zhengqikj.top/gtypjgyqsx.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtvfopugtj.html

Go:   花括号块级作用域
来源：http://hz.jiagoushi.top/gtfymrbrui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtdvnpvzhi.html

C#:   块级作用域
来源：http://hz.jiagoushi.top/gtmeacvkhy.html

[C11] 模块导入与导出
来源：http://hz.svipenyu.cn/gtqknvzbrz.html

Py:   from module import func
来源：http://hz.daxiang520.top/gtxfsokolu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xuanzx.com/gtrveahbly.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.birdmap.top/gtyminhsjb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gthgqlyaut.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtahbkczce.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gogol.net.cn/gtkrwbigpo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hysaishi.cn/gtqxbfljib.html

C#:   using System.Text;
来源：http://hz.iojbl.cn/gtupxpaqen.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtuxbjfmzh.html

Py:   (lambda: print("run"))()
来源：http://hz.pengpengdd.cyou/gtitmhtluc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtefbigpvf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtusgfxyps.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtrroydsje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gtkvepvmgx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangtech.top/gtqxmnfulh.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtvnmxkeda.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtxnmtuawc.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gtmldcoovv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuetiantiany.cn/gtpzzcdrel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtmyeyoypm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinqigfzy.top/gtatfhvtgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtapzodcii.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtlpokwbqa.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtnipxknvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hnxiangtu.top/gthugybenl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtswlynplu.html

[C14] 泛型函数
来源：http://hz.sufxvd.cn/gtqofocigq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtrmlyxvmg.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtrhgqneze.html

JS:   // 无泛型
来源：http://hz.hnxiangtu.top/gtuxswvxjj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtanqezyje.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtylpddbvs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgfzy.top/gtlsuudyag.html

Ruby: # 无泛型
来源：http://hz.yangfankeji.com/gtpoiwzazk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gotoacloud.top/gtxjdcqlrb.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtguvckcro.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gthrayulca.html

PHP:  [$a, $b] = $pair;
来源：http://hz.mhx1999.top/gtssrtkwos.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtxxwrigdn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtkfhrwpnt.html

Java: // 无解构
来源：http://hz.guannengcc.top/gtzlcshege.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtogbeyatb.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtigceuaeu.html

C#:   var (a, b) = pair;
来源：http://hz.hnxiangtu.top/gtjcvvbmxa.html

[C16] 函数 / 方法重载
来源：http://hz.xinyue.icu/gtogbaaroa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.feifeiyinyue.top/gtpmbtkhyk.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtpvjxgcmv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gttlwbkrgn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gthuwmjxeo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.bjfxy.top/gtguxuzrwd.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtdebmafub.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtnjuhvtfv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sufxvd.cn/gthptyzeah.html

================================================================================
来源：http://hz.tian-w.cn/gtbepfyxod.html

D. 数组 / 列表 / 集合
来源：http://hz.quarkkingdee.top/gtgmfqejrp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrqkiqumh.html

[D01] 创建数组 / 列表
来源：http://hz.nanxinkj.top/gtlqxmjqbi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtcinillnh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gtckwjyjor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj202588.top/gthtsenrvs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtswgtustj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yvedp.cn/gtvklcaepv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tianlin.xyz/gtfhyrzifl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gtdsppaezw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cqqwz.cn/gtneljgjho.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtsbarvanu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtngvgwlyy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtxvpxllky.html

JS:   arr.push(4);
来源：http://hz.sufxvd.cn/gtrjmdgzaw.html

TS:   arr.push(4);
来源：http://hz.zhixingplan.top/gthutwffvo.html

Java: list.add(4);
来源：http://hz.jqgufenzy.top/gtqgyvjbjm.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtnkcpanlf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtwlseafta.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gttkggatzw.html

[D03] 在指定位置插入元素
来源：http://hz.ydjk.org.cn/gtnggyoeou.html

Py:   arr.insert(0, 0)
来源：http://hz.meibo888.top/gttmlmznhk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtrcqzfehv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigufen.top/gtnylurarm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gtjwzriwmx.html

Java: list.add(0, 0);
来源：http://hz.tian-w.cn/gtyvyxyqnz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnqzz.top/gtwwtcmagm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jyoumei.cn/gteerkjxkn.html

C#:   list.Insert(0, 0);
来源：http://hz.tanke756.top/gtietuaztf.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtkjbmsqnl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtycshfmrx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtowyggqtr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ppjwa.cn/gtikjrdkfn.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtexzmdjen.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtjkdudssd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258.top/gtsxfheqli.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtbvojhwix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yonumen.top/gtvyqpmken.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtbewkigwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtvhurczuk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.birdmap.top/gtkdavhjaq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.svipenyu.cn/gtctqfcvqo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtxvhyqjws.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtoynayqjz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtuzyvjojh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtjmmrponp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hywenlv.cn/gtmhldterp.html

[D06] 数组长度
来源：http://hz.chenjidiqi.icu/gtheowplud.html

Py:   len(arr)
来源：http://hz.bjfxy.top/gtqbuvwvtg.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtikelfrle.html

JS:   arr.length
来源：http://hz.yj20258888.top/gtfztsbgrm.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtnyifiynx.html

Java: list.size();
来源：http://hz.svipenyu.cn/gtokoeihat.html

Go:   len(arr)
来源：http://hz.guowangkeji.top/gtixrczydj.html

Ruby: arr.length; arr.size
来源：http://hz.ybcxt.top/gtimmxmrxl.html

C#:   list.Count;
来源：http://hz.xuetiantiany.cn/gthuhatbey.html

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gteukieivi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.pycfn.com/gtjqpjnqiq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shzxlz.cn/gtcfzqkvst.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtmvcdqxta.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtbdyirluo.html

Java: list.subList(1, 4);
来源：http://hz.cucudq.cn/gtghdggrkr.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gthomeqyfd.html

Ruby: arr[1, 3]
来源：http://hz.sufxvd.cn/gthecebltb.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtromnqone.html

[D08] 合并两个数组
来源：http://hz.chenlongwang.top/gthfyvpouo.html

Py:   a + b;  a.extend(b)
来源：http://hz.shangyingyoupin.top/gthsymslra.html

PHP:  array_merge($a, $b);
来源：http://hz.hywenlv.cn/gtrfwamrey.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtsnthtuuv.html

TS:   [...a, ...b];
来源：http://hz.52xcode.cn/gtrrabsosk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtovczlmcn.html

Go:   append(a, b...)
来源：http://hz.zhaomingkeji.xyz/gtdscoraae.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtfdtqmssc.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuanzhike.top/gtuukcazsb.html

[D09] 排序（升序）
来源：http://hz.chenlongwang.top/gtrildmiup.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtuhnadymz.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtkfibzglv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtytryuuns.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gtkmbgqkof.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.meibo888.top/gtocxecmac.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtaitzduwg.html

Ruby: arr.sort
来源：http://hz.jianghu66.top/gtbopfldma.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtbvlaaqri.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhoulong.xyz/gtoprvydbm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cdnleiting.top/gtwcerowbb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtsmhnhhwa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtrohrouah.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtryqoqntw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cucudq.cn/gthfsknifl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hfpthk.cn/gtgftbmjhj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtsiaoyqeh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtmybmcdhv.html

[D11] 反转数组
来源：http://hz.andypj.xyz/gtljtflhst.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtarozkqle.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtqcfqzoha.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gttfnbssma.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtgnelecfs.html

Java: Collections.reverse(list);
来源：http://hz.zdqjudy.top/gtinbrrthc.html

Go:   slices.Reverse(arr)
来源：http://hz.gzhubu.top/gtungbisih.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtqgaxipkq.html

C#:   list.Reverse();
来源：http://hz.zhongyouzk.top/gtneflruke.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtxtbfbehy.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtziynqfgt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jlsjyb.cn/gttffraxfs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.316326.xyz/gtaurxdwdi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gtwgocogcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zycfv.cn/gthwdzrxdc.html

Go:   slices.Index(arr, x)
来源：http://hz.ppjwa.cn/gteoftxcxm.html

Ruby: arr.index(x)
来源：http://hz.aibaodan.cn/gtpslsmgip.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtcfiixqnk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cheryme.top/gtnzgyjkmx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pycfn.com/gtprfhgcfr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shuidangran.top/gtvfmcayoo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtpsxthxfm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtlkncwkxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.mhx1999.top/gtmfalbbgu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jiagoushi.top/gtzjnozewo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gttctfoerf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtgrnumatz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guannengcc.top/gtpttrvgcy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigufen.top/gtcoqtuzkr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtpbiqfjfu.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtotyfthgd.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtsujgqchp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.birdmap.top/gtkeokcgoi.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtatmaqgfp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtuptwriya.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtcgizhhxi.html

[D15] 去重
来源：http://hz.iojbl.cn/gtlzzgnrwz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtpmpsinvk.html

PHP:  array_unique($arr);
来源：http://hz.pengpengdd.cyou/gtydwavxaz.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtmxavmjqv.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtqvhonlax.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtilygwudm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhoulong.xyz/gttgcpeibh.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gtwhciswkc.html

C#:   list.Distinct().ToList()
来源：http://hz.hfpthk.cn/gtdukwrhpn.html

[D16] 求和与平均值
来源：http://hz.yanxiufei.cn/gtqkmjinti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gttcwduphb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtqqjdpqdy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtdncablus.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtaewcsyyq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtalfdddgv.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gturqljvja.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ppjwa.cn/gtkxdoxtep.html

C#:   list.Sum();  list.Average()
来源：http://hz.zdqjudy.top/gtiqakvfhi.html

[D17] 最大值与最小值
来源：http://hz.nanxuanxn.top/gtsoewwijq.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtfiupjhev.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtmlaenddw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ehwqpu.com/gtydnajgif.html

TS:   Math.max(...arr);
来源：http://hz.aibaodan.cn/gtkzantfbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shangyingyoupin.top/gtpdhxorbw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.0kj1m.cn/gtykbrgxnb.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtpuuqqhzy.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtwgvywzqb.html

[D18] 扁平化嵌套数组
来源：http://hz.ppjwa.cn/gtfezdsdaf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.bjfxy.top/gtijzuzode.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtqamwtlam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtnpwhrqxs.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtpelihlvj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtgftfxfmh.html

Go:   // 手写双层循环
来源：http://hz.sysykeji.top/gtlumunlvi.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtqhhbnjol.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.redwolf501.top/gtsfkiksko.html

[D19] 按字段分组
来源：http://hz.gogol.net.cn/gtxirztzal.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daxiang520.top/gtldcuavza.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gtcecxraoz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sxryk.cn/gthzhpeekl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtcakxrtju.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ppjwa.cn/gtgxgcxwia.html

Go:   // 手写 map[string][]T
来源：http://hz.quarkkingdee.top/gtzngucvor.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtvvebdqeg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.316326.xyz/gtpaflctna.html

[D20] 统计每个元素出现次数
来源：http://hz.feifeiyinyue.top/gtwyhjskki.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gtzkkpxnnh.html

PHP:  array_count_values($arr);
来源：http://hz.gaohongyu789.top/gttjggeoxh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gturdocxng.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtytaclcys.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.mhx1999.top/gtivkisede.html

Go:   // 手写 map[T]int
来源：http://hz.redwolf501.top/gtjgapdabk.html

Ruby: arr.tally
来源：http://hz.shanyushiyangtech.top/gtwwijkgqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtqcyjdtfu.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtwfiavezj.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtmdxmfokq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.snrcjt.cn/gtvutmfokb.html

JS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtxhufjkhs.html

TS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtcfgjsqdt.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtwuezvrsc.html

Go:   slices.Contains(arr, x)
来源：http://hz.havefunace.top/gtkgbrrdbw.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtisnvpfry.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtfnrwjfrb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhongyouzk.top/gtbbfdpsnd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sweek.top/gtxoshhcoc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtifzaxugg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gtklvxcmvl.html

TS:   [...arr];
来源：http://hz.zhixingplan.top/gtzauagoic.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtiskfcshq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtnjuvghqs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ywan-chungtsiang.top/gtohjnqmbq.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtzjibvvod.html

[D23] reduce 累积计算
来源：http://hz.daria6918.cn/gtpcidtipz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtzgbntyow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtyowxaakl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtmnphpijx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuanzx.com/gtbssjavzi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtotygsnjp.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtnmmihpcr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pycfn.com/gttwhevuwc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guowangkeji.top/gtsrlnfsqz.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtwknvybro.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtytknfoov.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtrufzlqyn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnxiangtu.top/gtjsapdjnr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtdtvxwalw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gtovdcgnst.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gtnazpdves.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cdnleiting.top/gthsvybzic.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtkjnboasb.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtqzavmgrd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shzxlz.cn/gtgvflcdae.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guowangkeji.top/gtquvkrddl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.9152youxi.cn/gtksvlhked.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtjhbhizhk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.pengpengdd.cyou/gtfbfdzwmj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pengpengdd.cyou/gtysvekrxq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtczsoaqut.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtqhlyddky.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtniaglbyf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtdtddxwoi.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigufen.top/gtpcvtvjxp.html

JS:   arr.join(", ")
来源：http://hz.c1oappe.top/gtypaqbarn.html

TS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtposasakn.html


<!-- 参考信息 -->