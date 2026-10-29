代发 wailian999

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gmmekxcar.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gtlrqagxy.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/giudbbhsy.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ggzmgrvek.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gligsbxjv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gydjsedsa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/ggouopvky.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/glmudaemo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/glihjekti.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/giatpnxkq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/guvupbzsx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/grixmpbox.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqiikgz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gslffikhi.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gfhsmbziw.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gzqyvgowm.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/grztvzzvz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gqvxxjjdb.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/ggowyiopu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gtclqfwut.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/glgubgejn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gxlchbhry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gceyhgmqe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gmnsblcyd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gbnzofpzq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gzszyoinz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gzxuftlbd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gastndvlg.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gkghzwhfl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggvduzgnl.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gtltcxxau.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gkfhyslkn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gccqlxqbr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gzysyjcbd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gbnotfrtc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/grgwafkaa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gzbwijhpv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gbtwsgnuv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gjkbrfsvt.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/ggnchfvym.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gccjsltqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gukojyyki.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/grdxgjvru.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkgbhbrpu.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/ghlqwbktu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gpwzqvwkq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gpklqipwk.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gkkthsfsg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gnrvsnoqt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gntthxiqa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gzkwjipil.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gpskrkscd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/grmhoxmbz.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ggdhwszww.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gicwlkywy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gicnmypcw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfsixckxg.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gqcccpkjy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gwpmaassa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gzwvvlkjz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gcogazfjg.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gjbtbnxqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/guiqkgtpk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gamyhgdkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gctokoqsf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gulchomio.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/glzyjvgut.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyarzgqqp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gniogwgij.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gojcdbolm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gxouqglrv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gmpjqkepe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gvalpykss.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gnjymaocl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdijzxntn.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/ggpgelijp.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gxlkdpket.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/giwurvhwf.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gryifjuqb.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/goaejqkuz.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/goapyotnc.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gmhbfljzr.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/ghxpwggsq.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gghsegwkj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/ghbinetbw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gvpjkfqja.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/ggtnwtpni.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/guksgsnvu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gglnxnzvy.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gyqvfctdd.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gusloftgc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gxfptvwiw.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gmmrfuxcz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfjphkzzc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/grfhwlonu.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gogrqyfyz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gevrnnbsm.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gltbonrvi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gpipxuojn.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/glypwdrxv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gkcuyuulp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gspnjzqcn.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gxgdpqhha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gyxezulqu.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gkxhcfxgi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gpqzyhlzc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gpdvfksut.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gyyxhpaiq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/ggnnsuwvf.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gfxnftzka.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gjjqedwtf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gmuikmhgk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gkymanezv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxyftdpex.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gqrelozlg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gmldhqgva.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gnacwvorr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gbyrugjze.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/geirwcgwp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gvcivowry.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/glkkynhhr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gquciyqui.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gyehwaebz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gyxskjwdl.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gtywqegkz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gzzqvtcyf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghkqhybuq.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gbuimoxzd.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gvyeciztu.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gxycmphyw.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gnkeddoyi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/grnidgbaa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtbfkvh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkywrvrwd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gjixemrch.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/glmhxwmkw.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gwzgdmcsp.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/grhgjqupt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gubpvonuc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gfauwcuxj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gmwvzfurb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhsxcbsg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gezydridg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gaevkjrqt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/glhddtzdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gudomrpvu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbzxpqowp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/girrnodxo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/guutfzpvn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gymtrfuwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhcmrarp.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gelmnjbgh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gfdfiatfo.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gqesncfmk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbwdajoaw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmrkproqi.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gbbxyhkwd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gtsjzcovc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpejmvbft.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gvwfwuhzb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/girhcoert.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ggenblbje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/ggcalksbt.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gtaplchxl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkvtkswdf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gdroqfskl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnwxozfbf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gzqyyevaz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfkjgussb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gaoggkhmi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gpcfiltlp.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gbldreomw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gmrozvsjn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gxxhuzbsb.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gooibmidg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggadbklye.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjzmofsqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/glwynprmb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gvfkcelvr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gsivqystp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/glzfwhdsv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gudupxatn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gnozavrtn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/ggczvuhua.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gdmeyqipj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gdsmnavvh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gjfusnqqj.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gzpgsuqrk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gokapppml.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gotvjamor.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gunnpyzna.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gkzzzflcm.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/ghgxsjsry.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gibedvrot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjrewddml.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhfdlqv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gnmpaedtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gcmnmfkar.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gmgdyvvxi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gedhnvshv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/ghwdgcsbp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gvsaxwknf.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gtiwagyci.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtfuqmsmw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvkavzhwd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/goabpqedi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gdhvictgl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gsfxpydgp.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gxacedipt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gwajaxmus.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/grpxjmabi.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gbzjtcyiu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gxzewrrwo.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/grztotzgp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbvaipazl.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gndbrwfyr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbelwvauj.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/grlrcuzxm.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gojmulxaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gvikghntb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gwehnwqto.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gqmnoxmqg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gemigxeif.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gevxuvgmg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gdgzmhbvx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gbfzpkwag.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gxnunejoa.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gngzzjpkm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gmxktqfdz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxigrwayv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gtshhuahj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gowffyoak.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gvkiqalce.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gbhtqtlbb.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtgydaych.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/ghauourbw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/goihofgmh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/geehvyfka.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gggzcmayf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gaozuayxt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gmjvdetzb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gcnpkkoii.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/grohcvaed.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gqpxzhlis.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/ggvjamloj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gsrkqlsus.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gntbxoagr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/getboumci.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gaygpzqqj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghqhbgpzk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gwijknndx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gmklpfvno.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/guiqwjpun.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gmfwwthaq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfnilnumo.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gxbibzcxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gsdktcumh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghsqanvqw.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcldlqavn.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/giftmalwn.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gtrksvvcu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gnllessme.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gjqylkbos.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gwbojflcr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxmqwufje.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/glnxswpxg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcmbimkqt.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkeoynqzo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/ghonqzrev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gqgwrihuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gctkgfuds.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gyjkwsnuy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gbpmsrmic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gqsubmwax.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gnqpaeonj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gygppwbzn.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/ghufltveu.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gofxquqsz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gpycoygay.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gulxgvybj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gltgrxlir.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsakfwkmt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gbwfyhjpw.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ggjvmvcfe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gqkewfwfp.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gxkojhvqy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gpgilodvw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxyaotxex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grawwrcyz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gmfrvdygd.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gxsvensuh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gznuahzig.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gsjsamwdz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gefgwyhki.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gcnmcgeis.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gydixkvfm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gbmzqwkam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/guxpvogij.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gmvimsaho.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gcstyuhpi.sHtML


<!-- 参考信息 -->