代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj202588.top/gtyglrgqlb.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtbjdiktzy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.dianchejie.cn/gtaihggsct.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtrbhpmdoz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gotoacloud.top/gtzeiitcqw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gaohongyu789.top/gtfniakold.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtrwxbzsxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtvpimcjeh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtsmwanxwu.html

Go:   func add(a, b int) int
来源：http://hz.mhx1999.top/gtdwxmbtqs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangkeji.top/gtvshnthsh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtfahuuruu.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtfqwacbzd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cdnleiting.top/gttjiwzmnd.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtysymjego.html

JS:   // 无泛型
来源：http://hz.iojbl.cn/gtrqqubibi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sweek.top/gtwtjbqorl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ppjwa.cn/gtohucorqv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtycksimdw.html

Ruby: # 无泛型
来源：http://hz.c1oappe.top/gtufgzsffs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gttdegogcg.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gtxswlnwha.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtimmaotjf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtokxgsmnz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.mhx1999.top/gtbybjjfej.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtoqwhzppd.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtyelegoqr.html

Go:   // 无解构
来源：http://hz.nanxinkj.top/gttawkpvja.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtwjsnibcl.html

C#:   var (a, b) = pair;
来源：http://hz.xziqi.cn/gtncqoonna.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtezapxlfi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgfzy.top/gtsrytjtmo.html

PHP:  // 无重载
来源：http://hz.ivvv.top/gtcmejraed.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtanpyzwet.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtjnelhnvi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aizwys.cn/gtruznflpo.html

Go:   // 无重载：用不同函数名
来源：http://hz.tianlin.xyz/gtitrvsrmy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuanzx.com/gtjpthmfss.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtxpvhwhzy.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnvdinyfo.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtrthewkwp.html

================================================================================
来源：http://hz.snrcjt.cn/gtdnpayqvg.html

[D01] 创建数组 / 列表
来源：http://hz.cheryme.top/gtpzwxintq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhixingplan.top/gtinxgqtkd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shangyingyoupin.top/gtcvqxbklk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhongyouzk.top/gtupywxudg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gtucmjpbqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtkjdnapac.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gtvfiurmjd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtujxvebjs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenlongwang.top/gtripbowfz.html

[D02] 追加元素到末尾
来源：http://hz.52xcode.cn/gtmbhckrpm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj202588.top/gthgsgrdsw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.feifeiyinyue.top/gtujloehtg.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtmyhprzeh.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtrvpfgrkn.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gtdhjsynox.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtzqapuozs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj20258.top/gtkmdpznku.html

C#:   list.Add(4);
来源：http://hz.ivvv.top/gtduvyyvhp.html

[D03] 在指定位置插入元素
来源：http://hz.sysykeji.top/gttgobilig.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtzfhycawc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhijiandao.cn/gtbmfkyqog.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtdgpgomwp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.redwolf501.top/gtlbivtpzc.html

Java: list.add(0, 0);
来源：http://hz.yuxming.cn/gttoethirz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.meibo888.top/gtnrjbbpou.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtvjieluee.html

C#:   list.Insert(0, 0);
来源：http://hz.cucudq.cn/gtrjyoygmw.html

[D04] 删除元素
来源：http://hz.zhengqikj.top/gtninepyzt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dashuyun.cn/gtqhmqnbkf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtstnvosfl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtpzjtrjty.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gtiovazyjx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cucudq.cn/gtilrlflat.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gotoacloud.top/gtdidkyxmt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.iojbl.cn/gteyaoxwlm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gtsmrkdqud.html

[D05] 访问与修改元素
来源：http://hz.aibaodan.cn/gtshbipzit.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtrlpwosdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tianlin.xyz/gtondfhphz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fengsongda.top/gtohkzogif.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gtjniezfba.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shangyingyoupin.top/gtbnxorhne.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.birdmap.top/gtrjljuemp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtuqpyuelk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtwomrzfpq.html

[D06] 数组长度
来源：http://hz.daria6918.cn/gtyrvhsfdz.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtnwfqfhjs.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtetxeqhgc.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gtwxtskcbq.html

TS:   arr.length
来源：http://hz.cheryme.top/gtsyucrkcj.html

Java: list.size();
来源：http://hz.gzhubu.top/gtfnbqgzhp.html

Go:   len(arr)
来源：http://hz.hnxiangtu.top/gtnddirhfv.html

Ruby: arr.length; arr.size
来源：http://hz.chenjidiqi.icu/gtrhtvpuct.html

C#:   list.Count;
来源：http://hz.gaohongyu789.top/gtvfblumft.html

