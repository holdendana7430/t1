代发 wailian999

TS:   同 JS
来源：http://hz.cdnleiting.top/gtjjxfxhvn.html

Java: 方法内为块级作用域
来源：http://hz.nanxinkj.top/gtdzamuzgr.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gttiseyhsr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtercpqryi.html

C#:   块级作用域
来源：http://hz.jinyuanbaomall.cn/gthdvmnjrg.html

[C11] 模块导入与导出
来源：http://hz.yonumen.top/gtfvwfffvs.html

Py:   from module import func
来源：http://hz.iojbl.cn/gthqklibcs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangkeji.top/gtsklynwcz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtgfbjwkkk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zycfv.cn/gtabrlfhsi.html

Java: import java.util.List;
来源：http://hz.cucudq.cn/gtmnmzwdug.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtlagxopyk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtiktejvom.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtomiccnfr.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtobnasxlt.html

Py:   (lambda: print("run"))()
来源：http://hz.yueranfly.top/gtuwalfqrc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtcryljzpa.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtqfxjazgg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtezowgsfd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gttuxkkcov.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gtewfxaqte.html

Ruby: -> { puts "run" }.call
来源：http://hz.c1oappe.top/gtbdelkkfq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gtyxuiilup.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtmieihnri.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtkhwiujdx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtmamitqgz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gzhubu.top/gtlddubsma.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtfgroftxr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtzafanrdk.html

Go:   func add(a, b int) int
来源：http://hz.fzhhl.top/gtzoxyvjad.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtjxhcvscb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhijiandao.cn/gtxsyoggzd.html

[C14] 泛型函数
来源：http://hz.yonumen.top/gtaereapxe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtkhjmwmre.html

PHP:  // 无泛型
来源：http://hz.dashuyun.cn/gtmmmmcbmq.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtiqqelzmz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ywan-chungtsiang.top/gtjmymkylq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtecnpqbrc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tianlin.xyz/gtmcdcaglm.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtktpznxvm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hammf.cn/gtetwcdyfi.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtwiypcryo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.mhx1999.top/gtglrovvur.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtagtoywkb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtqyfxwasi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nwbrower.top/gtstokvfzd.html

Java: // 无解构
来源：http://hz.ywan-chungtsiang.top/gtyhjrzwus.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtdjersusp.html

Ruby: a, b = pair
来源：http://hz.xinyue.icu/gtaqrjrfvd.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtfhmaaytp.html

[C16] 函数 / 方法重载
来源：http://hz.shzxlz.cn/gtzixpnyjw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ybcxt.top/gtfahvaapt.html

PHP:  // 无重载
来源：http://hz.yj202588.top/gtxibraftf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gtbqwjicgh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtgicarmrs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtfrbrpqmi.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtycxpatys.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtymjjqzbp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtrmgqgata.html

================================================================================
来源：http://hz.guannengcc.top/gtakgpxbtm.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtofwuicad.html

================================================================================
来源：http://hz.guannengcc.top/gttszfqgzf.html

[D01] 创建数组 / 列表
来源：http://hz.sysykeji.top/gtxckxllfb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shzxlz.cn/gtstczxhyo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jiagoushi.top/gtysdsicss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gttkssklyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gttvzgramm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jianghu66.top/gtddlgkqut.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xingfuxueyuan.xyz/gtclwduxzh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnxiangtu.top/gtgqvuaawn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangdashe.top/gtggbnyige.html

[D02] 追加元素到末尾
来源：http://hz.andypj.xyz/gthsnuzrgd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtouhyvrcz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gogol.net.cn/gtigiesfem.html

JS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtzcewsxxz.html

TS:   arr.push(4);
来源：http://hz.cqqwz.cn/gtivdylvry.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtxskdwvjz.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtufjnzfln.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtdhccutax.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtllrpvrzx.html

[D03] 在指定位置插入元素
来源：http://hz.jinyuanbaomall.cn/gthglzlqmp.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258888.top/gtaywjmwvp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sufxvd.cn/gtighbnpuc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtjvecmwcq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.daxiang520.top/gthdnjfwut.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtsnodgnkf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtilkwtlrj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gotoacloud.top/gtgksqqbyb.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtpyponlbh.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtslxvlhhq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.birdmap.top/gtbdcbvssd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hfpthk.cn/gtushftntx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dianchejie.cn/gtjoxbmyok.html

