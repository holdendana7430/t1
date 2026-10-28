代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtnsdxednw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sxryk.cn/gtnhnqlghd.html

Java: import java.util.List;
来源：http://hz.hywenlv.cn/gtfvwjkbvv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhaomingkeji.xyz/gtqadzunss.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtqwpaishp.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtsettmabd.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtllrssoqy.html

Py:   (lambda: print("run"))()
来源：http://hz.dashuyun.cn/gtsweupbjv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhijiandao.cn/gtmiwgsetw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtqzyqqpvo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtuqbmrjwz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxinkj.top/gtfshyswve.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtnxkflysh.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtiqoztqkx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigfzy.top/gtbsdawdfv.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydjk.org.cn/gtmtcjutnt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigfzy.top/gtgmvpwivf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtecbdozhw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gthbpxvlyl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtnkkhigzq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtzdoafpwl.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtfuvbzvta.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtfotmvmic.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtclcaelev.html

[C14] 泛型函数
来源：http://hz.birdmap.top/gtxacudfml.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtcadaivzp.html

PHP:  // 无泛型
来源：http://hz.zycfv.cn/gtaclixgch.html

JS:   // 无泛型
来源：http://hz.yonumen.top/gtvhwnwguu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtpwnzrdix.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shangyingyoupin.top/gtludnicrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuanzhike.top/gthdcrbnjh.html

Ruby: # 无泛型
来源：http://hz.zhiwuduotai.top/gtwduvbocy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.quarkkingdee.top/gtunrionso.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtkgjwgtwi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydjk.org.cn/gtpuejhbrr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtuwnlblpu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gzhubu.top/gttlybwwkw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtntuiflmf.html

Java: // 无解构
来源：http://hz.cashguo.top/gtlqwunaop.html

Go:   // 无解构
来源：http://hz.0kj1m.cn/gtrnpgterx.html

Ruby: a, b = pair
来源：http://hz.andypj.xyz/gtdlrsnffd.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtcwlggwld.html

[C16] 函数 / 方法重载
来源：http://hz.mhx1999.top/gtabpubvcu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtiuqqlgfj.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtaptrpiss.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.svipenyu.cn/gtucugqrhe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shzxlz.cn/gthfqhyhpe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.redwolf501.top/gtijpbzgmr.html

Go:   // 无重载：用不同函数名
来源：http://hz.daria6918.cn/gtbvttnwcc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtvcqdqugo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ivvv.top/gtnseldvnj.html

================================================================================
来源：http://hz.guowangkeji.top/gthzvjfncc.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtljbxnbbm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbkxarmfn.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtbdbogfzc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtazcxjjfo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtbgadgtgy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jyoumei.cn/gtjjtvcgio.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gtasdkoydc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtiltdrgqg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtbikmnqoh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj202588.top/gtfdsajetv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ydjk.org.cn/gtycunliuc.html

[D02] 追加元素到末尾
来源：http://hz.gzhubu.top/gtqkjbchoc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtpobkudma.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.smart0.xyz/gtyeprgnsy.html

JS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gtxorsjqem.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gthxtohvod.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gttjhmrbdw.html

Go:   arr = append(arr, 4)
来源：http://hz.svipenyu.cn/gtgxcmbyvq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jlsjyb.cn/gtlmwcihdk.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtrrthense.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtqjjyachp.html

Py:   arr.insert(0, 0)
来源：http://hz.jinqigfzy.top/gtrtofsjof.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hysaishi.cn/gtgcyugyvt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hammf.cn/gtugaqyyvz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.kuanghao11.cn/gtbbbvcdqy.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtwffcceqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gtkxogpohu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gtkpswhnch.html

C#:   list.Insert(0, 0);
来源：http://hz.jinqigfzy.top/gtuzjbzjrd.html

[D04] 删除元素
来源：http://hz.gotoacloud.top/gtqyzhncts.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.svipenyu.cn/gtekuwshuk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtypftzsbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tianlin.xyz/gtdcnuxtvr.html

TS:   arr.splice(0, 1);
来源：http://hz.hysaishi.cn/gtnnddepwp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pycfn.com/gtlrpsmztz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuetiantiany.cn/gtgkickgnr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gtufzyvyim.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cashguo.top/gtmtsxkbra.html

