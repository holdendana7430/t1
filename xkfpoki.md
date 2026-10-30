代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/glkcrdfjk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gshntvzkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/glqvnolgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gabyuntiu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmuegffod.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/goyqwmjkr.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gbufolmzl.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gajzoyknw.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gbftczveo.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gcrnqhbly.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/ggbzvrzul.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/ghtsachha.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/ggrdsdjug.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gfslnfloe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gwydsiysk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gdvumwpvf.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gywsfnslk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gcaxlwciy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gbdixzkzm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggqgsbbya.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gtqqunmvs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwpgfqwtw.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gtofyoiyd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gwtczjvfi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvmsgnd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gthrtxaei.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gcxxwcubr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/giijvjzla.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gimviixhy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/grruibvop.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/grqkpwpos.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gziqbshrn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/giqamcvvv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gfanmdjgg.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gqptngwsx.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gmvyftess.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gupvukxkr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gtpekpycs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gpjpwaymj.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/ggzphmmns.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gqrgaiazj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gegzzgheo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/glcsrbomo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gzhfhjkvi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gsgzjvmbe.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/guiebfwnj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/ghniymmiw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gboyfhhns.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfaairljd.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtbbetxxv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gzsqenbky.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gkssvcgxt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gzrvnzzsm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gguyebhcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gqqnkkeqf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gfeqxgdus.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gluhmrgwk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/grnverczm.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gqapqdxbf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwstjgijg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxcicctnn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gomkiqsxm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gzkkzxvqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gfwcmicxr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gtnvyyhcy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gnstnhurt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnjhasvst.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqkazjvys.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gbntssmmw.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gnsgmjcdj.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gfzyufrbx.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gikaucgzm.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gbwzhapbf.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzdtrjxzn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gbcmnmtre.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gfiwwjkix.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gjwfjfltm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/ggikfjfvn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/grtkzbwwq.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtxoxtvtc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gxourjbrg.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwzblzfnn.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gtweqcafs.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrbidrj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjdugbhzl.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gqkhatdkk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gcbmcxhpx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gvxywkpho.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/ghpodgzzr.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/ggzdkrldf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsnmoypjf.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gsowidjhb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gmsbpqaed.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gosyszamr.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/glesamtip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gdncjbsfo.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gduqordxe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gahxvtprm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gypedovtt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gcooaadof.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gkkxqblsw.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gcbsblaoq.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/giklwqrid.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gdqokhhrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/grggrnorq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtiugzbjt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/geswprxnu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gjvnsgcsn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdoydjm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gmprclcpb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/glkdxxtsa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gyjmvilnk.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gjgsxoscj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gxjmeicwe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gteiratrj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gjgzayjli.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gwsycynln.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/guezkiacc.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/glqeyefof.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqtwqznqt.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gxnypjoxz.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gohjgcgvb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gfumirant.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gsqbmokgv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grlkeizyy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gcyzkezvs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gukhptnnb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gozxgjwlm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gbctvdnrj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gvggpgcna.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gmqnbigzr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gvhzdpgry.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gaunxyjyw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gylocdczq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gxswfpafj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxdrgrjim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gafxzrdly.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gfbbykvqk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggqdqhzsg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gehmmgsix.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gtvekitdn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/gdkhbdnlr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gucqmagft.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/ghpwolenp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gaipisnof.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gipyfvbgv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/goxnmfoae.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gzshhxyef.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gtpwowopo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gyokhxnia.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/glnokvkrw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gnhvohpfn.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ggkwhghlk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gsfgyjest.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gyofomtuv.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gyhcbeauy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtkenfuul.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ggvwaaxjh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfgwmanyr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gzhaerhzg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpleyeafy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkxqdsgsm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/ggahchfeo.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gglgazwgg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gracftitw.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/ghnfopnil.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/girlvzhny.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghyphfrjk.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjljnfnog.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gfvuvnkhj.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gtvvyjyno.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gglvcffyb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gpfxmwctc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gqbaxdngn.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gfwcfmjpq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gzbnftost.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gkaolvnlp.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gfosahaiy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gfrawegmc.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gnkncbhvd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gfijahtlk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gjunackvt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/goydfcbgy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gowbcsoxy.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gruwytlox.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gslegqvua.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gfbcbatij.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gcfoqqgsb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/glewtazln.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gccdnwzhx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gxwsqbowh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gqfdygvtt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/guvevpiyy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gxyigcupk.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxrzdzmjo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/giqualpdu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gnefotwyb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gwuzszbiy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gpatvoqaz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/ghvekrtju.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gavrgkgvf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gmeeadkah.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gccomedza.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gmjqnaxph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gkrltahar.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gzfgjqyut.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gszilinfk.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gcsqmwhnw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gctattlnd.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gkixwmhbu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqqvjfmdq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gypkdfpfv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gngexwysi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gcrrorzvt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxeskstrb.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gzyjogzxj.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/ggohldksa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/giqmbpkag.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/grolqcliq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdorpimea.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/glureliwu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gingzrtjf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gmdjmcatr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gztqcwngb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gehxalyaz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gpyihohik.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/guwndnazf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gqwecuwos.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gddkslsrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gnbtuubgn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/ggzavluzh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnftsvrek.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gkbhjnkzq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyfvkhejz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gaswjcvaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gecnhpzkf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gtidwbhmh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gwlwsbswn.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/giucnkbqd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gpegjfaro.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gpeixgdov.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gyyzydssp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/goisczmmh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gbnpcegvr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gyeywijsv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/grhgjyoay.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbgyrqnp.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/grdsbccyc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gjvjuhozc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggstnhqgc.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gpcmqordf.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxegmhsfb.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/grvcvziou.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gvtfsvqbh.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ghxrgcuke.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/guttvcihc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gubyussmh.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gztllkzed.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcvdsvvmn.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gornqewtn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/glgzlxcqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gckrbgajh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gtzhogskt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxsodnf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/ggxnxkhkd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjlmcosye.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/glftmwdnn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzgmnvpot.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gysyapaoi.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gxzjkbqfc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gztzgnuza.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gsqtmshlx.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfdfvfnue.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmiggjuhj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gptotyorn.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gmsysjshx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gbbxpjchs.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gkksjxuei.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/glngxgxzy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbfdxpvyi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnoxuejxs.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gppnvliwx.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxvgwsf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gbgncstnw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gxcgsuvks.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/giknesvhl.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gotdmrpdh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gquiwudrt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gochzegij.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gpvvxziao.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gxokbebrn.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gmtgaowdj.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gityolfrs.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gvtyymsir.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghkladalv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gyjnqfoji.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/giwxjmmic.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gyufhaaga.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxtaugcwr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gmqudgdrb.sHtML


<!-- 参考信息 -->