[D07] 切片 / 取子数组
来源：http://hz.nanxinkj.top/gtscigeeir.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj202588.top/gtehoedjjm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ybcxt.top/gtkiwqmqnv.html

JS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtewqxbyck.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtmfrxvspq.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtgshjazgc.html

Go:   arr[1:4]
来源：http://hz.shuidangran.top/gtortgubqt.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtrvdkrwkm.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtpyoazinw.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtyanckqen.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhoulong.xyz/gtmbmwlkdi.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtaggysosx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenlongwang.top/gttyygxils.html

TS:   [...a, ...b];
来源：http://hz.shuidangran.top/gtpthyzmzg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gthpgqaaiu.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtepctglrr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jyoumei.cn/gtgqmvmczg.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtcptdhrqa.html

[D09] 排序（升序）
来源：http://hz.mhx1999.top/gtgyaadqrv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtiwqdusdv.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtfpworsas.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangshuangyany.cn/gtawxfbjlp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ehwqpu.com/gtvkljtbsl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gtsqgwyust.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtefpmxyjl.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtvcyhxrov.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gthycffywf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhixingplan.top/gttyikyimo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtkzeotlea.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangshuangyany.cn/gtzosiaoat.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtstrwalcz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgfzy.top/gtvhpgkfmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtzjezwpck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.meibo888.top/gtnnmqnlov.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.redwolf501.top/gtxrcznnlf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtnozqwjqc.html

[D11] 反转数组
来源：http://hz.sweek.top/gtsaudnsda.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gtttydzite.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtfizbwrje.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtkuogrkyl.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gtvqmqamlk.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gtqldujoro.html

Go:   slices.Reverse(arr)
来源：http://hz.daria6918.cn/gtfobqvtqm.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtgdnpoluj.html

C#:   list.Reverse();
来源：http://hz.xinyue.icu/gtkvwxcmek.html

[D12] 查找元素下标
来源：http://hz.zhoulong.xyz/gtqulkuzrm.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gthzpzfllo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xylfe.cn/gtupoqcqyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtceprrmys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtmujfmjnq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fengsongda.top/gtrqkdpzqi.html

Go:   slices.Index(arr, x)
来源：http://hz.fzhhl.top/gtxbexwbjm.html

Ruby: arr.index(x)
来源：http://hz.xylfe.cn/gtmmreagqv.html

C#:   list.IndexOf(x);
来源：http://hz.xinyue.icu/gtoqcalxky.html

[D13] 过滤（保留满足条件的）
来源：http://hz.c1oappe.top/gtvguiasaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hammf.cn/gtrlrfkpcc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtkrbvxkce.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtndmvcubh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtqftaesfz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhiwuduotai.top/gtjsbldxpx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jyoumei.cn/gtttcidcyp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtbsjwwmaj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shuidangran.top/gtiottqbjl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cdnleiting.top/gtklqmdpox.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtruennstq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtwvhhfxan.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtsptfjdcu.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtgarnrmoj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtnymqapea.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtmltruvnh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgfzy.top/gtkklfdvzk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sysykeji.top/gtfiussptm.html

[D15] 去重
来源：http://hz.316326.xyz/gtxgdxdhof.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.52xcode.cn/gtvyneypjr.html

PHP:  array_unique($arr);
来源：http://hz.feifeiyinyue.top/gtrqpenjpe.html

JS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gttkysxjnp.html

TS:   [...new Set(arr)]
来源：http://hz.guannengcc.top/gtjhfwrahn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gtihbuygon.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guannengcc.top/gtrfqryuba.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtqjnnoayo.html

C#:   list.Distinct().ToList()
来源：http://hz.jinghuilouyu.cn/gtfdnpyqkf.html

[D16] 求和与平均值
来源：http://hz.sysykeji.top/gtgffkbaag.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtsqhcrpog.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtgtqgwdqi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtznvhhtto.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtqxqapdwc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yangfankeji.com/gtpsedydbh.html

Go:   // 手写循环累加
来源：http://hz.aibaodan.cn/gtlykcirdo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtpzgkkvdu.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigfzy.top/gttyodgnxs.html

[D17] 最大值与最小值
来源：http://hz.guannengcc.top/gtivrnqonu.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtdpfbltgc.html

PHP:  max($arr);  min($arr);
来源：http://hz.guannengcc.top/gtbmbzeupg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.birdmap.top/gtdqdktnzk.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gtcuzqwnba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtutuokiow.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtbhnhafzz.html

Ruby: arr.max;  arr.min
来源：http://hz.yj202588.top/gtxtblrgwf.html

C#:   list.Max();  list.Min()
来源：http://hz.aibaodan.cn/gtuqxqcbwc.html

