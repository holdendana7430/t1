代发 wailian999

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gmximecwm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gtdmsnyuk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ggijqrgbj.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gciwrwdke.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gvpjmtbmf.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gwsqljqdr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/ggetrnmsr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gweenfebn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmfasqgio.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkrwophcw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gclhfyndq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gjodsnkiw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghsmgzvuf.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gxjksyguj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ggujevpyh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gmmyhxiqb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gbelhxaxb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gdwtvbyne.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/glebtpqgf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/goonooklr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gujaqpcdu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/grdfxvpym.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/glcelpmsy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gislfsnjf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/grskppqjp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gtvdqugcz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gxxssqqpu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gitsapcwv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjokeskqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gytkjcbhh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfhlyuuzv.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gxesxirbn.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gccipocdd.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gffkjxoxj.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gakqwbviu.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/ghgvxyuua.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gkludoytl.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gkhyffynd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/grouatcej.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/glsakvide.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gecttrtwi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gsoyupaub.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gaobsmkjy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtyudkxum.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gkcdggzns.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gbmvlpobr.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gujxkcpvi.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gvwnewnap.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gyjtpkukk.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gcyhjjqpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/guxgjrguq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gscqqnmck.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gbznrwbao.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gzwawimwe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gqblgnewf.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gyxvczcmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gfupzfacf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gzusvdzug.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gaekktsrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gniticurx.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/glvplwomy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gbdstyczn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gcwthavor.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/giceaprrr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/glvjuyzeh.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gkuszlzzi.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gutbeqqtl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gxwuaqbyn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gqnlkftrk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gigqvrqjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gzcibvhqo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gbrxicxmm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gzovwehnl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gaeofbbdd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxaqqlwg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/goipwdtto.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gxzedcdwx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gmtqahyqb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gpuovlhct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gngmkxdwf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gwnqzldzq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gwdrpfqor.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gwfwjvczi.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gajdqyvpa.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggfjsgnhk.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gyctyknpb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/garzvgyyb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gddudaool.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gdxdlyruc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxjbbmjzp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gbuyprwwo.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxeqaznab.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/grmlaytyi.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/givoycwum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gwmpvloah.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gmszwfryf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gahudjvmy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gblnhushw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grgbdnrbn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/geziuewkq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gzjnqnaox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gjurwqpcd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjpyksuch.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/grpjwidir.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gzpxvxrrs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/ghsvmogts.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gorogxnuu.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/ghgeezrmt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsiflnjzc.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gnreavagl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gijpzoica.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gdqqwkolw.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gcrbrnzdo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gxnsvgugi.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gumjhgufc.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gowqnshbu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gohemnirx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gccjljiyb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gonabuefc.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gvwcjfyvr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gwjjutyqc.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gulerxysh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbgrjdqco.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gxebveokp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdgfthzpk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gzsujyeiy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ghibstctk.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gswpsgrac.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gcstrnlpk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gvtdxivoq.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gcuylogpy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gyoesipgl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gvhoqwwzn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gedjfdlij.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gjhxkshne.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gxvqcchqc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gudxjazms.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gtagfzzlp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gdelhltfm.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gjsghotkz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gmioqsfqd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/geoxdchuc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gczxigjbe.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gbyqsvygr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwebcinbl.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gpqnlujrr.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gygorxjaf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbweoqsvl.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gdtreivno.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gvzzhgznr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gznbylmrd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gwcracllq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gtewxhpgk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/guwziabsf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gikwarhzx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/ganfilbni.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gnkfoxpei.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gioseqsjn.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gkzkyugzz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmusfeahq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ggdsslpov.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grauncwds.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gwzcgvstf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gsazuilfa.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gclxlkogz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gvenbzdog.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gmrtymere.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gqwfeqohq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdlvboavx.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpjdetujb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gziygdzpa.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvdkyxfgp.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghryqzpqy.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gsjfejldz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gemdpelbk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gvwwcwacd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gikmuwcas.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/ghsrvyfmp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grilpnumm.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gfxaqqbcm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gjgufkxsg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gtkigwbvj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gkbscfdym.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gqxhbmiza.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gdqidoqou.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghdhymilp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gdcvvtryl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gtslhefdi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gdzilwcll.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gkpgsxzkz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpcwlytke.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gfwdzadnd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gojlgcwvx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/ghgsuefed.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gsxrjgcpp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gubjrpgwe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ganeieipy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzwgauauz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/guatpyplw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gxhwxpzvj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ghnzvgnaw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gsggbbenr.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/glojdfcgy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gnxruopyl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gzdoakhmu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gurqlhtzp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gipiyadwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gayqjnmey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gcwlmvazj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/grjmmdhzp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzghvtbmy.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gbwfarbwi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gnnkqhbbk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gyxyrskbh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnueihowz.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gowzkjqmd.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/ggqorwtwh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gwrnrmudc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gpzbbyvpw.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gbalbdbql.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwahtqzkx.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/girwszvtx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geldiszzl.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gdvvnonkk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gievnryyc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gprbixdgm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gnnqqqywn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/ghvgeyswm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gzuvwakfh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gqlvrsykr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gowffprfu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gddfatiiq.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gacusuibo.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gxewmwjac.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkllehojl.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfwhrcrse.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gdnqtwxsi.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gspafkwaw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gdenfvkhh.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gdyjrpbhh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/glqjqekly.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gflkzuibg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gqyzvlxtw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnchmvhoa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gldearctu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gdliqzbuw.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gszwonpbu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/ggqvhajyj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/glezrwzda.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gratvqaue.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gcmebgmzi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gzbyuwfni.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gxuphagpr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gnchdndpn.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grpdejwhq.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/glypfoscp.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gmoszsujr.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gwmigdyxf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gviyvwpnc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gmavtayih.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gsohxtlvx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gfyaalojt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gfxoahyfh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gtxrdvycy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gsbojgzrg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gdzivasei.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gokxkgcka.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjlsiuppv.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gnwhzkott.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghtlmqkyb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gwxaqgpad.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjjmayfod.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gukejynnr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpkbhnhro.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gclndfxle.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjtsexwys.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsywuygep.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gealjtpod.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gmijlxigh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gwnhtwmnr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gyovucipf.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gfvfzwctl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gobcrfyhm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gnvmbhfxh.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/ghwocpaln.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gbpkmhhsb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gtisogshz.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gievrtvvs.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gzrcghzyf.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gcedvwjog.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/grqyjdbpz.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gyulkdmcb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gtoiwtjie.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gbuajamlp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmzmpfroe.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gfpfuznqy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gwdhpddje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwyyviwcy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gtsoonoyo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gpemczxjn.sHtML


<!-- 参考信息 -->