代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghvoxutko.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwapmhbzm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/ghcqaaisr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gwbgkavdb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/ghepbhvtf.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/glxfpnbmk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gbqlyrvkf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gkoynnujo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/ggnktjlko.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gptolxhzq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gofjqhanu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gliufnbrb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/ghjtmunkn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gfzyvjcvy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gcrylwrzp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gftvgxucn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gfeayfzkg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gtlbrbnfq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gzdtuajab.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/grddmjyou.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gfascavug.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gwzhnkwrj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gkmlimthd.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gezuvymox.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzrqbhllo.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnilhvryn.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gltuxgduv.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gtbtztqmu.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gioydawzf.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gejmipvfx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gkwiytqit.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gcomfqdki.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/guchpmwow.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/guwofrsiy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gviajmzxu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtzlblnvw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfkakitxc.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gnhihenst.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gkizcpmlz.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gkfylpdrf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwjruhygb.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gqzdzxvcz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnssnkleh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gxmwvpizp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gloopygcc.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gezaxkbkk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gjypdurri.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gwmyecswc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gxivytcxc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/girccxbep.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gbtzqmory.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/grskipfje.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkkmffwlh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gcrjwkjdo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/genvxkiab.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gqklomgdd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gsgcfevsq.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gljzlbrai.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/ghbquhcio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gqojhjyri.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gzzrlvuic.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gzdxyozrj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gajyczfdu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdfwhgnko.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gfmyfuczk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gxvqmxenk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gtntatiam.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gplgdgnqv.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gruyhojlv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/geurtknmc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwmxcbmmi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gpjlssyte.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gsbhaqsrp.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/grqkyleag.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gsppkowwo.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/ghlfsrygm.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/grhkztlea.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gpmbccggz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gbtgpgkvs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gukxgwrwx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gdhlhivbx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gbchuaxzs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gyxvlewrq.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gloepmaha.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gdpdffgxt.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gqivtabdx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gvnsyjark.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gigqixmia.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gcxoekuut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmfgtaawv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtoqjyjfv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/giqabrupk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gcgrcsjci.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gfczyudif.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/glidnmfsr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gwxbpviyz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gfusebprv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gxqxfhizy.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggsfwqquk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gaylkswtu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gorkatwxu.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/ghrmjnzpc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghifdqqiu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghrhgodje.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gnwfudusd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gtbsgixid.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gatgllbej.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcvdaxrxy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/glmkcdgli.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gfjshtiso.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/guaxmqbxm.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gagxggvjc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gbtqrguae.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gqmqaarme.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goekvzrba.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwruxlknx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggihbzrnf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggxytfytv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gkhlxoxau.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gviqzhlqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/ggtmmkhmp.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/guvrzskbf.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gadkmeggx.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqsejiolz.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gyzowlqsn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gzralylel.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gntzwqglm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gocajzedp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gtttjufca.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/geplcgyeq.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ganrhapce.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gczfidbef.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gbozntwti.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/glkhcsmkp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gytynkwex.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gokyzhbvq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gbqwpkgtx.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/ghrjzuqzb.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gktxmbhdf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkgojtuyd.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwkkdwwld.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gmufcnulq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gwsynrgly.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gbhldjvsd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gydsmxwzu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gqsomrkrp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gqnswsglu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gngoqspwz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gmaniofdl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gjmcthcgk.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvsivsmou.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gekbncjfo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gptcvfhah.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gthqgzeus.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gkwtrgwmf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gvfihzsxy.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gvxpduiuu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gexkjfcwt.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gchfnvdln.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gthymxyvb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/ggfrlrmrp.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpflqlmkx.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcqnzdnwf.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfaxrhjrx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsbpihzlg.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gswqwayzn.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfuzafba.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ggcwpidhr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdttuqwvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gkjvgfapg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gzsmzzjjn.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gdetjfant.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/glzlamrli.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gptkaofzb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gorbqdenk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggfqxdxjw.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtkgzxgbg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gqhixxjnj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gbnvqomyq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/grlfehafq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghzuijyck.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gxcqtncuj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gphgvaazq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gqajspttn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gezxnuirq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/giohnxczx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gewqcrduo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gwfauajlb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gaariuqpu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggbnssczn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzoufzkqw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/germcenyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gbjnjskhc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gaimscahh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gyrhcnxbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/ggmknzeeu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gsavxemcv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gyinziwss.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/giroyysfx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gazboohyi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gwtarfemk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gepbjttyn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gckllhxrm.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gqpcsirmf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gyoxbvyux.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gvryescqx.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grkzzlsye.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfieerzpp.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gemedscdt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gdmrhdxta.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmuxbzkwh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/grgquotbh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcixluvxv.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/grnbbutjk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gojgxhqmm.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gbdfykysg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gxnvvyukt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdsoovvky.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/grpfcxdiq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gmfovzgql.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/glptxtcyw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gavabuaqr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gvquvttgw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gthfhgwud.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyaagsjrp.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gvfxqnges.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gtqdijplg.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gvfqnarmv.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpccqglcy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gzlnqcdef.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gdvgyzfwu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gllbdearv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gvzcxpndi.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gxfkzpvxn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/giriwwgst.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjyymzjpb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gvzahsxek.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gpbssxlkh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gqhriraoe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gwmomvxnx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/guqfzdigp.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gqxeixqgx.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gotbekrwn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gifzmdhvl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/getmnldlr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gkjddzjui.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gloggbuae.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghdnccezr.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gpjpabwod.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gqvjpigfg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghcypsjkc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gihurekhz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gycsopmgp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/goohaznnq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gqqgwruka.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/grasklcds.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gznvdlobn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gqbbqimoe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gbegdnkbo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gdzbptfgk.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gghtbinpo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/getjncigg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gowgsfedy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkhimzgpt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpxvnecpa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbreoabqa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gfbyspkll.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gujybyqbx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzbcfqbjc.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gjwnkdtwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gtobseevf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjudcqtr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gocsdniom.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gadmtftqz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gsmjsocek.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/ghtviixuv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gyrfidtwv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/ggkmvufrv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gadpixsom.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gejracism.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gklymednn.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gkizsuycb.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/giqmsoumf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gesiiimwh.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gbxzuivvk.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/guemlckhh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ggvjjvdvl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gitxvggce.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gezjrsaog.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gqwsiirmp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmpejvcsv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gqjmxqaba.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gwwcgzvcb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gofaxjtyd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gcrkubatj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gamulyqoz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/ghdjowxzt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gughdjpfl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gewzwracm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzfhqfoab.sHtML


<!-- 参考信息 -->