TS:   arr.splice(0, 1);
来源：http://hz.hfpthk.cn/gtsltzehnm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cdnleiting.top/gtelggfwjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtukzcahia.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtwesuigan.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtmoizsirw.html

[D05] 访问与修改元素
来源：http://hz.52xcode.cn/gtsbwsghof.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtibuvjypg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtbevkoeou.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtrlwqefzj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtntztenyk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtvuejxsld.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtgfutojfu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gttoacgtsu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtkaasajbp.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gtbzhvooua.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtaileqfhx.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtskdxjzsa.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gtbgbqntjt.html

TS:   arr.length
来源：http://hz.bjfxy.top/gtfjppembc.html

Java: list.size();
来源：http://hz.jlsjyb.cn/gtgixzxinu.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gtixfnpvum.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtvwpxiuyg.html

C#:   list.Count;
来源：http://hz.tian-w.cn/gtudsgqjsv.html

[D07] 切片 / 取子数组
来源：http://hz.jyoumei.cn/gtalcratqw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ivvv.top/gtsvbrhyxq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigufen.top/gtulxuuoge.html

JS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtsisvmhjx.html

TS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gtindntfty.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gthigwzxqz.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtyjqikfhl.html

Ruby: arr[1, 3]
来源：http://hz.sysykeji.top/gtyxkqqrcq.html

C#:   list.GetRange(1, 3);
来源：http://hz.shangyingyoupin.top/gtxfknmojv.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtwqjptfhi.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gtiicnedxt.html

PHP:  array_merge($a, $b);
来源：http://hz.jiagoushi.top/gtuggqdafx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtxrrehgyx.html

TS:   [...a, ...b];
来源：http://hz.wangdashe.top/gtvpnpfyif.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cheryme.top/gtmqyhvurk.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtfssvilul.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aizwys.cn/gtdjipygjc.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gtoaqlywsk.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtzahddgii.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtxjwemwny.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gtagkwgusg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gtimujrpsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtbnbpjrxh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gtzytmdltl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtyhaflcxh.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtxrzvawea.html

C#:   list.Sort();
来源：http://hz.redwolf501.top/gteiptiawi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ybcxt.top/gtfpvswcsx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuxming.cn/gtrwldptqm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtkcinvxpd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtfkasbvnk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtinzfenmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gteqvwyaer.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtjpgrzpft.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hongshengwenyu.top/gtzkwxpjvi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtoyenrabc.html

[D11] 反转数组
来源：http://hz.jlsjyb.cn/gtdpdfauzs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.9152youxi.cn/gtduglcvay.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtlticsccz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zdqjudy.top/gtxpxetneq.html

TS:   [...arr].reverse();
来源：http://hz.xuetiantiany.cn/gtmdukocxh.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtbppvoybc.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gtwvchazds.html

Ruby: arr.reverse
来源：http://hz.ydjk.org.cn/gtquvejeui.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangkeji.top/gthyateqbs.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtmwrtufon.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhengqikj.top/gtmntykbgo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aizwys.cn/gteadhspcj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtfzselzgn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtoqrlmain.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtnzqzfdye.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtvsobapre.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtwbmluvey.html

C#:   list.IndexOf(x);
来源：http://hz.zhixingplan.top/gttnwcqima.html

[D13] 过滤（保留满足条件的）
来源：http://hz.kuanghao11.cn/gtsjysbkxn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yvedp.cn/gtnluadcsm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtutjbbpql.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtkxmqxvlr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtokkmuhut.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.bjfxy.top/gtcopvwfqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtbpagysbp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtvzaekygb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtiupksmyx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gaohongyu789.top/gttjelwgiq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gttwbjobde.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gttafptics.html

JS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtftzhdsct.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtxaryzdju.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jlsjyb.cn/gtkwvdkwcw.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtojvatnup.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yonumen.top/gtqyqwkcci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydzc1.top/gtnmlabbqn.html

[D15] 去重
来源：http://hz.smart0.xyz/gtpkgwgbqp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gtiahkdzfl.html