[D05] 访问与修改元素
来源：http://hz.316326.xyz/gtifbhryaa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gteprtnkpg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtxkhcfzwl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtzldwyyln.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gtafupqtep.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gzhubu.top/gtapxnjmnr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtplnqpyyl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtudokzavz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ybcxt.top/gtvogwtadv.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gtjbrbkfui.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtqgcovsbr.html

PHP:  count($arr);
来源：http://hz.yongpay.top/gtucbkezqt.html

JS:   arr.length
来源：http://hz.gaohongyu789.top/gtnuktcdwl.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtbfvwrklg.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gthbdamyuu.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtelrgwrwt.html

Ruby: arr.length; arr.size
来源：http://hz.sweek.top/gtqmmxvhxh.html

C#:   list.Count;
来源：http://hz.gzhubu.top/gtmaeavxui.html

[D07] 切片 / 取子数组
来源：http://hz.mhx1999.top/gtnkrradut.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gtcsefugqf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj20258.top/gtnsoawfkc.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtkijaxwuy.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtgblbqgub.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtvepusjux.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtfednrpqh.html

Ruby: arr[1, 3]
来源：http://hz.chenjidiqi.icu/gtexxvzfac.html

C#:   list.GetRange(1, 3);
来源：http://hz.guannengcc.top/gtdakajewc.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtbdjahion.html

Py:   a + b;  a.extend(b)
来源：http://hz.9152youxi.cn/gtdblwajvg.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtrsnkircy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fzhhl.top/gtmzglwdae.html

TS:   [...a, ...b];
来源：http://hz.jinqigufen.top/gtxwflzwqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtsdexfpgj.html

Go:   append(a, b...)
来源：http://hz.yongpay.top/gtycmcyyid.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gtnuksgxea.html

C#:   a.Concat(b).ToList()
来源：http://hz.yvedp.cn/gtslqtbshk.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtixqflrfc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtcftvnttx.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtxrqpqjpa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtoulfnmhh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yvedp.cn/gtafbdunmx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gtiwxfrtny.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtodvuaupy.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtskowtgbz.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtzlcohzxp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtbqyhzxns.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtcuppqrnn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtajplosmw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zycfv.cn/gtbfwbbenj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtwscpkyjk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuanzx.com/gtpdkipldq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.snrcjt.cn/gtzebbvujp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gttryinrvg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gteiiseldt.html

[D11] 反转数组
来源：http://hz.wangshuangyany.cn/gtmiolfhjz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.meibo888.top/gtyorodqlf.html

PHP:  array_reverse($arr);
来源：http://hz.0kj1m.cn/gtixwhqkyn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtpdtrclsn.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtsqljlqlv.html

Java: Collections.reverse(list);
来源：http://hz.sufxvd.cn/gthdnqbdkp.html

Go:   slices.Reverse(arr)
来源：http://hz.ydjk.org.cn/gtjcyearsa.html

Ruby: arr.reverse
来源：http://hz.wangdashe.top/gtunawlmcm.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gttazniemc.html

[D12] 查找元素下标
来源：http://hz.smart0.xyz/gtgxkecbrl.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gthylyxfmo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.birdmap.top/gtfmudnsgf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtqifmidtn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cucudq.cn/gtaocuytfr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtomyxboec.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtotczlqhf.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtryoljklc.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtgpixgnus.html

[D13] 过滤（保留满足条件的）
来源：http://hz.havefunace.top/gtmlykkihh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gticczdtwm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtdvwgwiko.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtldofylsc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtjjttgtlw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhixingplan.top/gtcaellfva.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtibjdvbef.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gtwroygbps.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gaohongyu789.top/gtdzvhxqoj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pengpengdd.cyou/gtmgjpwych.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangshuangyany.cn/gtjghpdqpj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtwvfxmepz.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtcbrulahl.html

TS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtiozzysed.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtmzbzkmji.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtrohrrujq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtdkyyosnu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gtsktonzrd.html

[D15] 去重
来源：http://hz.zhoulong.xyz/gtdpyxwtlb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aizwys.cn/gtlgesvcur.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gtvxiudciz.html

JS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtwbuuhund.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtbtgmymes.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtdvtvrbpa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gthjgejgmk.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtqkilsail.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtovtonout.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gtkoeprdte.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtyshnqhhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dashuyun.cn/gtzazjozgt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtolimwrne.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtjvstnmii.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtleekkdup.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtjcukctlr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigfzy.top/gtncltvlqe.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtgqfxvgqr.html

[D17] 最大值与最小值
来源：http://hz.hongshengwenyu.top/gtiqeyyjce.html

