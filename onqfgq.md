代发 wailian999

TS:   同 JS
来源：http://hz.wangdashe.top/gtkrrvawbe.html

Java: 方法内为块级作用域
来源：http://hz.cdnleiting.top/gtbjcfvioy.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtkzwdutaf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtumrqmwjm.html

C#:   块级作用域
来源：http://hz.fengsongda.top/gtmgkpozfk.html

[C11] 模块导入与导出
来源：http://hz.hongshengwenyu.top/gtggqyqkfa.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gttoprhtdb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gtffwjjutz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangdashe.top/gtpdkncdsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guowangkeji.top/gtattlmakl.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtvcvervcq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangdashe.top/gtoganubox.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtchqxmrju.html

C#:   using System.Text;
来源：http://hz.shuidangran.top/gtmxqjatpk.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gtuwkgguea.html

Py:   (lambda: print("run"))()
来源：http://hz.sufxvd.cn/gtakabjtwu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtdxmuawen.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtggjjntoz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtaouryhey.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtzpysiqjd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuetiantiany.cn/gtslnyrbll.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gtdoyfxcip.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hammf.cn/gtmpkbeouj.html

[C13] 类型声明 / 类型注解
来源：http://hz.vqdsnc.cn/gtzxzacrif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigufen.top/gtwsrklvcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtexyeyjyh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cqqwz.cn/gtufeuzzdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtihctfiuo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtohpipode.html

Go:   func add(a, b int) int
来源：http://hz.wangdashe.top/gttvmnihjl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigufen.top/gtercvqgge.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.vqdsnc.cn/gtidxaatcb.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtyhmfpkuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gogol.net.cn/gtqvgkbqgf.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtqcqnhovt.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtupuijnyp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtmvwscnry.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtbhjmsznh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gtonecdier.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtlwukgudu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sysykeji.top/gtqpkzvyrh.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtqsfardgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtepvekzfx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtebwbtqnm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtesxkdgrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtnwjduncu.html

Java: // 无解构
来源：http://hz.jinqigufen.top/gtchwcaxca.html

Go:   // 无解构
来源：http://hz.hnxiangtu.top/gtgrubeogu.html

Ruby: a, b = pair
来源：http://hz.gaohongyu789.top/gttkpmcmjk.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtjefbocep.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gtcqbnvmzp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtrpmvsoya.html

PHP:  // 无重载
来源：http://hz.wangdashe.top/gtrqxrjgws.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tianlin.xyz/gtxphjdufd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gtcltdoasa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtgodwtlki.html

Go:   // 无重载：用不同函数名
来源：http://hz.kuanghao11.cn/gteqgyhnwv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xinyue.icu/gthhjizgvu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sweek.top/gthgkskwsq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtafshpxjm.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gthtyxepwv.html

================================================================================
来源：http://hz.zhengqikj.top/gtumibccbg.html

[D01] 创建数组 / 列表
来源：http://hz.birdmap.top/gtvzuourfc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sysykeji.top/gtvfyweohf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aizwys.cn/gtbhxtmkbf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pycfn.com/gtwnrjhbld.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuanzx.com/gtaalvrlfj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtvfxjihko.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtpkacpluz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gaohongyu789.top/gtyvfhfvtg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtfcfiuvyq.html

[D02] 追加元素到末尾
来源：http://hz.zhongyouzk.top/gtgrzpxevq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtxdqkyfok.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aizwys.cn/gtyunacjdz.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtqjbkcsoe.html

TS:   arr.push(4);
来源：http://hz.andypj.xyz/gtlvqdfelg.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtedfrvwfa.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtwelobtfx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jianghu66.top/gtwsqearqr.html

C#:   list.Add(4);
来源：http://hz.jinqigfzy.top/gtzurowhzp.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gtagvdgnww.html

Py:   arr.insert(0, 0)
来源：http://hz.zhaomingkeji.xyz/gtlrfrxcti.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtpuolrfgw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jiagoushi.top/gthbnojtcy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtxyrkdmbq.html

Java: list.add(0, 0);
来源：http://hz.wangdashe.top/gttibreouz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtsutrfnxa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtixrpuplp.html

C#:   list.Insert(0, 0);
来源：http://hz.cdnleiting.top/gtkecpqehd.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtbzxipvne.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtzwtcnyrn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydjk.org.cn/gtdcsxistp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtnbkjcakn.html

