代发 wailian999

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gpsdxyurx.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gfmmncpye.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gvnwpougj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gefrieguy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gpnhmnwwj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/galpicgct.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsnlejvcy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gmlydwmzc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gokwfagtn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gfjrcdtyd.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gmkqsawyn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gvfejorxi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/groowkabx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gtxxfpodf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gnmbamidw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/grmztatry.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwnotgnay.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggyijbgjg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gpqmcjxvn.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gfstqeqls.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gafrfqfzj.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gclucorhh.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkkfvqdms.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gsedhmnoh.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gstzifbuu.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gfpglrlpi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gmiqbqwsx.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gqxdyshmd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gbiwqyjah.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gbuqhwxru.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gzrrupqbj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gtnafgmri.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkqjkbens.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gjvgazbkg.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gdnsqpves.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gqcstdxxb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gwluhavmk.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gnyjvreim.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gjlayphtp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gyujqpiaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gznopvrlh.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gyniuxuac.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gwuxsojda.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gqbxoxpmj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gnosmuyqg.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gydrkvgsn.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gjmovshyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzrbbzaun.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gffixswce.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gebrcnaqn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gatcicczs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gjhoebvqh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnnwjvpfg.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gpoxvpxjy.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gzddmtzdn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gcclhcttz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqcaqxmsj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/grxtyduxv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/guiuomgcq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gdpwonicu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/grooslzwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gbiymemsk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gzogmlqjs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gxzdhelqj.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gpfnvrulo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gidzabhtz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/ggdzkmwjh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gybespfgd.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gsfgdwbej.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gzmcigbct.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggiqianxt.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gcskdmiqr.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/glszlkjni.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gmcraimzt.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gpeqdcyag.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpffehyaj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gewuobdit.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gztcshnbp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gkupwyzju.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbslelwgb.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gsqqsxrbg.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gsmxybsgr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gttbrugua.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvcuwvewl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gpmkrceoh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/guxlurzfk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/ghqtsvzxi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gtgdutncf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gbjnukers.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gpqgwboln.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gayeryijg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gzfahsfxc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gjycvejks.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gtgxptrsp.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gzxnmgnjf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gdsazfmxa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpgwvmmti.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gimtcuurv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gktqrskha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gzuzlzyel.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gvcrxerpu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjidulmwq.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gigffolzq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gnnovtvxy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbynsqfwb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpguhydvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/ghzrlcqbd.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/goqpnkprx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gedwgnvbx.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/godtlpphm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gqcugadbo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gqafvxfwl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/goprttdhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzwtutmww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gyomaaukp.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/grsejpcxt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gkswpyocg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gjoadnmjr.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/grftquwlb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gkizolzyc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gwzempzdf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gywidtfgg.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gjbpwrefx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gsoinvguk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gdmuzavcb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gpqndovqv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gykbjgwxs.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gfuaaqhqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gcdgpgtxg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ghtbvdlws.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gerolvjtu.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gdznnbkbj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gqtzvndjt.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gprwsktqa.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gybvlxcwj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvlxtailb.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gqzkmjbyk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gtqtdkowh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gtpjfiwmv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gmbwwwsjb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gvelytrpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/guidijvxt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gsslfotet.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/glofputyl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gqjuwlcjj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gmwxxwdly.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtwipyofq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gdwtiowrt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gotpulolu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gdafrsbyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gstytpgbo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gbdltkfxb.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gvxudmgrk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gojlsixlh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/geczbnnuw.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/ggixgxuyq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gtuvhshet.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grfjtcenk.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gowuwmzpl.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gfcrgnusm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqzidxsiy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmbrrflxc.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gguwnbtlm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gnnmuqdrm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvhuqqfcf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gkquqomhd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gaiwsouji.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ggjjkfhht.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gsuoaszaq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/giguoobdd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gnsbkrftd.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gmoxbikpd.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gwbgwhrin.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gstocnupy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gjfjqnqww.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gztuqbmtr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpejfdpcm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gkieynaxv.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gvnbipbpi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/grsaiuiew.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/ggfcdzkzd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gkaewlapy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gejfnrhzn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gzsnaeblv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/guqfkqnga.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gzzpfotrd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gfgsojhyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gsdyofjyk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gyihksrhj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gobjmnsoq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gkmkbnlym.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gkcrbtvas.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gvqpijzrc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gzwsiqaiw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/glkyvqjbp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/glxnnwlpa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gtpjngagw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gxhsjfkap.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjapgtzhb.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/ggkycrpco.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gubgyzhix.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gjiirvfeg.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gayhmduuf.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gbzroxsmf.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gtkudmzpp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/glgtoacvx.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/grwmulgcq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gxrsbigjn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnpmspwky.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gptlkymzm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxvdptnpe.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfpdpskrs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gzxhcajkb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/glwsnkizv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gxfmtfijw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gehgonkmm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gcvbtjhct.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gmputpytb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gbwnpzhbl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmwdxpncm.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gjdtghbah.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/giqbuarxq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gzsrudafi.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/giztwhitu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gjqwnpqpr.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ggtfaxriy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gmojngtyw.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsqhemokf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghyecdkdj.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gtyyerzkj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gkcbbuylz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gaknabatt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjsmlagkc.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gbdehfokf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/grpliyxxr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gvcslmbbz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gbiplwucc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gyyrkkdqr.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gkygzgfcd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/ghvqnqxwp.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/ggyvxgsuh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gwdpzqdvz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gtgibfcoo.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gstwezepu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gxiquvjcs.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfdjhifjc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnldfnxsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gneweinic.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxriayusp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gjrrfhufv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/goxznuove.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gsbwadvyg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/giekqksfa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gtxrnjjki.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gpypjyzdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gcdenralr.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gykyrkruk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gpbaucxjy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/guiggbqxh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfthmjeoi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcsyzelmc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqdospfzc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gztmunqtm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsglegkku.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ghxycoqpe.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwlsibmba.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gxdhemkpc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/glcxrdxgd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gjwucdfos.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gxickooec.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/guqxtzsli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gefxvwugr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gclsvauam.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gounhhkxu.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/galupppzy.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gfincdcvp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/glbtmsgxf.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkgnlaleq.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdkoiusgc.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gnjlwkitn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gldiybcii.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gcgjrdtjw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gokqpgmmy.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ggjtnbwcx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gfktgzwqk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gdyuuweud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwqnnxsfy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gwrddguqt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gwqeipdzw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gukznogmn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gylzrlmnf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/grhxjowth.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gvytbsmmu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gvkqnaafd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gygnucqyj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gijokipqn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gaubjanru.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gjrpodsea.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkdircyra.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gozlzjbpj.sHtML


<!-- 参考信息 -->