[D18] 扁平化嵌套数组
来源：http://hz.ywan-chungtsiang.top/gtxunuofsb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtkzxxozre.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtfezozgoe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtuqjctkpy.html

TS:   nested.flat();
来源：http://hz.jinqigufen.top/gtdytudikk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.snrcjt.cn/gtejosprqn.html

Go:   // 手写双层循环
来源：http://hz.jinqigufen.top/gtwqmmlhnr.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtzftjmckm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gteegmhice.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtgbglxslw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guowangkeji.top/gtgsadiuyj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gthcznqxcg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangtech.top/gtscvqwqzs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gttwwpdinn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gtmegyavnm.html

Go:   // 手写 map[string][]T
来源：http://hz.fzhhl.top/gtrqdtydbv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenjidiqi.icu/gtcnjeeqzc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangdashe.top/gtxgmqnfhc.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtrlceinhz.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtjmubspzp.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gtcthzmode.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtlbajxhky.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtpcowhxqv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zycfv.cn/gthrtbgfzu.html

Go:   // 手写 map[T]int
来源：http://hz.shangyingyoupin.top/gtfppfzarp.html

Ruby: arr.tally
来源：http://hz.xziqi.cn/gtvoxwkszn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gtgewlepfq.html

[D21] 判断是否包含某元素
来源：http://hz.pengpengdd.cyou/gtyplxvfet.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtkksrghgz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xinyue.icu/gtxwruxhzv.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gthubvgdif.html

TS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtrghctgig.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtezqqpoje.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenlongwang.top/gtotcyigfj.html

Ruby: arr.include?(x)
来源：http://hz.yj20258.top/gtmkwaplez.html

C#:   list.Contains(x)
来源：http://hz.guowangkeji.top/gtmqyuvjdp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.bjfxy.top/gtruhocrsy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.snrcjt.cn/gtgrmwsqkz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gotoacloud.top/gtsxaypwnz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtqprlhtye.html

TS:   [...arr];
来源：http://hz.nanxuanxn.top/gtoinjlopc.html

Java: new ArrayList<>(list);
来源：http://hz.sysykeji.top/gtltgpkqkp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtwvwqgdeb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zdqjudy.top/gtomhtjtzc.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gthmhvwqjo.html

[D23] reduce 累积计算
来源：http://hz.snrcjt.cn/gtfczfbpoa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtbncmtjap.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ivvv.top/gteoztsori.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gthbkuxtfp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtbiomaaop.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenlongwang.top/gtueymevej.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtqwztqdit.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtwwksckhl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jiagoushi.top/gtlneikzyp.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtwrjolwmv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtxjpfbwel.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gttfrqkfzg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtdijnpius.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtsvurtpbr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuanzx.com/gttchlzqcr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtzdbvnohh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtqlmfoewf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangkeji.top/gtpzyiiclx.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtssuphkmp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtdifhgakj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtpvjvtcng.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtwhryexvm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtxuepkwle.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtjarbfsng.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtniogfyar.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtggxctrah.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gttlapeldj.html

[D26] 数组转字符串
来源：http://hz.yuxming.cn/gtobqfgyqy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtieopkwmb.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtfwmawvcv.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gthzlxrfqq.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtdloklvly.html

Java: String.join(", ", list)
来源：http://hz.hnxiangtu.top/gtltiltmvl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtuvgtdryu.html

Ruby: arr.join(", ")
来源：http://hz.guowangkeji.top/gtxltbbbnm.html

C#:   string.Join(", ", list)
来源：http://hz.nanxuanxn.top/gtjrvioula.html

================================================================================
来源：http://hz.ydjk.org.cn/gtvyjbiddd.html

E. 字符串处理
来源：http://hz.guowangkeji.top/gtoqokszqf.html

================================================================================
来源：http://hz.zdqjudy.top/gtgoireahz.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gthwrgtmmo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jlsjyb.cn/gtelgfvahj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shanyushiyangtech.top/gteyejvyso.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtyeskznqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtewzsagln.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtgavjvuli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtbanzgwvv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtnlcjlctt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtjmdnlxvh.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtnkatlvry.html

Py:   "ab" * 3
来源：http://hz.c1oappe.top/gtvehrkinl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtyeisvsar.html

JS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtoknzwppr.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtdtxglgup.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gtfdiaykvy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtozlqmicr.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtmhonbche.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtygvarcmh.html

[E03] 截取子串
来源：http://hz.xylfe.cn/gtuwhcphhz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtdgkhkajo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xinyue.icu/gtoqvwwfmb.html


<!-- 参考信息 -->