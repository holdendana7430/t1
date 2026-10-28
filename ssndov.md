代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gtykuulpns.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shuidangran.top/gtbvgpgfjh.html

Java: import java.util.List;
来源：http://hz.zdqjudy.top/gtcewefink.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gtlhbmxcmq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xylfe.cn/gtdrbgxleg.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtzqhjtmcb.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydjk.org.cn/gteyjabzgp.html

Py:   (lambda: print("run"))()
来源：http://hz.cheryme.top/gtvvougzte.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhijiandao.cn/gtiwnijywt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtpgrbhhxs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtbvsamfmc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtlondwbkg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangdashe.top/gtvxdaxdfo.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gttmokkpcq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.haohaochexian.top/gtdudckatz.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangshuangyany.cn/gtjqwhkjnu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ivvv.top/gtasbxleia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtikfdjipe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuetiantiany.cn/gtcpcpuhtc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtgluxpxtq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtahuetgeu.html

Go:   func add(a, b int) int
来源：http://hz.tanke756.top/gtndsrfhoy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtuhmkjmeb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtvmlmirey.html

[C14] 泛型函数
来源：http://hz.xingfuxueyuan.xyz/gtnxneotjy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtcrcxbyic.html

PHP:  // 无泛型
来源：http://hz.jyoumei.cn/gtujznvaix.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtkpejcxij.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yongpay.top/gttssiyvac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtkvhpmbxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fzhhl.top/gtokgbtoma.html

Ruby: # 无泛型
来源：http://hz.hnxiangtu.top/gtdfxewnzw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gtyactpxxa.html

[C15] 解构 / 展开参数
来源：http://hz.sysykeji.top/gtxugurvdw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtsdtlmxkh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.birdmap.top/gtvsdscujv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtwfojwwpq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtuiccgpzv.html

Java: // 无解构
来源：http://hz.chenzaomai.com/gtejvhaprz.html

Go:   // 无解构
来源：http://hz.hongshengwenyu.top/gtajcdojlw.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtwxyguqch.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtsgsetxkg.html

[C16] 函数 / 方法重载
来源：http://hz.yangfankeji.com/gtjfvcphfw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtfdrjpxxy.html

PHP:  // 无重载
来源：http://hz.yongpay.top/gtherystaz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258.top/gtmcjlglqe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnqzz.top/gtiuzqcdib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shuidangran.top/gtbvoaqbvm.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhaomingkeji.xyz/gtrdogcwzh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtgmbjuukk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yanxiufei.cn/gtsjaailjo.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnzitjwaj.html

D. 数组 / 列表 / 集合
来源：http://hz.cdnleiting.top/gtwjqxjvym.html

================================================================================
来源：http://hz.hfpthk.cn/gttaihrxee.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gttwburwbf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtwfyepkqs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.kuanghao11.cn/gtxdfilprt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cashguo.top/gtvqoatzhz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.meibo888.top/gtdxesgmvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtvpsrkxtq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cdnleiting.top/gtelaemhpq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtqztofckf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xylfe.cn/gtaftqcrzz.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtdslmbjhx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuanzhike.top/gttwvaoqng.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.c1oappe.top/gtkmzbtgkc.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtksufvbty.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtuihiqjzq.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtkulamdon.html

Go:   arr = append(arr, 4)
来源：http://hz.xylfe.cn/gtvxblruhx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gtejrcpiqo.html

C#:   list.Add(4);
来源：http://hz.feifeiyinyue.top/gtpymbnhlb.html

[D03] 在指定位置插入元素
来源：http://hz.ydzc1.top/gtiibxevaw.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtqgcnryse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuanzhike.top/gtahdxrhsx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtglmebkot.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nwbrower.top/gtntdeltbh.html

Java: list.add(0, 0);
来源：http://hz.sxryk.cn/gtwfsekflu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sysykeji.top/gtfobtoico.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guowangkeji.top/gtdncuoifj.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtfgsmgcgl.html

[D04] 删除元素
来源：http://hz.haohaochexian.top/gtfdxqikpr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tanke756.top/gtgqdwxltw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.316326.xyz/gtpjeepvxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtrziqhyqx.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gtobdfpppy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gteuayilpo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtsyycscxi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.svipenyu.cn/gtwtlbohpo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.guannengcc.top/gtzipxnsra.html

