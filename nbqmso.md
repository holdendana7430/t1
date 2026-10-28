代发 wailian999

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtguzhcrbg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtpgkzucml.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yueranfly.top/gtlkfoiuzb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtghawdelb.html

TS:   同 JS
来源：http://hz.zdqjudy.top/gtrhmmeilj.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gteqmmjaff.html

Go:   花括号块级作用域
来源：http://hz.aibaodan.cn/gttswlwpoe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.smart0.xyz/gtiilgpccx.html

C#:   块级作用域
来源：http://hz.sxryk.cn/gtuhzpiwnm.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtdjctdcqp.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtbdckjfmt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hongshengwenyu.top/gtvsrcrnjk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.andypj.xyz/gttdjtacfp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.snrcjt.cn/gtndhkifdz.html

Java: import java.util.List;
来源：http://hz.yangfankeji.com/gttskaonsh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gtrkawqngh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ywan-chungtsiang.top/gtvfefamxh.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtxknehpcz.html

[C12] 立即执行函数 IIFE
来源：http://hz.shangyingyoupin.top/gtwrhtewhp.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtlgvyeqqx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xingfuxueyuan.xyz/gtkmzghfnm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtgxzhpdsp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtlwwgpabk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtotqtpqcs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtfhulafxe.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtbdglzwfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guannengcc.top/gtlycdtamv.html

[C13] 类型声明 / 类型注解
来源：http://hz.yanxiufei.cn/gtsxhqbxhm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtnynflvry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtittwxdrk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtgijkmdvz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtbpedvrnw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtoetpfsom.html

Go:   func add(a, b int) int
来源：http://hz.cucudq.cn/gttnbtjout.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fengsongda.top/gtmikjhatj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.quarkkingdee.top/gtvcuxritl.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtftwzzvnv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgufenzy.top/gtaqvjpqjo.html

PHP:  // 无泛型
来源：http://hz.0kj1m.cn/gtzjrwfuxg.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtvgqgeqsa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtvjjzwbid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gtaxabyolr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtpgqdrbue.html

Ruby: # 无泛型
来源：http://hz.ppjwa.cn/gtiurihccc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtaodvfkxq.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtliavrkue.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtepetccci.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuetiantiany.cn/gtsxmoftam.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtqkqgcvby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtujfbaipq.html

Java: // 无解构
来源：http://hz.jlsjyb.cn/gtvzvypwps.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gtbgdrbebt.html

Ruby: a, b = pair
来源：http://hz.hysaishi.cn/gtvlujqqzi.html

C#:   var (a, b) = pair;
来源：http://hz.dashuyun.cn/gtjshmwvdn.html

[C16] 函数 / 方法重载
来源：http://hz.ywan-chungtsiang.top/gtaygxnzdx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gtqblfpdtc.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtrhrntkhs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtckcigrns.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tanke756.top/gtzzprmdon.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guowangkeji.top/gtmddkfidj.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtclltwxmx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigfzy.top/gtqgssvawj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.bjfxy.top/gtpjwzmfcf.html

================================================================================
来源：http://hz.tianlin.xyz/gttptohumi.html

D. 数组 / 列表 / 集合
来源：http://hz.andypj.xyz/gtelgugsrb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjgooxebw.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtiqrezayc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtqzuqizxm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gthbjqjmop.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258888.top/gthcnbsrph.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gaohongyu789.top/gtacooldxv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jlsjyb.cn/gtdimjywdl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtpuwoymry.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shuidangran.top/gtoywfxvee.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtrlsuliul.html

[D02] 追加元素到末尾
来源：http://hz.kuanghao11.cn/gtvzrdrsxu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hywenlv.cn/gtkvidojuf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtywrjkjcr.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gtrxlaosmu.html

TS:   arr.push(4);
来源：http://hz.xinyue.icu/gtfjwnuwgr.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtdhnqybci.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtklryicoh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hysaishi.cn/gtjadezjsa.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtblsbvgrh.html

[D03] 在指定位置插入元素
来源：http://hz.hongshengwenyu.top/gtxproxsec.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtchfstuqg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtnxbcqzdd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuxming.cn/gthphuudyx.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shangyingyoupin.top/gtywuhyazr.html

Java: list.add(0, 0);
来源：http://hz.aibaodan.cn/gtyihaqgjm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtsohnzmff.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtqdqloint.html

