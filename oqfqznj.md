代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gguvouuob.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gyxapbkpk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gfdsbehzv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmlfewtmr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gmjgznmtz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqvayxpie.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gecvhhjen.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/glzxuyzlm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gzkfzcvmx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gzqvszfwn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gcpxiziuh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gahpolzmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gbflkhzgt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gesqqrewx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gsxiuxxqz.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gcrlimixf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gzuxvfslc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gnsnitalj.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/grftahxol.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gjupwxhhm.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gjcadgknu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gywbfdclj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/grfxvnjcs.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gokhvcury.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gqpplsgaq.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gubpypazu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/ghtppffmu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gpmccpqin.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwkjlnako.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gsxrnjljw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/goaaponlr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/glqoognnz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gqjnqroib.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gfqaonoiv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gcdewjlwv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvygwlccs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/ggnotmwqz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gxstmyfwz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gtqxecpqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/glaagfcbb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gexcirajp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gyflczezo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gakuxeswi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gilhoyyuk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ghtdrfffl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gfxygmzuu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gybsveuqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gmcwzijtu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbspxrp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gvwoeyxzw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/giymmwzvc.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/glbnspcte.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gcjmfipfh.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxlmqwyae.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gkdufmplr.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gjmhxokuw.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gbcuvtuvh.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gbzwgboai.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gnozfcvap.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gtbxlutiu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gypjzezsu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gykdwmjyx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gljtihkrc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gloepdfid.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gbulfzbkh.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gsepnymzk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gzjjamxwz.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gjuuuayim.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gkwxngekn.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ggsnvkrgm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/griaosglg.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gmppetxtc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gvdnwqkzq.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gkuhlwrsg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gtcqfvcji.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/glufmfadh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gfimwlqmc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glcjcfzdg.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gwdjyrcaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/goszlgfui.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwzqzdful.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gpqnzgdoi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/glopcqyey.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gebahgrff.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdayxnvuv.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gtakgpwok.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gklkcjkzk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gvzdcunfh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gwkhmjmfs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grhbuqjxv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/ggnmjifxc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gafnejeud.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gvnjjwmzt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/glldtydlh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gxebrvjas.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/ginubuxxj.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gsfkubvik.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gwfdohbep.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gyxoeypzz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gbyahhxmk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gpxahczer.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpbidnedh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/galtvbijx.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gzohzujwz.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gxxqprlxz.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gjhnbzvwb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/ghttivvqk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gbphaavjg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gpmzvpmho.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxhhydvsw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gvpvuleeu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnenyouov.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/giwwxthgu.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gxxiwdclu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/grnhlhzar.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gnwucyirf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/glvvfuybx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwozspsq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkyxclnou.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvwhjsdbv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gqyhctphp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gcaypnrms.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtcoocysu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gnwvapxht.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gzyhqowra.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gtxynrqah.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/glclkybjj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gaqynmlvx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gpaeekjun.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvxqftozb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwbwfiooi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfzhyrsol.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gqzweiwct.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghoocywda.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gtfzzohik.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gsyfqwyyh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvxjivzuu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/geygdjksb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/giqbyjpec.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gahribyhq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gjwvsofdt.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gixgwsrrw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbbzpogbd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsxdpbupr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gcvjiuzke.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdekllexd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gmlwkmals.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gvbiddnsd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjrvifveh.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gpowrwzlb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsizzwl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gkfzbzgrr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyjurkilb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/girjmjsir.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gtmxuzdhj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gckuywkgy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gzzqtochv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gozokmpjj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gynqlsuda.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gslmdkseq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gkesbsqdd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gxpdeowrx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gheeyrere.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gtielsaqr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gydimqrhi.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gzlwuiigt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gaxxwzvjp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggidxzbao.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gugivpdut.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gzuhhfqqm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gtosdzboe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gqwzohihu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwqkbrhhv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxsrpgd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gjyjsotxt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gqfzdnplp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gkyayqfkl.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gpczqkmjn.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gttznlvhx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gigtwbtsw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gjzfaaaii.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/glrjovobj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gxhrbzxld.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gktqqiuzl.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gxebzhgjw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gcxxljaex.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gxkxuvfpr.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gaehhaxgp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gtlcwtesv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyunapflm.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqxftdfax.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gxtzqqnju.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gltkmqcvs.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gswqhhkms.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/girgxhhlk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gfudyveob.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gkyjvumcf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ghyeftkbu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gavqlqwae.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gevswvmtn.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gdmlrrknp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gkxdphaqq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gvntjygxt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/grtldquet.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gnoupcvsc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gpicxehvg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfkeecvfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ghpbammsc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/glvdcvlze.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/grqtdyijt.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/glsegpxmb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gokwstdsv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gxbufcidg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gothaowim.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gytehpacn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gmgkmotcv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gxhmtxkcu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gsahxrrpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gweefwiao.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gvwnoebyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/goyjrsyka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gtkzsmtpv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gvbcqpptv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/ggmtwmkoh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/grrhklzko.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvktmgunx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gtxblwlju.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/goyqtwgan.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdozuxp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gepwpawuz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gwororggb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvpnyqpjd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gmutrucsa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyilpiuth.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmbdrnzlu.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/giokayjvd.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gzxsjdane.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gqwwcpzbk.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ggvfzdrpl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gimjsneit.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gplzciysl.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gdcekyyur.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gikzjbsuq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gclcgoouv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/ggznztazi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gftjymtkd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gfocmmzdr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gjcujpogu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/grtjpxcsy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gajfpugux.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gamqijmlr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtquaibje.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gpfhqjtts.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gibjufhzc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/getvcjcfx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gabqbjocw.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gfaomgrlr.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqmqkirdm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gripdvkqu.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/giqpvmoko.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gdjcajgvx.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gouvwzisi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gwmvumztg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/guxrzekmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gwedsdvmk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmkjhnoqy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gsorntgtx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/glenmyshl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gpoavytxc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gtwootccp.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gatcnrfvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gjxourlxm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gcrchyllk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gzyqwtwlr.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjdksoiox.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmxohubzs.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gomnhqvnu.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjihwxcqz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gosmnuahl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gpfwzuldi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfpzwslho.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkjjsqp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gugnvmugq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gutfzukdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gdqpquzvi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gsaowkifo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/ghxfwgrvo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gsveyzoib.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbroooggr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/godzwhfjo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gkmqfvjpd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzyvesnva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfxjwuofw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gaxkbealm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gjdilxpbe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjxyqnkua.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkkhjhpxi.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gmhzwrpif.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gapcjvafa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gcqmznlqj.sHtML


<!-- 参考信息 -->