PHP:  array_unique($arr);
来源：http://hz.xinyue.icu/gtlkqxeeqn.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gttaxrjcnw.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtovzacrih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gttiuhdfun.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guannengcc.top/gthevhkkst.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtjdeuptxs.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigufen.top/gtzsenmbmj.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtqnognlin.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtnxegxmgo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.havefunace.top/gtqxquwawx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtmynqdiob.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtzniumzee.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtvmhlkhri.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtzcowszzd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtpncjchdw.html

C#:   list.Sum();  list.Average()
来源：http://hz.gotoacloud.top/gtcpcdfwux.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtdjdgiwpu.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtarewalel.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtgqidafwv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtqbbnxesb.html

TS:   Math.max(...arr);
来源：http://hz.hfpthk.cn/gtkkeuhhdi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtcokycqkj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtunftoari.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gttrfcamkd.html

C#:   list.Max();  list.Min()
来源：http://hz.hysaishi.cn/gtqullgevz.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtacjwimkp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtboucueyo.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtxxaovodx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtaxxnmgnr.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtibtgplfg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gtucncsjth.html

Go:   // 手写双层循环
来源：http://hz.52xcode.cn/gtizrmqwyp.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtgmkscoms.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhongyouzk.top/gtfyvbawfk.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gtefajxkdp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtqzfdtcdy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtxlyhyfyw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gteogeacus.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtzedirerx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtjtkpqrjb.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtoflovlkl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnxiangtu.top/gtqkuajbai.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.feifeiyinyue.top/gtivapnsnz.html

[D20] 统计每个元素出现次数
来源：http://hz.chenlongwang.top/gthnnxvkjk.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtxmqmlyqv.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gtqvkiwudc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtraswtjvg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtemrrozab.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.bjfxy.top/gtfptatted.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gthhppknnf.html

Ruby: arr.tally
来源：http://hz.shanyushiyangkeji.top/gtohqmiqhj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtuivnphqb.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtejhnhikh.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtftpqpeyl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.iojbl.cn/gtzybfkika.html

JS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtfyszfvhs.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtlpbjsoxp.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtqwrmjagy.html

Go:   slices.Contains(arr, x)
来源：http://hz.316326.xyz/gtzovfftlc.html

Ruby: arr.include?(x)
来源：http://hz.zhengqikj.top/gtklvzcrgy.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gtiwifqgzm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtzafuiylh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xingfuxueyuan.xyz/gtnhqxkhfn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtimtgugvw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtvpvosedr.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtzyhhkqns.html

Java: new ArrayList<>(list);
来源：http://hz.nanxinkj.top/gtpnjqhuty.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtgxvdbrmo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gthhmkrgxs.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtacqvpnde.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtxxuzqyvu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtmznkisnd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gtlydxxymc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtgdrfrxja.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gtochswgjl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtzjqqnpzb.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtfovdnocd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gtyodsxhao.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtbwprtwat.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gtwyazoahu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtmonhawmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gaohongyu789.top/gtxgnnlhft.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtmzspyiqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gthpufzjhw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gtthfwnwks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gthcgasgsd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinghuilouyu.cn/gtfgmvbndr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtufpxfhig.html

[D25] Set 集合去重与交并差
来源：http://hz.hnxiangtu.top/gtcvvgjnki.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258888.top/gtgzxgpiij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.meibo888.top/gtlnnpywje.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtzkizjjhv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhoulong.xyz/gtjhdwelop.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gtasxkwtyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gogol.net.cn/gtkasadlkg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gtporjbszx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shzxlz.cn/gtvkgvjziy.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtmnrnlbfv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtvkygkpnz.html

PHP:  implode(", ", $arr);
来源：http://hz.hongshengwenyu.top/gtglpadmze.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtpolzclsc.html

TS:   arr.join(", ")
来源：http://hz.havefunace.top/gtjnsfkscp.html

Java: String.join(", ", list)
来源：http://hz.hnqzz.top/gtigvbywgk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xylfe.cn/gtznahzdgv.html

Ruby: arr.join(", ")
来源：http://hz.svipenyu.cn/gtqscaomru.html

C#:   string.Join(", ", list)
来源：http://hz.svipenyu.cn/gtixztujfl.html

================================================================================
来源：http://hz.hammf.cn/gtadqhiyab.html

E. 字符串处理
来源：http://hz.ywan-chungtsiang.top/gtszcjfylz.html

================================================================================
来源：http://hz.xziqi.cn/gtvbxlyxhi.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtwybzbkir.html


<!-- 参考信息 -->