C#:   list.Insert(0, 0);
来源：http://hz.zhaomingkeji.xyz/gttyzfroim.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtfbfrxgfu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zdqjudy.top/gtegjkuizk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.mhx1999.top/gtxuotarov.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cheryme.top/gtznenuylz.html

TS:   arr.splice(0, 1);
来源：http://hz.yonumen.top/gtxvigtfuz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtepmbtxkw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtpzvjdgjr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gtivmdytdr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtpkmabobg.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gteghlbjza.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtgkketuxi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cucudq.cn/gtmmbokqhj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sufxvd.cn/gtypraruiy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtlyhrrwyg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtygixydag.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtdncuhlzi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtelxbfrbn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtixjbdkys.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtyohhpfyu.html

Py:   len(arr)
来源：http://hz.wangshuangyany.cn/gthlgugdug.html

PHP:  count($arr);
来源：http://hz.yuanzhike.top/gtqsgbxras.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtxpftnmdw.html

TS:   arr.length
来源：http://hz.zhengqikj.top/gtqsedwcqw.html

Java: list.size();
来源：http://hz.shzxlz.cn/gtoobdkeok.html

Go:   len(arr)
来源：http://hz.hammf.cn/gtjlyzhepo.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtgcfvmxcv.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gthxrlejed.html

[D07] 切片 / 取子数组
来源：http://hz.daxiang520.top/gtbldxpcqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtttplbqjh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gtyigifevm.html

JS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtzpbtvtqd.html

TS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtpkldpked.html

Java: list.subList(1, 4);
来源：http://hz.jinqigufen.top/gtqpcbdtzz.html

Go:   arr[1:4]
来源：http://hz.shzxlz.cn/gtqtvjdnbm.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtwvqpyjwu.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtousvymws.html

[D08] 合并两个数组
来源：http://hz.aizwys.cn/gtwbtggtea.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnxiangtu.top/gtkmlpmmlz.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtgnbvjmqm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cqqwz.cn/gtqjwxhhnu.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtilianvrx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtkvtnjzzy.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gtfnsyrglk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gthguugrhx.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtrvlzekjt.html

[D09] 排序（升序）
来源：http://hz.yuxming.cn/gtgcbuuinw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtyqwzqidc.html

PHP:  sort($arr);
来源：http://hz.shzxlz.cn/gtkkkbfhws.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.52xcode.cn/gtptpyeklr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gtddherpgb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenjidiqi.icu/gtudmunxqo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtvxqehrqq.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtjyzieydd.html

C#:   list.Sort();
来源：http://hz.gotoacloud.top/gtdfcvraea.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtgdxbkurh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtvqmjylbl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtfqhbmivt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtvwqglkhc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtckmxoabt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtnxwiyfri.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.meibo888.top/gtvfrjegzt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigufen.top/gtxdahxukm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtljvfnwja.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gthlhdprnh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dianchejie.cn/gtqkdjfgim.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gtrucwhqtx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xingfuxueyuan.xyz/gtouhxlbnd.html

TS:   [...arr].reverse();
来源：http://hz.tanke756.top/gtmxuuanaa.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtbfxkxzei.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtrguvxdoj.html

Ruby: arr.reverse
来源：http://hz.birdmap.top/gttjvzriau.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtvjkjhhfn.html

[D12] 查找元素下标
来源：http://hz.dashuyun.cn/gteohsippe.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtjfxoubkj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtldeaonhp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtctwijlmr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtdociriqx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtvstzwvqk.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gtpdzqdyco.html

Ruby: arr.index(x)
来源：http://hz.sufxvd.cn/gtlimrgiln.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtghbndgvn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ehwqpu.com/gtfsddvyht.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhongyouzk.top/gtnruakgrv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gttvlvklxb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtjnzbyzji.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtjbvtngbe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangdashe.top/gthvluatyj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenzaomai.com/gtipaonmby.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangshuangyany.cn/gtrgyuqqjs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.andypj.xyz/gtwxmgcahd.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhijiandao.cn/gtyvkxcanh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtvafdfdxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxuanxn.top/gteqbzfdah.html

JS:   arr.map(x => x * 2)
来源：http://hz.ydzc1.top/gtylbtjvoy.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtfvyjykal.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtplygqvrx.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtelmwsbyc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shuidangran.top/gtowjuxwmo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.andypj.xyz/gtrwsagsnm.html

