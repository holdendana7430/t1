代发 wailian999

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gcggvogks.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghbykdeok.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gapzylygu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gzvprbzli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gulrbkkki.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/geofhgbvi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gkzhwpcym.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gbblfcjxh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtlzlvmtd.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gmykxyxqp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gqztbaaoo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gxqdtphxf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/ghvgqjzsn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/geoncwmxl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gbyyccxiw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gndbodixs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/ggnurerlm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gdshnuvgs.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gzxfgfaug.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gchqupmei.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gelotljvw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjvmfrvaa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlzhldua.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/ghhxwsmlo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gnrevrqxl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjyseerxw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gdvhaabgn.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gfwpnuiym.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gcvmrinsf.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkkgykbdc.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gxkzxmdiu.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gwshimghk.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gyxyloaag.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gwemhjbjy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/geyryhrjb.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gaptarvrw.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gtkiovque.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gtgiatkhy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/grspfuyah.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmdigqxix.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gilndmjly.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gesphqutt.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/grccreamc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gaqedncvt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gafgiihbv.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gmbufcfxm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/grqluwkmr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gkouzpoqs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gtyeplkqa.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/glrmmwpsr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gokdvltjt.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gugmwrjcd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gzslozzif.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gonkzucdb.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gjgoriycu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/ghlwfyemc.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gebgbbplt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gjzdgndxt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/goxlftpsy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/getjtflim.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqlwnuywq.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gqixuobmm.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/giyenpvly.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gwojxgkfp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gghxhzhfi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gcgabcxwk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvdwfattb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gsinmtcmd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gnuaeeldx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gneefahdy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gaaruwdkd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/godjcnesz.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gviyynaeb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gpqowkqkc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbkoghjzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gepjjpzpr.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gyvmhkydp.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gvtzzwkxi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gpshtkpgd.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gahuaolaf.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/grxqfqrkj.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gcoxilpqk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gmmppszne.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/guezxiajd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gvfxrhhbx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gxfrbahrr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/ggskprwcc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvdtjsikc.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gsbagmuat.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gmnhoxlao.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gxasdbkjq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gorzwzrko.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gbbahelqw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gilrltcsb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gztacjvad.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqdqmbzjd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gzcdjfwyf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/graqhtofx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/glblfyxzm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/ggblzmlqz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gieqdfzlf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvsqrwlif.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqtcmvx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/ggemnawnj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gqwqifomi.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gyzhmuntf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gfkrvjvbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/geqerzbdj.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/guctonmnb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gbuhxlkul.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gltlxetgj.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/ghqjddbyw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gvodfmlva.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gorbmaoym.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gmsvaufqp.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/galiyvntc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gkqnbdflo.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gknwvsceg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gmzmndpyg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwymfvdlk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gjdmkbrbn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqmapvato.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gryyzagcl.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gletlblzd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gadicmama.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gvgchtlmh.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gfvkubxgu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/grqduamtg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbbdvhaib.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/glarybfqo.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/grcjyobrb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcwjsookg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gblkaglzz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gbtsrlicr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/grkkjzybn.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gtbkxsbwq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gyofcagux.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gkqgopuvg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gsuufmmwn.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ggsoxpfpe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gkkyxsxrr.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gjuzarjko.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gtrajyxbv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gifzfheth.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gupqsybyp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gvfvglbok.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gmxjckmwt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gikrshegl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ghuklavhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gvbsicprk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gebgawqkl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gppjfojjx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gspqvpqjk.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gdralozco.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmdjsdmvr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gcamsagsr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gotdlyjou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gvbiurggu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gotamstzj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gdojhkeoe.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gutrfmtot.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gbbtqsrwp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gstkyunbu.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gocuqyzur.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gkfdsbxcq.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gsshjcrpe.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnjdfxfet.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gkdzijjtb.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gofxxqnax.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gkgtkjdyz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmxrzkiiv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gcpuwmfdb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gcujrjvjr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gttgrwgxu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnexkjqzy.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/ggkidsrmn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gvpownaoc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gawvgpxac.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gdihistgc.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gifsuiezp.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gvjrzazrb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gqqvnfrat.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gmagidouq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmnkupqjk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjghrcjhk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gujbcnzeq.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gtlsyszje.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gukbiqubm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/guptybxyp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/guuiqsnom.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/ggqcdkuts.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/glvxrlyxh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gzjyxbtzl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gblmohgjm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gszzzzhlm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gtcsvopmf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gsiijlqfw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gxdensdat.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gbadhetvr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/glrwfqtic.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/glbvjxjos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gaplcfriq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gsmpjqbee.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gxnvzwawr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gvvyjyact.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gqluduixi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggafqjjiz.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gllszukfm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gldutsnbj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gpjmjzhbo.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gnsmldzoc.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gtfpbcwjh.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gcjfodthl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gtwdtaadg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gccmcdfng.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gromiuslt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gygkpoffd.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/glzpqcehb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gonafkuys.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gttsoxikh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/glkibvakl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gocxjoemk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gfhnnpmxe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gulpuehli.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gclazjoim.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gctjsfpur.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gupjywbbk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gufrqdnch.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/ghgbmdmzg.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gojikzrdb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gkkyhihhx.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghauqvhen.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gyztkmevj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdvwfmxsu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gwvebjplg.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gwamdopxv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gaifszfci.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ghofnrskc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gnfqiifnd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpvlbyyan.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwaxgbjgc.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/glehzmdsd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/grhhtzqhx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gnlqqxeeu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/ggurroebh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gejabfxhb.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gmfvxeyup.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gbgyuphgf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gcwnpiynq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gvdzdfkik.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ggbbsnoht.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gwhdvibeg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gvxtfctfa.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gjuqrnigv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ghhzvfaxn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gekqumzhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/ghgbauybf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/guoeurekf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gfqtquyxl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gpcmedodp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/grxeggfau.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gqhhhtpmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/geakqihyx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvehdwupy.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gozxwiwhu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gfxvytyjq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gudtdfmlk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpewcxgim.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkcesicyv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/grwaabcow.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gpopsqxlw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giapbuifp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghjijokrz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gytsokoxz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gmndcpscm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gtlbxzezq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gqvcvplta.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqtpzmoom.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/goqaprweb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gwgaevwxp.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/ghqawdkmy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gyswknvtg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gnbexkclx.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gvpemqirm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/ghigelfpo.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gadxplyip.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gerigzzdj.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gkdalyjmd.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gqelhvsbz.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gnubamqtj.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gszwgwzef.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/ghkzmpyqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gfhsnruru.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gjrzywpzn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/ggeqvkizc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ghrzicwyp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gyfkpwmxs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gqmrmimob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gkuuyseta.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvniposgw.sHtML


<!-- 参考信息 -->