[D05] 访问与修改元素
来源：http://hz.yangfankeji.com/gtmcuykjgs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtgiuhbica.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gthzozgzqu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtfxtelecv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gzhubu.top/gttdoggwej.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhaomingkeji.xyz/gtgneavxvj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.birdmap.top/gtnkfngziu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtbvbtnaci.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhiwuduotai.top/gtsugjurir.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtsuambqjc.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtftzpdfon.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtuqpaedmj.html

JS:   arr.length
来源：http://hz.jlsjyb.cn/gtqcsztzuv.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtpnhqzcrk.html

Java: list.size();
来源：http://hz.snrcjt.cn/gtczyjphbl.html

Go:   len(arr)
来源：http://hz.tian-w.cn/gtfuhtogtr.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gthtilokru.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtiffkhhvh.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtajxoaxyo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtitflgxrm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtvutntomg.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtvvncjths.html

TS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtglbhgghb.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtmpbiuldn.html

Go:   arr[1:4]
来源：http://hz.tianlin.xyz/gticxwbjxw.html

Ruby: arr[1, 3]
来源：http://hz.havefunace.top/gtswbinmpt.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtzvikkjuw.html

[D08] 合并两个数组
来源：http://hz.dianchejie.cn/gtuogtfbya.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtzvskaacx.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtgpaftede.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtjvzlfrsv.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtosfhkoge.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtfuwxjxpk.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtjgsfnijz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtkbymlpgh.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtvtlttmmb.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtiiidslrj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gttstdxmdq.html

PHP:  sort($arr);
来源：http://hz.gzhubu.top/gtnxofzfwh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gtmxgdybws.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtqequmqut.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtnbdacpjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtakvgajor.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtimlolsoa.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtuikiyzwq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gtpakmrdyc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtmjxwzxkf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gtfgzaxfng.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtnsgsbmwh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gtnovriaut.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtjiqtzxtk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenjidiqi.icu/gtyqrhairo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gthueobvmk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtharbvmid.html

[D11] 反转数组
来源：http://hz.zhixingplan.top/gtdyhyesgh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.316326.xyz/gtktzxjwcg.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gtevugjivu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtglbbqjhk.html

TS:   [...arr].reverse();
来源：http://hz.yonumen.top/gturoihixj.html

Java: Collections.reverse(list);
来源：http://hz.xingfuxueyuan.xyz/gtqcuoizrc.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gthmsrdnsj.html

Ruby: arr.reverse
来源：http://hz.jinghuilouyu.cn/gtaluavhdm.html

C#:   list.Reverse();
来源：http://hz.zhiwuduotai.top/gtdarofmly.html

[D12] 查找元素下标
来源：http://hz.andypj.xyz/gtckshwhvx.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhengqikj.top/gtwsqwxpxu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hysaishi.cn/gttmgsayjd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtiufcoaud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtblqkrdmr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.svipenyu.cn/gtszsrknrw.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtxgatbkga.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gtetglpqlf.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gtfnrjfxwo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtabfbnhwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daria6918.cn/gtfhxrdhqb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.redwolf501.top/gtvhjvtzha.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtxzsraobt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtmlidhett.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gtyalbixdt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtalapmupt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtzljplkkp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nwbrower.top/gtceqrrhkm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtnutoceba.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtwrzvwhnn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gtwznlfnqp.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtffajtzuw.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtdpnjsjsh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtjfdibbsf.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtjfnhfblc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtzmhwepsx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cucudq.cn/gtzgvvleng.html

[D15] 去重
来源：http://hz.52xcode.cn/gtkungfuhh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtavrdlopo.html

PHP:  array_unique($arr);
来源：http://hz.yangfankeji.com/gthsmvziyy.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtxzcutybl.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtdgraxrzj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gteslbfggy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gtesealbhq.html

Ruby: arr.uniq
来源：http://hz.iojbl.cn/gtzdzjgrue.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gttxwceszq.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtefqtrklp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gttzirhlcs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtarxtzofs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gtduswpgbi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtlksdwkgb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtigbxivgq.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtoojbetch.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gtoaxldeof.html

C#:   list.Sum();  list.Average()
来源：http://hz.pengpengdd.cyou/gtwrlidrxo.html

