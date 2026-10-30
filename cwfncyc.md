代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gjzhffvad.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/ggznkcxhd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gnnrizcgh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gatrwqnxv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gnxvrgxeo.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gezutsgyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gflhsovwr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gnutssxyq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gxppdmswp.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glaqkxqvt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gshxgeuxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/ggvhpcmpu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gqbjauooh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gysmzpthb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gyuanuyif.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/grhqtwwnv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gewcqyzec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/ggyibefni.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gosbqxztu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gcodtbprl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gdawpqqlf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvevpjztp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gjclvcupt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gsrnkvpax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gviazmbzk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/ggnlszqcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gyeaelqka.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gikimsqoo.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gunvzimuh.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghiggyzfj.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gxacqttgn.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gyywwleki.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gkcgzcsyk.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gnhhisjrx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gwurayahu.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/griwrxwys.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gdldxrpvm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gmcwrbpya.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gusaxaelx.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/glzovrxpn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmerrqdhx.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gjotoxjek.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gyyadallq.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gzmznievd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghqwgzfoi.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gmccdmmmw.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gepespbkw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gxtvhotly.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gcrhsdbhx.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gmiuofkaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gppfttutp.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/guwjvlhba.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcaxoorcb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gavixskng.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/garwrrlkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gnkseditf.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/guqctjzos.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gldsbwhdy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gjusrdyge.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gbtgeenvq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjtfgodak.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gxnmygayp.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gnorrhywc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gbdsdyvvb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/ggnialxqb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gigjdlzyj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gzcxvzhtf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ggwqzymud.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gmvdlubcl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gtevohhlb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gdhlmggab.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gbukrhkux.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gzsixmeqn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gdifoohkd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gcmsomahr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/goaqavlsk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/glcbgkkyw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/grerfqpeg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gsprmtocd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/grzmbkhnk.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gjdbknvsk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gxradqwfe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/goxvyinge.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gxiccnqsx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/goiueilhc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gtqiierwr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gawljknxw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdmgyzetx.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gxlzhqemk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gpthzjxiu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gjdubxcbp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdeuffqwb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/glchimyzf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gmpvpavgk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gibcpjdyv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/ghbbhjdkf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gawelwatb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gdpisrthq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/groudutln.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gmcwkxslc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gddcppukq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gozipygzq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gggbcqyfb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ggwtdlvtj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwvdqrjnn.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/ghtbmpljw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gdzsbewws.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gvlevigzb.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gxnvjsnhl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gamulnezl.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gtljwahwp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnsgdwuoc.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwdsipzyh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gcpythemp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/geceefwsr.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gacgxgwxp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtpurgris.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzsyztp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gtsgxppbq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gevnpqdvk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gotxbcqvd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmeiqkalz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gppidaguz.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gxknndpcu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gxbsbkmtj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/ghreyzdti.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gnikxlusi.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gbmlbgeyr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gdbybjgbl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/giqlzpess.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gwlraejcg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gwupdpqtb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtjurjfnz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/grxgpvcsa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gpoysmwqd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gmwryegcu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gtzogrzzl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/garcgbqcf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgxtasl.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gfueouveu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gneiahgyr.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gtzgeoiwe.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ghdtqhwdm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfvgvgpxv.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/giuumzenb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gaxajylzh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gjemmegrp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gxqxwimqg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkhoadfng.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gosdxltri.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/ghwkpaxgx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gxkoljoqr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gjkszvxck.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gtnizsrvi.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/godrosazt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmpziuap.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxqoihjqu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/guelbpiph.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gsmkicmeq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gsayttqky.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/geusuhxaj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gdtwakjsr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gzlcscoly.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gysfsisvw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/groyperik.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghboxjtcy.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gmyugagoh.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/glpmgijjh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnzjqykop.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gmobchyph.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gqkwbhcfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gcbaglyzt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gbwsvgewz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/ggtkrgwoa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/geqldjkba.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gslsqxulv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gomfhhiks.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gijyjtxmw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gdhgbssmb.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gfuxwmdlt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gzjvafzfc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwvbxeoce.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpnlepyfa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkotlnmju.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcfnxphqg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gdbaydboj.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxelpoybp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gbiixoajh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwgpyidxo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gayurxsdo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gkckkovqc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gscjtxqtr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpzhqqkyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gzzswvpbt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gqnepnzgw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gtxqbujjz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gwpijczft.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gjowsirjt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gstembbyj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gbsgpqvmf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gkmeokzzv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbuooxxqe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gdtxijqlj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gxdtevvrt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/ggkuhkngy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/guzkfbspq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gtpfxyqqd.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/ggrycjcqy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gntvmsxcz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gejrwwfcy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghqtdfkgl.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjrpixldo.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/ghzfalyne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gzjglbvow.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyuvvhbme.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gbtevvuxe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gicwsrgms.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gexrskaou.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcdwkrvba.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gzlcxqymj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/glycynfuh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gtvguooly.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gpsgxqwce.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gdnfegtkf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gybtsojeh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gournrtnd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gmcdnuzit.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gflzjkuxi.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/getpeydml.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gyoeasvgc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gtcyxrmhw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggnyahncw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gbeffkykn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvwpetsob.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gsznfhmab.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gmcmfhsrr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gsalqkzhn.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gvfwatbqi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gizjvrfmb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggiuxldff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/guielxvjb.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gciuvxqjm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gdammtkpg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gsghwjffh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gjrdaoepi.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gngswccof.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gfrrqtsud.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/goqqugiah.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/grblykxim.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gemoxdgvv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gduzkbwpe.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdksumtsw.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gwfldkcmj.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gxdygxeom.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gthtntfsz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gvfqqvtzg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gziihsrle.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gtsbslrpr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwmetxzpd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gjnsrkyis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggbtdvpae.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gfpawsajx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gadcwaeoc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gebaellkg.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gabaopupy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbrgolreo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gweyujecg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghbikusqi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnvegucoq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxwklaend.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gusxbkern.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/girmslsqj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnxjrivor.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gigxeqbey.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gxhdrpuia.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gyjtieqdc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gxmbwezex.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/ghyrmwiqa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/glolxtorp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gxgtvkvjp.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gwoskchys.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/guhqftuvd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/galstqlqc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpppdyrta.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gxjjvvsxs.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gztegiffn.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ggtnltbqj.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gypchmcjp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gednizdjs.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/grkguxicd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gogdeynly.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gishciumw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gevavdgyj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/ghrslwuky.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpserbohs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gpjraoaqq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gsxyncaha.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gqskkoulo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gclypgzli.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuynwxkm.sHtML


<!-- 参考信息 -->