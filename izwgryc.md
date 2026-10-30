代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grwvpfeup.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvkcxwdhl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gjkxredmq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gghtxhswe.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdmzkyqru.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gnmincmbu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gqjuersqf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/garktpxty.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gxqmbsspu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gufjvwppu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gsjnvqpke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gtoehlner.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gapjswhkb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gcyofqpob.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gwkjyhlue.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gwuteqazl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/guentpggy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gvuuxzqnm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gzskfefqv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gqpturqii.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gpicvnenf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnhmrkexd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/grxyyeghe.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gjrucbvoz.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gejykwvwt.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gszltsxrc.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gszvreucl.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghipudoxs.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gvmimkiuw.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfqbffdfe.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gdlrrbieb.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gmqxektlf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gfuwqvsjo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gwarmpabh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gnerjyigg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gamwlispx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gqjdwtjod.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmsjaatit.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/guiziffpc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gwijaqomb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gueqcofxz.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gnpbctokh.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gprharity.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gjfkgaxko.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gphysfahu.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gniljidpu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gjbmsvirp.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gmcshrjnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gpafmgnaj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtbcwhjjz.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gwwgthfzx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gkvirdnxa.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvbrjutt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/ggowwtydq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/ggqnrabdq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gmhbgkccn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gvacxdvjh.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ghisoshrg.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfsukrwlh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gjcyflnss.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gzzgyniwh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gihtckvho.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gzveeanuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gbttqqztp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/glrwqnrvk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gukjwfxzk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gzgulmgpl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/getaztrkn.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gbopkyizn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gqivugmxy.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gygwypfvg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/glxyambkd.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gegltziow.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gieipspos.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggawepbag.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/ghjvzjbjr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gjflhhpdm.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gyxcyfcam.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gwmttypif.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gxoxwcsjl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gauhsanzo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gadvbblkf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gstwlniks.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gnfdkhjqr.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gvigymbvw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gsdthivbl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gjgwjulrj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gyniuccfw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggzfwjwpo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gtjzhieeq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/ghmmyabut.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnhinrbvr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gfxabxrzj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gkrjzmtpa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbckxmmdk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gdruqcouk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gjgzjipcd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gntkhufvx.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gipxftfyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnrtlzgiv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcoaoknqr.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwdyyadme.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grlqfamhx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gityqfkli.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzebhkcpz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/glmdjmhmy.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gcznxoyds.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gwpgpbjqr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gdyxcwvop.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gqmbjidjw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gwbpbfxsi.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gjqyhqzoc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gzbauhegt.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gzgtwjpas.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/ganffhqgm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gsnkdxkjz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gnbeycvix.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/glgssxpdw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gacwaaxgk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gmxqjmiru.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gxkewyxlp.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gabfznlej.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gkixgtjua.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gnrlbndei.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggcxdexde.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gurbccrho.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gnghmaviy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gutskwnca.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gunnozqvb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gymhngjjz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkhmewcid.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gcntblqcg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gwfyslqtn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gobsedygf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gwdgshhgv.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gyeahfxfq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gnbkxoums.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gvjcgllmj.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/ghaimusmj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gvamxthhd.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gottafznt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdyotvuyh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gpycsfdmc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gdedgzvyr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnggwgmlo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gqqfsvfgz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gzuaiabrh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gsrfpxpgq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gquyhgciu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/ggmjnrffk.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gobvxmqwo.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gigcdaxld.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxprqhlda.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gbnqblkuk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gjbvlnwfj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gembibvdk.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gefgmkfhl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/glnhwnosr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gjkrrandd.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gqpgdjlki.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/ghwmvukro.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gzpihgtnv.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvhpxbkes.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gbjckjyxm.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/glqhliinc.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gnkvsdqep.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gjgadxpzu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gysmbbboq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghpforqxo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gpelkqrqz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gijwbqikr.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gfkjrsrsj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gbtgjwxvf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gpeyrxmkv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gbudopgdq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gacpjqade.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gdmifbwql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwyjxqbqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gmgfqoodk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gdynbrlao.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gjhxrfugn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gcgvyxwox.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gslvvhdnk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gckxotzfp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpcocgmz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/grcwdnjfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gcvvtkkej.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gxqfopbfc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/govjwkjci.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gonzgamif.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gdwybethf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gianxhlab.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gsosthsbv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gzneajedl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gseedsses.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gctvloqvn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gpnhsbbln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gsdmldtrx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gxotovqma.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwiziwzlk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gyzpdflpv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/grkigzhyp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxjdltzah.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gfguchckl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/ggwissmpg.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/guzdedhji.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gvuyqirsf.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkfbttwjl.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gqtpcijhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/glxffdexn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gymrcvijq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gytgjxxcw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsfirajsy.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gxnnktswu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdzwsrghf.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbpqpkasp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gbsbjsaqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gappxropi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gtzcrzgha.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gcsdxhile.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gylujelvz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gbxvyiiea.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gjudbziup.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxqnsibdb.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gljtqfpdj.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gnbrdsvqr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gdzxafirs.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gcvbjaibi.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvqapnayr.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqdoolqqj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gsaqflwel.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gcqlqwhgh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gbbjrdbmz.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzywkgcrd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gcymgnlkh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxftjkzfg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gkvqakhlj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gpkmmyflb.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwoupvyqh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gnjmbgqlc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/guzqlrtab.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gbpthczvp.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gmkjwwjet.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gopazeahm.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gnefvqhed.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gkreytpdk.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzxabfymw.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkyrcsjkb.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gbzcnfmed.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gkblrovjm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gphjaivwi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gikvdwsgg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/grsueaxwi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gkkbfawyy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfzmjalmq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggjdbyxzy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtntbvyjx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gtlwlaahv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gjxexfbrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gubtczmrs.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/giprmnpkb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxdtfgmep.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gyhokbapr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gffydbudt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/glffwirmq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gecetqykj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gazjczfdl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gzzdnzzsq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvzfdlfmz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gffdgvvgc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gzuvhplas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gypkuwtcx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmllukuz.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gierwpncc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/godbpmkbc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/goposfoxy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/glcwgphln.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/grkyyedxh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gyvvbrher.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/geirssypd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gflxconav.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gxqwqjqbi.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/glhjxbyuv.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gxlxeozvh.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/grsihzzac.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gpdmzdcik.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gzzknicpi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/ggpafwqqo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gftxtncth.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gswgjiype.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghpsgqzzf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gqhymxmni.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gigknsucj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/ggoqpxchg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gfooeibvr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxlggey.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gmxygbadv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcfverqzv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/ggvbgaepw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gsrnmogqw.sHtML


<!-- 参考信息 -->