[D17] 最大值与最小值
来源：http://hz.mhx1999.top/gthqzpstol.html

Py:   max(arr);  min(arr)
来源：http://hz.sxryk.cn/gtvmnucolv.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhijiandao.cn/gtrpbmmihf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtjmozyixn.html

TS:   Math.max(...arr);
来源：http://hz.0kj1m.cn/gtzyutrweg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtfzdpmysh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtqmljxhhr.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtrmqqiywe.html

C#:   list.Max();  list.Min()
来源：http://hz.feifeiyinyue.top/gtbzgenjlu.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtyvjiogpj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtuuaajltn.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtmxiybrnq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtnmfwtufj.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtngnqldfo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgfzy.top/gtdemtomrb.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gtqkbkyyas.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtfqbyfmes.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuxming.cn/gtcrmxyhfo.html

[D19] 按字段分组
来源：http://hz.316326.xyz/gtolqrmgvv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtuuhqrszo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtzunpbpgh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dianchejie.cn/gtbzodktue.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtgzanmauu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigufen.top/gtsrdrahed.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtrwlcqbxj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258888.top/gtmjlndylv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigfzy.top/gtrcpcnuci.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gtrbvnjois.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtmgmslvhf.html

PHP:  array_count_values($arr);
来源：http://hz.jianghu66.top/gtcywfrizm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gthoxsextg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtxhtlqwse.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtzinwwowe.html

Go:   // 手写 map[T]int
来源：http://hz.gaohongyu789.top/gtkebjkpft.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtfhxkksif.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hywenlv.cn/gtcviepqyy.html

[D21] 判断是否包含某元素
来源：http://hz.hysaishi.cn/gtdsungjsv.html

Py:   x in arr
来源：http://hz.ivvv.top/gtisprhmbk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.birdmap.top/gtbsufuzhi.html

JS:   arr.includes(x)
来源：http://hz.ivvv.top/gtrmdoeafh.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtwqicthvj.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtigxqyudx.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtvirzmoqb.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtmtzyqcja.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtkurqrtox.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cashguo.top/gtihfrgwnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gtozhvxecf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gtxnbrzxdu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydjk.org.cn/gtrqqythny.html

TS:   [...arr];
来源：http://hz.yj20258888.top/gttwnnqsok.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtngrmhaff.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtbconpjey.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtvhtlucfm.html

C#:   new List<int>(list);
来源：http://hz.yonumen.top/gtyfvtxoti.html

[D23] reduce 累积计算
来源：http://hz.smart0.xyz/gthabrsawm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtercqiqcj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtjcfypvki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtmapyvzbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aibaodan.cn/gtiusifdfk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtanhqetts.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtlkrszqsm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hywenlv.cn/gtgmffcxob.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hfpthk.cn/gtugvlhwmr.html

[D24] 字典 / Map 基本操作
来源：http://hz.cdnleiting.top/gtfituvnjy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtcpuokbyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtbnskbtmb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtjfpaaemd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtivyvamln.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gtrjzacmex.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xylfe.cn/gtrhtrealt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtyamvtetm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtfahhferh.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangkeji.top/gtcgkmugmn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtglylywcf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yongpay.top/gtqfvhmwua.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtrdjsahwl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gttkehgmhe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.bjfxy.top/gttsokncye.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gtxhbdviqa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtwazxuxuq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtuzprauga.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtrmndamun.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxuanxn.top/gtinctldyc.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtwzykkixt.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtxmbmilbz.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtaatixuoc.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtlesrfxng.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ivvv.top/gtpxukgzov.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtjsnforgr.html

C#:   string.Join(", ", list)
来源：http://hz.52xcode.cn/gtjfuuzmkm.html

================================================================================
来源：http://hz.hfpthk.cn/gtqdysaihh.html

E. 字符串处理
来源：http://hz.xylfe.cn/gtjnowvghd.html

================================================================================
来源：http://hz.iojbl.cn/gteciivkic.html

[E01] 拼接字符串
来源：http://hz.birdmap.top/gteluklnjq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guannengcc.top/gttigvbucb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.smart0.xyz/gttevhutjw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtgsfzgwfy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtdbpewtih.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gotoacloud.top/gtrsbjujou.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yueranfly.top/gtekqddysm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtjbmqzmnn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtivlrtjtv.html


<!-- 参考信息 -->