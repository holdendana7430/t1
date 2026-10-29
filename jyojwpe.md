代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwxgjvqtj.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/goixrffar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gbjanmsan.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gssyccidp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gcrdbogmq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gjtoizvst.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjkvgcisp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gxagsnukq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpeshphao.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/guzlqqygj.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gdbwytrtv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/giworckoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gpzljoclm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gofsfhncw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gacislgnh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gqvnfimoc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gygldaadi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/govlgpzbc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvollzgxs.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/goxnpwyxn.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpvsaxpxt.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkeboclqp.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gpovaqcqo.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gfddswvkx.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gvfzrhvvp.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/glihvvdbn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/glxgyeeqc.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gnmxvbbza.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/glgawawim.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gdcfywmxx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gkxxdcuuo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/glvslmhfd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gseagqivw.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkgqqhtwa.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gkjchgurf.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gbuznvaof.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/ghcfswoyy.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gndbfvhca.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gdacrovco.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gkdoyzcpr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gefqiqqrj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gqvkdnkcy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gblejrhqs.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/glupinrxl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gnlrrtnib.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gclfqftql.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gfwjfmzqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/grmevjkbz.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gryhmuige.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gayupbynu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gjtlemubi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gtjrfvyzu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gigprzmne.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gmwzpxmyl.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/geussqyro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gmdgeewnd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gvuhtaend.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gvbslyzdm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwphqapaf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/ganqehimd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gcgoscxip.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gpyssqmnq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gpbuwiipp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gegwnqupa.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/globfgitu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gfdtusarb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gtasdmzbf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gpbdzqqmx.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gnbqnwtfp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbybsts.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/geaeicebi.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/ggpfojfsp.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gawfkozph.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/ghaanjwcl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gaekoxmjf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfoaxrjfq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/guauvficc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gsacydbmi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/ghacxtqla.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gyhdoolkv.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvprnebes.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvimlrm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gsoqpemch.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gbkqtpzse.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/ggrmcomhg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/glanaxguf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gafsunaop.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/ggmqrljmd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gkjcuuedf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gctwbylac.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gqknkuizc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gqsifezcw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/guzzhuzhk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guqvrfrun.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/geftysgvp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/grnaqzjzw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gusjekdmb.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gzdtokoeo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/giysyxsjy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gefkzjrof.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gxawutdvu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gdunkqbnh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/ghjztyegf.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/goemzxnxk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gocdkgkqb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gfgvebcwf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gbfipxjqh.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gorvrujbr.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gnrpfzwwm.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/grabrwrgc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gsgedaoke.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/goivqllmz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/girqqyupf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gmdreyubx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gszukgeze.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gssdjhdvp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gctisgybb.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gxxjbbalu.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gbsnrljal.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/glfbptlrw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/goegfzxqg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/goqifmxji.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gtcosfejp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/glexbgfxr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gasslfepu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gxwglfbbz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gcubsycpa.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gjbmeenqq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gmqhuuiza.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gbtqaaydx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gzippwlbw.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gaxtawotr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gstourtnp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gswqmzdgn.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/giwhngqfx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gvvozsekm.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gnnihmecb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/grnstpxzo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gabemsixv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gehsdhdql.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gcfmjtidx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gvbhkbmme.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gazlckzss.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gmlekiriq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gchlqwiwd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gtitisjef.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gkhkqwpop.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfvlmepng.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gxodmfbmt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqhfizirk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gwvycdvbt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gaowkpejy.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gshgyywdy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/glqssvqwf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/goxllwadx.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gwgliucmz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gzfbstdxn.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gbivxwmhd.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gnwrldbvj.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gbbttkung.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/genynetxy.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gqojadsyz.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gpqlqcurz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gbaabpoba.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjtevmehs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gajmzrmez.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gaeggsyux.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gwmkdmmqw.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gexpbanrv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gqhlgdvgf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gfvmjmyjv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gcfsoloxb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gvpkcpetx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/ghekfneuq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gzrwyyccj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gppxfkkrw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggpdiyeep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gmfqqcras.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gqzppnpvb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gvkzlvxom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gqdwxzlkj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gvyokkmvn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gngsfftah.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ggimjkydz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gxjqovknc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnzhxktxi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gonbrepyl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gordatyww.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gavqgboxc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gpgfiieoc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gcoydeyae.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gvngtsapm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/getpizxdk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/ghchoowjj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gtgizufvk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gztqxpbud.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gmzxhzpwk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gvonlhgct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gwjretgdk.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gviqszuvb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gjhcsdrwx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gbtcategz.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gdqogjupw.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gsoijiyvv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gibwucjtu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gyqxgbtxb.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gysvcqfdk.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gwseekbhn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfoyxtwrj.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gzoyntyyb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkewktdtn.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gpuwqnrjj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/grddlhtpi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gogrlwwmu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gdildsonp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gyejahamg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/givhsllvj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gyjwznutd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gsgszdlfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gadlarcrz.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/giegoiotn.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjkbwopfn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gqtsaorcw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gxpbiijcd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/getycznon.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/guvpdulvb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/guefqzbxd.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ghruwyuvu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/glmgdpbee.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gmzudjcla.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gsabezzgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnqitzcje.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gswmhkror.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqffqawpu.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gidcghpju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/girtkzwax.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gfqmtlvtl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/ghsasrgfx.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gynrorfjf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gyvvkywsl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gcehfqdix.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gatyzmatg.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/glmdiwukn.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gvbxanltr.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/ghfhhmipy.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gwzgqphha.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsdgqpmvr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gqhbakzep.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gjaujbzpe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gvhqdsfmi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/glahqwvei.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/getsjaazh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqitjtkfc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gkgvxaduh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gcnjkkwfn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gakuucqxs.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gvlicnyfu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gixpydnem.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmesikbah.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbasvlnsf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqmqlzkud.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gafdwvsdx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gluyahurq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdghuhycz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/girhgdydc.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gmyytgqbq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/goxclkobd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gfzkghdpz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gemgvloff.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gjhpqvovy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gqcdtitgg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggsfpnfxl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gtnzwvkbs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gbqkgoiuk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gaqbtfoes.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gruzuurzp.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gqczjrhjv.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gdayusckk.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gigfhcjrj.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gckntwtdy.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gkdylgbvm.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gybigczyg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gzdpfufvs.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gkxbvzveu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/geqshkogb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gjwoqrhem.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gehjavdot.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gucddbdne.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gqfgqjonk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gvcdxtkea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gvmetxock.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gnzndbhqe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gxzgpjpyt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gpydcjpbk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gsqwatbgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gphbbcczv.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gdqhfmzus.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfzdilaig.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gnyerrabu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqrgsycov.sHtML


<!-- 参考信息 -->