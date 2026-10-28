代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sxryk.cn/gtvajghjwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtubjqabhp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhongyouzk.top/gtqyfblhlv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtcoxdjget.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtjlzwnjph.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gttddekbqf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenlongwang.top/gtenccoskh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gttvzmjliq.html

[C14] 泛型函数
来源：http://hz.wangshuangyany.cn/gtmqmmkxro.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhijiandao.cn/gtfnmyvwsw.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gthqlmojya.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtcxeikyhe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yangfankeji.com/gtarlnvoii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtusablqsg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinyuanbaomall.cn/gtyazaomxn.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtsatnawbq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.kuanghao11.cn/gttwdfdlhn.html

[C15] 解构 / 展开参数
来源：http://hz.meibo888.top/gteofmdxlp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gtfrrhsxpt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtadmpxwln.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gthxneyqcn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtsjvxmojq.html

Java: // 无解构
来源：http://hz.yvedp.cn/gtlavkpzux.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtvfjszllw.html

Ruby: a, b = pair
来源：http://hz.havefunace.top/gtwqjyzfjx.html

C#:   var (a, b) = pair;
来源：http://hz.cashguo.top/gthixvgeag.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtkmkdeiaw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtonsbyrad.html

PHP:  // 无重载
来源：http://hz.feifeiyinyue.top/gtprlmdanc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fengsongda.top/gtwxzdyoos.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtwlclfxnm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtxirmdibp.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtxknnzeju.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtuujmjrry.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cheryme.top/gtagigcokk.html

================================================================================
来源：http://hz.jinqigufen.top/gtliuodrft.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtzdantrxu.html

================================================================================
来源：http://hz.hfpthk.cn/gtlrsbsnrv.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtjyiparmk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtkszsffef.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.iojbl.cn/gtmoiynvpv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhaomingkeji.xyz/gtbzcproks.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xingfuxueyuan.xyz/gtqtukbsuq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtlbgnsckl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtxwqcveqw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yvedp.cn/gtajcwngob.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtcyvgdvwm.html

[D02] 追加元素到末尾
来源：http://hz.iojbl.cn/gtkovjfybp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sysykeji.top/gtwehnjuor.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtpwpyxukb.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtyjwsyinv.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtudjgqcrv.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtuwdpavpl.html

Go:   arr = append(arr, 4)
来源：http://hz.jiagoushi.top/gtccosjsfr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gtcihxknqq.html

C#:   list.Add(4);
来源：http://hz.yvedp.cn/gtiftbygqm.html

[D03] 在指定位置插入元素
来源：http://hz.sxryk.cn/gteqnexucu.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtiphdvigq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigfzy.top/gtlgmbttsp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtqkbjydev.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenzaomai.com/gtygmpfzyk.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtupcoycrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtevgkvcqj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hfpthk.cn/gtuvbhutse.html

C#:   list.Insert(0, 0);
来源：http://hz.iojbl.cn/gtpjdomilu.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtnhkwyetl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtgqicztaq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cucudq.cn/gtujcrfcsn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.meibo888.top/gtwhpwluau.html

TS:   arr.splice(0, 1);
来源：http://hz.cheryme.top/gtrvncmooo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtihwqvjjf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daria6918.cn/gtjrhwkefs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydzc1.top/gtbpjxiuwu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cucudq.cn/gtcxcqyvwu.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtiuuunqor.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gtdpksxubs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtkpzmplvx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtmvnglixo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yongpay.top/gtdpgpnsqs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gotoacloud.top/gtsxcyznio.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtvmpzatme.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtjfehogec.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj20258.top/gtbamwcxpd.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtatgtlvcd.html

Py:   len(arr)
来源：http://hz.9152youxi.cn/gtgviwnhul.html

PHP:  count($arr);
来源：http://hz.iojbl.cn/gtprddmipj.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtdrmernwu.html

TS:   arr.length
来源：http://hz.aizwys.cn/gtolhvtblf.html

Java: list.size();
来源：http://hz.chenlongwang.top/gtnmgjpqez.html

Go:   len(arr)
来源：http://hz.jiagoushi.top/gtkrnjtnoa.html