Py:   max(arr);  min(arr)
来源：http://hz.tian-w.cn/gtayseaoqn.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtikruhgac.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cqqwz.cn/gtghpezitt.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtjwwaepqv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gzhubu.top/gtoaghhmco.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gtcyeydvdr.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gthufsyiom.html

C#:   list.Max();  list.Min()
来源：http://hz.feifeiyinyue.top/gtgjcolzfz.html

[D18] 扁平化嵌套数组
来源：http://hz.fengsongda.top/gtyyccyfla.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangdashe.top/gtxmgbeusk.html

PHP:  array_merge(...$nested);
来源：http://hz.xylfe.cn/gtasoyltuj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtjezkteyd.html

TS:   nested.flat();
来源：http://hz.andypj.xyz/gtxsmzclpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shuidangran.top/gtvakhjgry.html

Go:   // 手写双层循环
来源：http://hz.shuidangran.top/gtaawhikbg.html

Ruby: nested.flatten
来源：http://hz.nanxinkj.top/gtzrikyqgc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gteynsltno.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtigpewxbd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtcouzexzy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtsctzkrag.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtsaetolsq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtehlkakle.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.feifeiyinyue.top/gtydnexpfq.html

Go:   // 手写 map[string][]T
来源：http://hz.iojbl.cn/gtwgnfkoio.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jianghu66.top/gtkzdrbost.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenzaomai.com/gtmubyjnvw.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtuyixnzzw.html

Py:   Counter(arr)
来源：http://hz.sweek.top/gtydwhbxst.html

PHP:  array_count_values($arr);
来源：http://hz.jlsjyb.cn/gtooboeddc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtlorefvwk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtnkoxufjt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgfzy.top/gthqsyhzxm.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gthbnkzuws.html

Ruby: arr.tally
来源：http://hz.jinghuilouyu.cn/gtskjflksj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhixingplan.top/gtwftxhbuu.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtscgbkfvh.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtzhltfybc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtqswhuzpd.html

JS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtevziovjb.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtolydczdp.html

Java: list.contains(x)
来源：http://hz.vqdsnc.cn/gteuxpvjhx.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtimxbonkt.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtiddrjmoj.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gtztfgyota.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pengpengdd.cyou/gtreddpzbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tanke756.top/gtytdnccez.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guowangkeji.top/gtwfjtmvzf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.vqdsnc.cn/gtmqmdyfmt.html

TS:   [...arr];
来源：http://hz.yj20258.top/gtwbbgkvqy.html

Java: new ArrayList<>(list);
来源：http://hz.hammf.cn/gtcdbdlvay.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtlzryaeyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtmssoplff.html

C#:   new List<int>(list);
来源：http://hz.gogol.net.cn/gtwuqraryv.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtvxidnyls.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtegonjnhg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtgzpjgska.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtnirrwodb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yanxiufei.cn/gtiskxfykd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daria6918.cn/gtxenylkps.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtwdivhfwv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtaedvcllh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhongyouzk.top/gtakywaprf.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtzftditmy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtcndzkila.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtgcvfyqvs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtbrboylkl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtrrpcbhpu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtsjctflkl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yanxiufei.cn/gtkgwqilfn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gttfsyltej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtytcaphvd.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gtwykzjsnl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gtjzzwezoe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hywenlv.cn/gthyzzhzsf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sxryk.cn/gtwjuyxlzt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtalbzpweb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhongyouzk.top/gtyavetgae.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gtwshiepti.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtjijifimw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtobhjmdlu.html

[D26] 数组转字符串
来源：http://hz.zhijiandao.cn/gtrhrmudtw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuetiantiany.cn/gtdhvhlgbj.html

PHP:  implode(", ", $arr);
来源：http://hz.meibo888.top/gtqxnyqknh.html

JS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtidbjhgmj.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtmgmpbzyl.html

Java: String.join(", ", list)
来源：http://hz.0kj1m.cn/gtuqihmhoc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtgoqbnuuk.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtejppjqvl.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtrpxrurup.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgfadusan.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtkwpgbpjd.html

================================================================================
来源：http://hz.zhixingplan.top/gtqlarfjmo.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtzhhdrnzc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuanzx.com/gtzaexhdzs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gtoeqnpqsd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtgnhzndbd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtpvismyxu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtiaqstmrz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangdashe.top/gteqrwbbeq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtwnsmbymz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ehwqpu.com/gtjqvwxpiz.html


<!-- 参考信息 -->