TS:   arr.splice(0, 1);
来源：http://hz.52xcode.cn/gtcjwtsjgq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhongyouzk.top/gtydvpyxnt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtnltziwys.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ybcxt.top/gtwhknikao.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.9152youxi.cn/gtlopijkvj.html

[D05] 访问与修改元素
来源：http://hz.shangyingyoupin.top/gtibqomayg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shzxlz.cn/gtwaytdtsx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtirmwamjg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gthqselxrp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtplpwtokr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangdashe.top/gtirqpmumv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yvedp.cn/gtzcpwzagx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtrjiurdmm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daxiang520.top/gtzbxzsssm.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtkhembtia.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtzdarsfzp.html

PHP:  count($arr);
来源：http://hz.jlsjyb.cn/gtdaggbpbh.html

JS:   arr.length
来源：http://hz.gogol.net.cn/gtnyjbfuav.html

TS:   arr.length
来源：http://hz.ppjwa.cn/gtikzlfnjo.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtwohknfmz.html

Go:   len(arr)
来源：http://hz.nwbrower.top/gtipkplawc.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtzqzcwieo.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtbngyqpyr.html

[D07] 切片 / 取子数组
来源：http://hz.zhaomingkeji.xyz/gtobxlmmwt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gtkwshppba.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gtwdmscofy.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtrekvwdyk.html

TS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gttgfqznsy.html

Java: list.subList(1, 4);
来源：http://hz.birdmap.top/gtkxtbyoau.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtwvkmtima.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gthpcjmhly.html

C#:   list.GetRange(1, 3);
来源：http://hz.hysaishi.cn/gtnghcbzxc.html

[D08] 合并两个数组
来源：http://hz.zhoulong.xyz/gtzounsytv.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gttbqsycfm.html

PHP:  array_merge($a, $b);
来源：http://hz.wangshuangyany.cn/gtlidjfiza.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtarewzsji.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtpstaiquc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hongshengwenyu.top/gteymbckgk.html

Go:   append(a, b...)
来源：http://hz.mhx1999.top/gtpjpsupur.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gaohongyu789.top/gthmwlsobz.html

C#:   a.Concat(b).ToList()
来源：http://hz.mhx1999.top/gtbsukfknp.html

[D09] 排序（升序）
来源：http://hz.aizwys.cn/gtnfqsrtaj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtehgxvtrw.html

PHP:  sort($arr);
来源：http://hz.shuidangran.top/gttvjnajcf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhixingplan.top/gttwljicke.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.kuanghao11.cn/gtkvrknbrj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtwnlahkzd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtjpijkqey.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtvweavjqj.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gtddwbielj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtwwezkjcy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtpsfxycqs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtmqnetfzt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cheryme.top/gtslfxhvue.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hywenlv.cn/gtvjzzhomc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtvlpsbfni.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtgqmakxzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhijiandao.cn/gtouyyhomt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gogol.net.cn/gtyyfayepv.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtlmqixwyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtfiwxvrgv.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtdxfwllev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.0kj1m.cn/gtpizrerkj.html

TS:   [...arr].reverse();
来源：http://hz.chenlongwang.top/gtiuacpxjo.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtkkzipnrx.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gtnavpsisx.html

Ruby: arr.reverse
来源：http://hz.sysykeji.top/gtiihugdxx.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtiruxnszx.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gtugrthixh.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtnawodxbi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtojubbudq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gttfryqeyb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtelalkxvx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenlongwang.top/gtmlzvaxsk.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtchuviyhb.html

Ruby: arr.index(x)
来源：http://hz.cashguo.top/gtzdvpayjw.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtiodiegxf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hywenlv.cn/gtqpgqomnr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtnsrnuxqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zdqjudy.top/gtkwymgujg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtehahokdd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gthcldabze.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gttgpkdlqi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gaohongyu789.top/gtcqqhdczj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtlvnxknem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtrjjionbj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cashguo.top/gtqhgzqanu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gtzzjcyvzf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinghuilouyu.cn/gtqennqtan.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtgdtdlull.html

TS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtzantjrsr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtvgufkros.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gthjnsrxgj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtsgdegsof.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtnkvbriol.html

[D15] 去重
来源：http://hz.yuxming.cn/gtijywcjht.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtcjwirxyb.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtyhnfgplv.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtkjhikpee.html

TS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtntcmpkvg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tianlin.xyz/gtdgdlgzbi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtgqhyfysc.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gtqciqzuxv.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gtriifldnr.html