Ruby: arr.length; arr.size
来源：http://hz.zhongyouzk.top/gtvrzzydih.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtrbmzwawx.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtmvpgpqni.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gtmtzlzopv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinqigufen.top/gtrjbivosl.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtzpbzvpqe.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtfutusksw.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtooijjyxz.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtwkkyptio.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gtbylunfwp.html

C#:   list.GetRange(1, 3);
来源：http://hz.xinyue.icu/gttycldbqu.html

[D08] 合并两个数组
来源：http://hz.cashguo.top/gtowdqxwlr.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtwcjzjstm.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtjdohacza.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yueranfly.top/gtezaulutm.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gtsqeunowg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zycfv.cn/gtdfxxdyvn.html

Go:   append(a, b...)
来源：http://hz.tian-w.cn/gtuslbsueu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtlsnzgvrp.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtksvglqmt.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtmktydbqu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtmyftxqun.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtozplhesp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtjduquuko.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangshuangyany.cn/gtymxaatij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenzaomai.com/gtkchplzvj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shuidangran.top/gtkkzritcw.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtjotuiceh.html

C#:   list.Sort();
来源：http://hz.xylfe.cn/gtazajljrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangtech.top/gtsbjwifqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtzejsszpj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtgubyithb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gthqwkoqdq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtgpwubwkw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtykemsyaj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cheryme.top/gtjpzanrst.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gtsegkpexz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.aibaodan.cn/gtnmzogmxa.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtfkgseetq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gthvfvfghe.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gthkqfwugy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtuzlsbfsu.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtxsdszeum.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtaccwtesi.html

Go:   slices.Reverse(arr)
来源：http://hz.feifeiyinyue.top/gtqvgmlvpv.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtzfmxraxb.html

C#:   list.Reverse();
来源：http://hz.shangyingyoupin.top/gtbusnapss.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtlxmzoshi.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtmsohnorx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.vqdsnc.cn/gtogpqlzhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtpvzxcokj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtolewwsqf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtahkzvttl.html

Go:   slices.Index(arr, x)
来源：http://hz.316326.xyz/gtmslyhjfj.html

Ruby: arr.index(x)
来源：http://hz.havefunace.top/gtfskzzppu.html

C#:   list.IndexOf(x);
来源：http://hz.xuanzx.com/gtabhvijlu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gtrpjznbbb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuanzx.com/gtwmzpejhu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtuovagumj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtlnmvobis.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhixingplan.top/gtekcbeyle.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtzpxeysmx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hammf.cn/gtesheqsbm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tanke756.top/gtwdsvvxhf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtkkbgsocm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtnuxhgdwg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtooodftpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gtchqgzirc.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtmpnogvlz.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtmbxtjmor.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gthinlkdrb.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtzeyzejit.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nanxuanxn.top/gtqoxxzufm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhoulong.xyz/gtdudybehh.html

[D15] 去重
来源：http://hz.kuanghao11.cn/gtwtdwebor.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jlsjyb.cn/gtkthlbazw.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtiljkkclm.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtnkpoghfh.html

TS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtwgtyxvkt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tanke756.top/gtcvmflzuo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gtgnexhamr.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtqemticyv.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtxfkabqob.html

[D16] 求和与平均值
来源：http://hz.ywan-chungtsiang.top/gtshqnebqk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gtchkrqwnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jyoumei.cn/gtccpqjdem.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtfcozujwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtosfdlhwu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtwwzpwlhv.html

Go:   // 手写循环累加
来源：http://hz.yj202588.top/gtjngomddm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sxryk.cn/gtxibrikqv.html

C#:   list.Sum();  list.Average()
来源：http://hz.yanxiufei.cn/gtqngrhhjp.html

[D17] 最大值与最小值
来源：http://hz.yj202588.top/gtyllinngi.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtpdinhygg.html

PHP:  max($arr);  min($arr);
来源：http://hz.yonumen.top/gthryjwvgb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hammf.cn/gtblnouhsm.html

TS:   Math.max(...arr);
来源：http://hz.jianghu66.top/gtseipdvwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtchqkzscv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtkwuzkonx.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtzblsuusa.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtdwaxerfg.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtjjfxwfae.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtgtzatqho.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtjextbwoo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aizwys.cn/gtsqutrkfz.html

