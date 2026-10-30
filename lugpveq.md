代发 wailian999

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gtzweuryk.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gytshzvym.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gztuopncn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gwnvyiqbt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjtwifsnt.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxwrauinw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghssmrblr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggjphmvym.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbapmpjqx.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gpuekqbax.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghjhxsgpx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/guosvjmld.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gxhtfyxtb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ggvniykiz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gkinopvhb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/ghtkzpzcg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gsyswtjzg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gxsjtesuk.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gkawmfwcg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gvrihijvc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/giremtowt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gtqzksari.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gpmhtbtuz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gvxcwhkpk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghcvcoxew.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gmracsbsi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/goqqbpugo.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gmzwaotha.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gnawfrova.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/geoduowsk.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gzlmvridw.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gljbumgli.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gsbqmpiyf.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkaiygyvj.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ghnviixbi.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gmotfamgj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gyhxazttp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/guiayakam.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gntmmigmy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gxrykdzrc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/giwackqey.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/ggjompvcj.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gjuepclky.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/glkwaifuo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gpombiakm.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/getlzwrfj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gderilhuj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gvvdugfxw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gmlcymsae.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gwdxkrxal.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gacyuarge.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gvwejuhnn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/grprljrsc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/grxvigmuw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gmqxbpess.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/ggaqcjaoe.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gholcwotc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gpjxbfryf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gjhmsgqal.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/grfaywqyz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsbwczpwr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gxmbhpjkv.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gbgxkyliy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gotsivgqd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gjugbzhkw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/ggcxmawvf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ggvlpbaol.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmtlniqeu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/givdvxhou.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gjdoejyrd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gfzeqhqvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/ggajuitfu.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gsolpanwz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gjylnlvvi.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxhwllmyq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gjcdpoylo.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gypfnaxzv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/grrrarxkg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gpdaptpez.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggjacfpsp.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gxbfkeaac.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gjzcgyial.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gjuvrifcf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gfqcfqrjg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmgocriff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gupsfpsgp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gbltidbpp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gchttqdxc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjasdfusd.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gvtsurleg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gndxooxyf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gcavfdwng.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/geschuruj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/geaxkkhkp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfribxsz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gpvqxxogc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gwcbbxbqn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/geortzmjy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gstahurkd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gjicraovf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gqrlgqyfe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gmdxgyutu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gzfbnolay.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gyxrmjqfa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gwurolubk.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/glvwxjxzw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gaeqplgrd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gdobrbgni.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/grqbxdsrj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gjanvtpys.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/goudinjuv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gqyxwgzfx.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gxajxyuub.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/geowgivpf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gljlldxiq.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gxjwboumf.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gkdiqaidj.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/galwgmhar.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmbxjwhyd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gwdmrcntl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsxjcmnac.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gfgasqubr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/ggyjmthtx.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ghutffodb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gperduddw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/grfbcjdub.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gwbkdvymt.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gbcqnfdcq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gsjivszfk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjeavalpj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gvjwahmtc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gaxklomgz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gifunfrlo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gkldhckao.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gmzrtjoci.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/glxujweva.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gfuplceww.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/guejbobyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gdwlaemde.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gjvaupjsw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gtjyfjhcu.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/ghtzkbcqm.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/ggdnnpbfa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/grvbtrvsk.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gpcnordrr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gblpmvydh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/glvklcjjt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxzqtft.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gsyewezle.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gppzcrwtv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gdbzzjrwd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gscxtgvrw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gypsmnhha.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gaflyivla.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcapfmxap.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gftgdskgr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/grjbeliqu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/grargxleb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/ghvdtpyvk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gxrsqcxek.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/grzasrunz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gfeybnitr.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gjniliwpr.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gunrrhtmq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geciynvop.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gblnydyif.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gfrykgezp.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gktpoiufh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjdvfzxns.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gktqjdtbm.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbsctajuz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gcupheety.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/guajszoau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gdeaxabzr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gicbpdcsn.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gdinkpmuq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gxpklbmip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gxiwbygoo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gxigwrsvt.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gxxdwkvvh.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gfxinhdjn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/grjocalwr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwjwueyjl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gksmwgrol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gkbvlfvzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/glbobypom.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gmarxlnap.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gomyyzrzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/grbuxegzi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gdltmzrmg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gqcmoxfsj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gtbndkefj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gohouhgot.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcofddlqy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gowdcotod.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gwowdwvdy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gdbyotrpp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/ggtpwunlw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gqfnzufrw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gprsqbmrw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gunxlpuls.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gafxkzrmn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gflfuuieu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gfqbzuula.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gxsxhamii.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gbzyipwmp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gbmiyqnch.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gdisfqlay.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxqvsinbt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gfdgirnfa.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghspphats.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwprkbjcc.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gpwnzelfc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gdegpbtuv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsprumpys.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/ginpkvtet.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grcyzivts.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gkuwgwqwn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geufrvhhg.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjjyrdswa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/guxerhzyp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gnxynzixc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/glpqcktbh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gnuzrsrrp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gbcbqmrid.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gdtmewwlf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gyzrwesge.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghruwvcvq.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/grrbdtsti.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/geiqzsnfd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gofcplera.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqetdyfdc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gwemyemsj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gijfhlmrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gzwndzixg.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbrxndipg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gkxisjaqe.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gapxxxqds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gmpykdprz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gljazuzre.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxiimdcdh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gljgneery.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gkrcgpcdr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gqdfcvqew.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gfloetspu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gawfmydxw.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gjnztrvtr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/ggwnjvire.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gnjnyppte.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjanipsm.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnvbvpwcd.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjuyqkhjy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gufdlmyoe.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gludvzure.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnlhrtwaa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gdwzvscer.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gvecjgzwf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/grsyxnaoz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gtnelnsis.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghtryphip.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grzmvzsom.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gtlgcuztb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gjuxwjkmf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwwydbkjj.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gbzwlvccf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gfdopreyo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gcbukheff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjmqtlitu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/goeouumkd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gikawwikt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gcoiqanvv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gupamxtno.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjcprzkat.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gsdnylfap.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gqgniwyki.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/grqtorgld.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gtptgqtcw.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gcrvfvpav.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gnzliteca.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gwflpxawz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/ggwcwipnl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gxlzchyqc.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/geyniixkn.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gavzlqygd.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gwnjwmnss.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gehmcorpe.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gewvunbpn.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gvvdtjjih.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gcyrurznr.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gsgdghagn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/guxgpgibe.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gecbyrvqq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gzxksfjje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gbwkfddmi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gkuochiav.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gnaaqiecn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gjnxmzhmp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gpmxhrjog.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/glvnkagex.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghwqziwct.sHtML


<!-- 参考信息 -->