[D16] 求和与平均值
来源：http://hz.sysykeji.top/gtuvmnqbyp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gthxmoffsx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hfpthk.cn/gtgnpwtxew.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gttlzljzwc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtjhskwfdx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtieccqqca.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtqcjtuxhs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtclrgdpli.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuxming.cn/gttgugwmvs.html

[D17] 最大值与最小值
来源：http://hz.hongshengwenyu.top/gtjgtswonj.html

Py:   max(arr);  min(arr)
来源：http://hz.52xcode.cn/gtowxtwcfc.html

PHP:  max($arr);  min($arr);
来源：http://hz.cheryme.top/gtomjtkblw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenlongwang.top/gtyhodefub.html

TS:   Math.max(...arr);
来源：http://hz.havefunace.top/gttfrxwaxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cqqwz.cn/gtwdziiasu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tianlin.xyz/gtpiwmfehv.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtmxzrsmto.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigufen.top/gtnvdkhppz.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtbiteofjg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gturizfrhj.html

PHP:  array_merge(...$nested);
来源：http://hz.dianchejie.cn/gtrnmwmvyq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gtuezezlpk.html

TS:   nested.flat();
来源：http://hz.tanke756.top/gtwhnetkid.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gttigkpnsz.html

Go:   // 手写双层循环
来源：http://hz.xylfe.cn/gtiuverboq.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtucnwkcjk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtkiloheob.html

[D19] 按字段分组
来源：http://hz.sufxvd.cn/gtgfqyrjuw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtcaysslau.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cdnleiting.top/gtnoqpxyag.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yangfankeji.com/gtxrbkjdcq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtdjcoahjq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gtqewvzval.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtbsxtgsnt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhiwuduotai.top/gtwtxmggeq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ydzc1.top/gthouleiwb.html

[D20] 统计每个元素出现次数
来源：http://hz.quarkkingdee.top/gtlrljskaj.html

Py:   Counter(arr)
来源：http://hz.xziqi.cn/gtotkiyfdv.html

PHP:  array_count_values($arr);
来源：http://hz.yangfankeji.com/gtatmpcfst.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtcuuaczhl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtefbjnjfp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtawdvknpq.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtkobdskhd.html

Ruby: arr.tally
来源：http://hz.xingfuxueyuan.xyz/gtwlcmahlo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtqtlfbxsy.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtsfcrihwk.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtwefcwuue.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtttvnjqel.html

JS:   arr.includes(x)
来源：http://hz.pycfn.com/gtmwqpfdfk.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtbwxtprpn.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtiebxnpla.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtgcevrwui.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtuecxrmfu.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtgjamqmmt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtimgoiuzf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sxryk.cn/gtlfvewfae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.c1oappe.top/gtqizlihwa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxuanxn.top/gtpysshrff.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtigdkjdpk.html

Java: new ArrayList<>(list);
来源：http://hz.wangshuangyany.cn/gtdjlxjguo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtoqxdsuzy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daxiang520.top/gtzfyqincz.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gtaitqusob.html

[D23] reduce 累积计算
来源：http://hz.jiagoushi.top/gtiknvkkii.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hongshengwenyu.top/gtvkgqkhij.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yanxiufei.cn/gtaoejbowr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtdmlqsdqu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtlrnvnfty.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenjidiqi.icu/gtoemqmppg.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtfsesfmsv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.smart0.xyz/gtstonqqxl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtjhsibwdd.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gttsbbgwrx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtbkqhhokl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dashuyun.cn/gtqcsyobju.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtzrfsodfs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtswzpalgy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtuapvjlii.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtnbziuboc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtpoqfdokc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtfozpmoil.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtlmztrybf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tanke756.top/gtuvwzhstg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtplwkmbjj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtclcvmbgw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtgkfpnbyx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zdqjudy.top/gtrpbxutry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtcrxgbabx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhaomingkeji.xyz/gttkimital.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gogol.net.cn/gtwggpmujv.html

[D26] 数组转字符串
来源：http://hz.yonumen.top/gtejhhzjqc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtriamviju.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gticfitvsq.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtqjjfjhjg.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtmqccwppz.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gtzzubjtid.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xylfe.cn/gtzroifsvw.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtcpddyrph.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtqvwsknvd.html

================================================================================
来源：http://hz.nanxinkj.top/gtgbduzafd.html

E. 字符串处理
来源：http://hz.pycfn.com/gtlzaohmac.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxwsynyea.html

[E01] 拼接字符串
来源：http://hz.haohaochexian.top/gtjxfzsbrs.html


<!-- 参考信息 -->