TS:   nested.flat();
来源：http://hz.shzxlz.cn/gtqmqzveah.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gtwvgdzueu.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtdasqixrd.html

Ruby: nested.flatten
来源：http://hz.svipenyu.cn/gtonuiaczw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.meibo888.top/gtpixdustr.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtjeozsroo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtuzsnmwyt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuanzx.com/gtkcnlzfud.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtnhbxgyih.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtpayrbjgo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtijzjqsaj.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gtpssrhami.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ppjwa.cn/gtkwbckqsg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtroyeqzpe.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigufen.top/gtmczxgtlf.html

Py:   Counter(arr)
来源：http://hz.yonumen.top/gtkylximbf.html

PHP:  array_count_values($arr);
来源：http://hz.daria6918.cn/gtrhbbaqaa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtorhdbqgj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtuxnbweqb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtnxxzfqwg.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtmizythil.html

Ruby: arr.tally
来源：http://hz.9152youxi.cn/gtrloodiaf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtoblnnbnp.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gtjzqkgjiy.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtbtvdhhhl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dashuyun.cn/gtmpmnldvv.html

JS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtujsjophz.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtnwzldthi.html

Java: list.contains(x)
来源：http://hz.hfpthk.cn/gtfztgrnuc.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gtcwdmtsxh.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtyfikelsp.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtczbvkeqw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtybrnayrg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gteajoumwe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gttdfcirvv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtglylorwo.html

TS:   [...arr];
来源：http://hz.guowangkeji.top/gthvksxogm.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtozgebugf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pycfn.com/gtakzzhsuu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cheryme.top/gtrwivldzc.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtziltjhkv.html

[D23] reduce 累积计算
来源：http://hz.svipenyu.cn/gtoldgrjcb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtmmifxgal.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtrgktsyse.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtbgedzzwz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gttjqjfzwj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tianlin.xyz/gtwhcatvzb.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtxbwswjol.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.iojbl.cn/gtcoipinul.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gtncirztmz.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gtslarxhpr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtwaeyzbyd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtskpxwppg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fzhhl.top/gtkqfkgouc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xinyue.icu/gtlkyulbap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtokuxhrfs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtcruipbiv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.feifeiyinyue.top/gtnnimdpby.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gtuvlxioft.html

[D25] Set 集合去重与交并差
来源：http://hz.hywenlv.cn/gtifqlwxjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtbwmckqve.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhijiandao.cn/gtfdgwdgxm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtubcnhtqg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yonumen.top/gtqitsbhjp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtddoqosay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gttonkmqgi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtdvezqjex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangshuangyany.cn/gtjxnttdhw.html

[D26] 数组转字符串
来源：http://hz.hnxiangtu.top/gtsvgxxwiv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gogol.net.cn/gtpixncdnw.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gthhnkqftk.html

JS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtjqzfhigf.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtbilbkpmu.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtirppjflj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dianchejie.cn/gtxjxlcvbl.html

Ruby: arr.join(", ")
来源：http://hz.nanxuanxn.top/gtzrblmoww.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gtftbtbtyq.html

================================================================================
来源：http://hz.yj20258.top/gtjwgdifrf.html

E. 字符串处理
来源：http://hz.yj20258888.top/gtaqrxjigv.html

================================================================================
来源：http://hz.wangdashe.top/gtbzhpxppt.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtrwofzooi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtqoeqctgp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jlsjyb.cn/gttorffcxf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtoqagapmo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtcfgpasnl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuanzx.com/gtwpuqmqjk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtyrtvxyfv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gtthedfxlw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinghuilouyu.cn/gtxljamcwb.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtrifqzrnm.html

Py:   "ab" * 3
来源：http://hz.jyoumei.cn/gtnwczlaqf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuetiantiany.cn/gtdqyhvygg.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtgfybsega.html

TS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtgzbbqhap.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtecprsmqu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.redwolf501.top/gtwlkpjvhv.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtksyqahig.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtcxnbathm.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtjougizbc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtchttcsys.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gtgacymfms.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nwbrower.top/gtnolnpsln.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtpgcivmwv.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtnbgcyklo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cucudq.cn/gtxlqduyuw.html


<!-- 参考信息 -->