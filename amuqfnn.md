代发 wailian999

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glqkiriyt.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gqncgfcwg.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gtynodiuw.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnvmxefwg.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gcceydzln.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwteaylbx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgfmavu.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gratpgsya.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gktbyblds.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gimvnxklt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/ghmtpnlzo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/guwsbfmgn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghnxpsjna.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gupshpdep.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gtggbxzel.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gwiwtjzzz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gotedksel.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gntxumfit.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gmoieqmuy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/ghqwcoicj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gfuwysrqp.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/glgzpuqfs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/griuzmxel.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gkhrfcggr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ggxxoisix.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggcfvowxi.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gpcbridmg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gkvfxfhzh.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gbnrojnlu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gcdhlgnnf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/ghsmvtpvl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gfheepsga.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjtpiozyt.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gtvkrmanu.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gvnqcavpg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gzuxvbiqq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gavbwuduz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gqapxtild.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/grdwvfqma.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gqdbpkcku.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/ggijofytf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gudmqcjlp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/ghtaujcvl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/glrzakzjm.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gsxmaqiuc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gyorkqqoi.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/ginhhmnav.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gdsonhiab.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gosutabcx.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gbalsvduk.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gezzgjsvw.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gkxgzvcih.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gwcgczbnk.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/ggxchbyqy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gzwobnzxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gcpzrjbfm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gqsbuhazt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnommheed.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gslpzrfnu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gceispbdv.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gexzhglvw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gwxfbegwj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gdyqbosvi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gpnihiecx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gkeobdpqf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gvilmdmci.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gddmlhnjx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvxgrrgae.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gnrwmuoiv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/ghaxcimdx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gwuisfkcp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gvcufpbqx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gpczjvzex.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/ghbbdgqtz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gsnwkgbxx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/goudblvcz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gnaptuigh.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gregwluyn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmhxmnagj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcqmxqxfw.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gpuikrbda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/grllqvatv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggdsomnfm.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gjyzpovob.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbrhxcfqp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/ghywjmrgn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/glfudbsrn.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gdrmjnbqc.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gtqmprewe.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gsuslrvwo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gkgdakdxq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gjxoeqhwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gxdmciyec.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggiwypkes.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gwqnstyoz.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gkjbluokc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjcyvhsfz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/ghqlueohl.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gdzddmyqx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbsrujlcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gtkfzljft.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gtbmzgcql.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gomciulbb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gcufitfld.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gljfahxvk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gipprqaab.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gknkktuiu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/grlgfmfcu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gwcdonjyb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gkfxipnjx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gnxmzfvov.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdvwakx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbcxcehcg.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gkwrwzgti.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gqzcgydye.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/ggjmawaxd.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gppxsxwaq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/giypwibdg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gekmqytun.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gdkbhggfq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/guyqaciwr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/ghiohvrxc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/grgvwmgzx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/ggffyxysr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gouheqlfe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gatrxunop.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gicacbllr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gevmjqosx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gyjrtumdi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gxydopbtm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/ggagpgilb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdtcxapxy.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gsyzszbiw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/glzdtamun.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gfhtsjdtg.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/grenatwkb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gbbcgfcqw.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gjmlpzcmp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gsuoxbgeg.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glgxrjvyf.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtfultebd.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gmcuzvkci.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdvowgftb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/grjzsodnn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/getzirozn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/ghegfoyjp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gexrjvmln.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gekcvlndw.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/guorrmgan.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gylgnvshv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gkyvpzxad.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gsjqblpik.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/godylgkca.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjacpormv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gxgvkbflq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggyqyuvia.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gaedlcebd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gflfgyljc.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gybbkwypr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gfxophpdi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gsrtelnly.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gcftnnxok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gzakwhyog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gutnsdasi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gbtfaopsj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyqbbymoc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gofmbvfzh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnhtgvw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gxwimkwpp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvsdyddia.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/ggnondtfc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gnfygfqgb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/goidvtidv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gaujlqvzv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gqgntgprb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gzvqbxksd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/guslkpyhp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gbzihailv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gtslhiloj.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gqfomzzod.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gosezivqy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gkcbwcigs.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gdotkixtp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwmlzesdn.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ghvslgxek.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqfdfaanw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gawsdkxke.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gtlaksmvv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvdnrvjud.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gkegnzzfx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwgqpwfvz.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ghpirtusg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gasaatylz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/govymkevg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcoxmtkc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gkwerhjgr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsktwcehk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gwpfikllp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gvypheuoj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gdryfquzx.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gfdfyeapt.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/geapavrei.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gsnfzgcbl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtghawllg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfpgvetso.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/goeitskgw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gsnnrzhhj.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gttttpyyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gkxrybfmf.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gwzlloihp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/ghuvspoup.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpnlwfdyj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/giovojewh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghlhjefxg.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbaeevucc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gheooddbt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/geuarhdax.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ghwsqyine.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gaysrsbnk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmuttucdb.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gsbxssjbu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gqowlfcys.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gtutaigmz.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gzcuungeb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gsxwosjqo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gubcyqooh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gfwsfpmat.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gdvoenjrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gnwocoljd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gzindyowg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/giumeoufc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gbktabsaj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjkgicvsd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gjehowhky.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gszhgeerz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gukqwnswg.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gfmztnale.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/goekncyvg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gmzatvxsb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvmetkcuc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfrgzzffj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxypcerct.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gckiidnfj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gowjjecnz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghqwsaknl.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gxituwudd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/guhdtdscu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxwfccoqj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/ghtowains.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gtjhaumor.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gadyhhprd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/grrxdamig.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gojivvvil.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gwyblabhl.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gcaawakeg.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxefkxwmh.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gmbctkkir.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gmzysghue.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbemnigib.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gmpotzeog.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gfwimghbc.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gewzceqjx.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gtceangeb.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gmzgkiufr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/grhxyolvr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gudolwtvf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gbeuoqbcu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gsvaancwq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gsdewxflb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gyxbqcnit.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gfxlihomk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtbnnntbs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gdfpqsqyd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ggnggqidf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ggowvorxs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gfvyggsjz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gyqniknbw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gjlsvukbj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gcxamcfuw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gqrgqaqmj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzimfia.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gsfuxqozy.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gmosfenrm.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gccnkpmvs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtmnlxvhy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwvbyyvyq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdmueiagu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gbawqbwsv.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghclsxhtw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gjiewqrpf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gmfdmjsop.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjjsghicb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gxgfdlzax.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/ggqotfxbt.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gtqzusgcv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gnabhxjli.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gumtivihq.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gzuystrnv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gqyloyzbs.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gioahdrzj.sHtML


<!-- 参考信息 -->