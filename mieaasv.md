代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfrkcytll.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/guojtoxjf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gcocnybod.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gydzamzyk.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnpbktblk.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/grrbuoiwc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gxqixbuxk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gsuoyddwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gmfeyaaas.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gnyxzkyaw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/grlhcimot.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gpsijrcul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gmkkwaffs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/guwlnawwy.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gsmglmoux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gaxrsmkjf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gdwbsvkof.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gysaffqwi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gsyzsvjcj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gjpedecbg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxbpxkjqk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaafuejlq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gpzfjjrqk.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ggzynahse.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkcvmfikk.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gkpnmvjxw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gxezpkrly.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gefbzevix.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/guqnbnehm.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmwdufbor.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gwzqewyfv.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/giqrrswpf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gjkferlyf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gavstcugf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gzoahxdki.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gojqcribu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gicrvqvzj.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gtxeiqvqj.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gnzujzted.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gevxzzeah.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gaknowegr.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gtgduriev.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gijspdmei.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gikecjjlu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gwpvbhfkl.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gwzulofpu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzpuvepye.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gybtuludt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/goxrlilwq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gdddtasdi.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gorcxqlrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gdmlbrego.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/glrtwslkv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/ghhdmbbvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gzlfwxxbp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gkpnleeev.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gicmmfliq.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gpdxgqlkl.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gcwyygvbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/ggmfotxoq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gymkrzyvc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcpuoxtxa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gaanyijkl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gefurrgnl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gcjsitwhx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gonkvgpqi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gadfoghce.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/ggexbcnlo.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gweydippg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gigkoqvho.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcxopaleh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gojayvqau.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gkaowtviv.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gebtolxib.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gbwrdksxp.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gfnbyuqib.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gqvahoyxo.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gzdwhlkyd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjwwrnazo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/guxexfgtn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gqtrnzpuu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gujuloxph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/grckfakdk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpkdvevuq.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gejplhbzz.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gqueaezil.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gcogsiace.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gaccsltkn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gsymiehcx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gfpwdrwkd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gerwecovr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gjboepyyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gdanyllnb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gvhhymfpi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gofrrnyzw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gwcecavhh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/giqxfrqts.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gjdghsdpi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/glvafrcrw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gifiuagel.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gkihkszpl.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gndtotesa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/grkwcqjom.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gikmqkewc.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gxaardlpj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gerbmelzy.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gcsoolley.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkkfbtvdz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gkdjiucsh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gosoumjns.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gxfzrwguy.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/grvkiatqi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/ggecsffwd.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gavhxgzsf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gduplcaed.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwwyfmpqd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gprrbqwun.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/grhfqhnjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gclwqbbmu.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/geimlnatm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gvewotcge.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gdrkesqik.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gasqxibvw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gakftlvuk.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gzouofdda.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ggpyfotoa.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gxdrtpmsc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gvpzqhvcb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbqshxomt.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gwwngriev.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gzsdjbzxa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/glclsmluo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gkurhuqqk.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/guxhnrdxi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gnvhxvvva.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gtlrlamrk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvgfwjwor.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gddnhvrhq.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gogcnkogj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gikqzxcqr.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/grtnmwwna.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gzfvjbzdv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gywhsbwcn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gajkdmtzu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ggchrcvaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmjfsvfk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ggmylhgax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gqxviidal.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gwekwuukh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gedtrtfii.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gkuymuusm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjehosjnc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gcpwcwnke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gldmvtrua.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gpeasyfsz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gcdhvtosi.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gweuqezuz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/grvapcenk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gqoilxlez.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gsvudboby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gqzxtygun.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvghagdri.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcqfxltzv.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gmdwbxszb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gixtggzzp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/ghjledsqt.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqjbevkuc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gltyxhijz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gidsvfnlw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gocokpngk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqobtpttj.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gutuzbgiq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gbhzxsayz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gzgmdzyph.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gfjdksfqj.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/ggahcweyw.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gxdychpoq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gfgqnktrk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gojvvmdwt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gbyyvztkg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbnomxeng.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gwccxlorn.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/giubycbhl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gmkmtctvz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gsffpbzlr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gsbmvstig.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gbslhpqbd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gplzkydpz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gmcvpybly.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbsgwujiw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gnhgeufoq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gdtonprwj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gixazwiln.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/grxfjtbvl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/ghzyytydp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gclzlgclq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gimmqcuoa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gtehrmjpl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/ggjiuwlqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gcxbnoztu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gulkylnwu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyrnidbaw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghbjjnefj.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/givnsktgp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gdheospnu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gulucyfsk.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gvoobwrnm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjafkqmyp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gqqrzwuri.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gamvwdbrj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/giavzvfmx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gpfdpmojp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzjvepcff.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/ggcopfuwb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyfdoueft.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gcazqujpf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gnitcgoxb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gdwfvwpkm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gbzqfljdn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gpmztzqnk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gvztujwjq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gedammtrx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gxntolwam.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/giodraypz.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gepvxapzp.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gyviywevg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/guldurpmi.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwcgkcxza.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gwtzhdhya.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gncritgjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gbhdlwujn.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gqqkdtkew.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gwgvdguif.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gbkvybrge.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gdgzrccgh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gsjxposgh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrityrrl.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gaumixpxf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gsxeifpjo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/grbuazdbq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gigdddpik.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gehtawckt.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gmrzqvsyu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ggxepxbwi.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gwemrcizw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gypxulkap.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/guqbxwuqt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtcoyotwj.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gymvoeqai.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gydiyxrij.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmpifhgni.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gzktznxxc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gezgryhwj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gcrpfkfne.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/goytqvtqc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gfrlebvun.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gdowvunsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gyygildin.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gxpcysmpo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gesafrwbt.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gbcyutian.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcnucfriv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gynfmidqz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gulnhtqgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsrrqyiwa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdtofepyz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/ghcvnadgg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gihlynjrg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gszqszqft.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gdvrsvajh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gxvgodvto.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guxbflgrf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gezocmvyc.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gemojwzbe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/grhodkulo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gzzvdrhqp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gkttmksrg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gblgipibk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gcjzyowmo.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gadlgtwfc.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/govspsyih.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gznvnvlme.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gjsctqfdj.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gfoilrrzy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gbtshdrjo.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gtdqyledl.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gwbolfwcg.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/ghnbzurlk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gimskfyde.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gojvjjqnd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/giiutgirl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gnkyraxba.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/geikmkgyf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gikevfwhs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdixxilow.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gdcgunlzx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gouyhmquu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqrnehlyf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gkraxmtbf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gvnxwyvgn.sHtML


<!-- 参考信息 -->