[D15] 去重
来源：http://hz.c1oappe.top/gtldgnhkeh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtfbiltgil.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtdqnpbjtv.html

JS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtikwyhigf.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtnkffyjrt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtksiqcyjc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.dashuyun.cn/gthwxvgfif.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtxjezkreo.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtukadjtcq.html

[D16] 求和与平均值
来源：http://hz.iojbl.cn/gtvnzacwqh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigfzy.top/gtfebuzgga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtebnckrpz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtgjkmxxlm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtwkoxafnm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yueranfly.top/gtkqbxkgmi.html

Go:   // 手写循环累加
来源：http://hz.hysaishi.cn/gtuawearhh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnqzz.top/gtxrjlodro.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gtbqxeldwu.html

[D17] 最大值与最小值
来源：http://hz.zhijiandao.cn/gttyktwcos.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtpmlljwmx.html

PHP:  max($arr);  min($arr);
来源：http://hz.gaohongyu789.top/gtawenkxll.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nwbrower.top/gtffrdvccy.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtoolyjbwr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cheryme.top/gtuwwyhkvc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtsngbihkk.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangtech.top/gtqygttsen.html

C#:   list.Max();  list.Min()
来源：http://hz.hnxiangtu.top/gtrgqdygok.html

[D18] 扁平化嵌套数组
来源：http://hz.dashuyun.cn/gtrlzqmnfi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtbreyillc.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtvstvnagq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtwhhixxit.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtdoouavxw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtjvxqzntr.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtptpbothe.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gtgqhxwtbu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cdnleiting.top/gtdssdhkwe.html

[D19] 按字段分组
来源：http://hz.jianghu66.top/gtuxjddoxt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtjthlpglx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hywenlv.cn/gtxhdplssi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtiihqtyfl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gttosuhmfa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gthtvdxgiz.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtqcodxecv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtljfmtiwc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtbofqhnli.html

[D20] 统计每个元素出现次数
来源：http://hz.tianlin.xyz/gtybhvfxes.html

Py:   Counter(arr)
来源：http://hz.sysykeji.top/gtzdfwelwa.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtagtwjkzv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtxchnwkwv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtnsqklvnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gtzvisbatu.html

Go:   // 手写 map[T]int
来源：http://hz.redwolf501.top/gtzpifczhd.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtgkbvwmlg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yongpay.top/gtyfoemcpp.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gtkfpfiyes.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtmlpmuwyb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shuidangran.top/gtcjllmaxd.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtjmerfmyd.html

TS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtporhhdep.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gtpdrefomd.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtjtibfqge.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtqnvdgxvh.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtxfqzwkkv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yanxiufei.cn/gtnmxicxkh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gtixzbydjs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.smart0.xyz/gtzyajfzvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.redwolf501.top/gtbfpjkwlu.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gttpbaoajm.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtjyflstrr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guowangkeji.top/gtecuajkss.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gtvcwjnabq.html

C#:   new List<int>(list);
来源：http://hz.ydjk.org.cn/gtyhpchjuc.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtvmvzchgz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtetoniqrg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tian-w.cn/gtyjxhoxvy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gteojoywdy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtyjwddqol.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtyzxsclrl.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtnehpbfve.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtrrmnrsuo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.316326.xyz/gtwdfpmdkc.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtgovziinf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hywenlv.cn/gtiodxvyfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shangyingyoupin.top/gtxxyvgmfu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtcierpzao.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtwamzjgzg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhengqikj.top/gticnrcwjy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yueranfly.top/gtkkpbknys.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtvzgrgkmo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yanxiufei.cn/gtjzdimrdf.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtpzeufpwt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtigovolfv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daxiang520.top/gtstrphvhe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj20258.top/gtgyzueroo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtncftvagt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtnhaaexvd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtklbwqkcr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtdpzppzyd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtrurpokvs.html

[D26] 数组转字符串
来源：http://hz.xuanzx.com/gtwcxkfrif.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hongshengwenyu.top/gtaiewrorf.html

PHP:  implode(", ", $arr);
来源：http://hz.xylfe.cn/gtbokohkyv.html

JS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtexlytxax.html

TS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtdvjrplnq.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtetpqtueu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtzqzkxedz.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtxymeyvfi.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gtgpenvwjx.html


<!-- 参考信息 -->