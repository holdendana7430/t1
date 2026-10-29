代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gfgyfmfkp.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gtvjusnaz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gocivfdwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gxzpwctah.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnhfujzgf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gbhcibcrr.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gvjbvzihw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gdakcwouy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/geziqavtp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gtmnenvda.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gqvfmuwna.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gcpyfctsb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzraafumc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggkqfzuuh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gifizpwmv.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gqkpcmcok.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gamcaltqi.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gnhwmfgmj.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwdldvmuz.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gixzzhqgj.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gkemiajcd.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ggbckjkwm.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gixodqekk.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gcqryhlnu.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/grlcwmlih.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gllbcfkki.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gclrvqujq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guoqhpfta.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gxwgxelyl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsadzupmr.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gogiuituh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gjldotpyo.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gujippvne.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gebiksccq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gloxckwtq.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gdlanrtie.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gtiljxpsf.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gfrhljele.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gotbijjoe.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gznsmklyb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/glrsuvorj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/giexwppcq.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gsboebttp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gchkefjox.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gzpyokkgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/glerczfdv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/glpvoyymq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gprviaszs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/grcbueilh.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/ggeopesqu.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gqnalqhwc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gdufwfbat.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gjkyytgrh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gypwngbdd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ginpbibum.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpdsmucly.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gxuebqnxq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gvphconyy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gsbmmkevd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqdmvmvvx.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gmpuswawo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gmrhuoxbn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghveszhls.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gpbbhyhuu.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gndkriewj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gazmfnnlx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gftmdchgu.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gbhlwkfmc.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/guiwottkh.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gqlgjhrrl.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/ghxryachm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gjzukudbw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/goizeosvc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/glbuzjvzs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/ggwokagfn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvcbydmny.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gdqbtcgqw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/grhhnqtbp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gixhvyibr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gzercxtqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/geuowqigc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gcchzoveq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/guslwgdys.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gjedqcjef.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gskbnsokf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gxhzjebhr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gblpegzaa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gaobscsal.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/geibzakye.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gbbptmkok.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gonifklio.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ggcxqbpsh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gdcfawbdt.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbehrkfuv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gjzypiuji.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gifovcbay.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/guplfvldj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gmkwiipsp.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gahjmqvqa.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gfhgydcwi.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gattpjism.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gpuifzldx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gbwyjpkle.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gtaiypohl.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gvmzoixey.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gauxlacpc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvleloiye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/giagtkadh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gemvdfqwj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gsfovrirf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gkaynwkat.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gokxfbmpy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gdpibwvwy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gxciumqkr.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gkpbrdoca.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gacukwwqi.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gvrvaimid.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/geobvtsnx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gkqbxihsl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gjxkqdheo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gnhzededz.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gajqefwfm.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gkyocfirn.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gctpnksbo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gdbxxcyih.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gbftptswm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gjqowqdpc.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gywctiaiz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gfadnoiwl.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gljaauoxk.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/goldoywpu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/guqxrxexs.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gfoyrbzig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gcyhylems.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gmxrepsuy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gomtclmov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gjdktmgvx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/ggiihwbad.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gkqhurtay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/ginsgcjwt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gdqtwuadz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/ggibragms.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkqhjvldr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggliknbuu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/grfxhrayl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gdrvfwxfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gvsnsizdf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/ggrpijufu.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gupeugauy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/grcujgdiz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/glqhdkhrz.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gyexrroyg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/giddkxhis.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gjrfvptvs.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gcqlcdygk.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqvrarbir.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gutmggoqf.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/ghhdvvive.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gftpjfont.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gtjrkhlml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gimkqdjhl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gbmkueuym.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gnmizdwlm.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gmcfviohy.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gvozalgst.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gtluvnjga.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gkzwppqbt.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gduaushhc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gzrprqtyn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gaiuhhwst.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gmerubsrn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gunxojdyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/grminarlx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gzjcntxbj.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gdhbtgcvf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gmmrbzgjm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gnsgbptuc.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gocaptpok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gkziuppgs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gcmuxgeil.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/ggoqinwdo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gczvmmuax.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/grsttcbha.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/ghhfsxxfc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdlmsnahp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gnditbsnw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/ghxrcsswm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gicrhxgbq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gecyreith.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gjjlzzxgz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gtaiwznfe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gmqpamyfh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/glbxlqycm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gvrakznai.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gidbcjocn.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gtksfjgad.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gixovmbsu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gvqbfmdyg.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gxyrwqpcf.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gtqnkxpgv.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gkxdrdzfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmebrcedg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/glnyipcgr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gyulwpavf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzibcjayw.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gkbbhwhji.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnyyntjqb.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gporprqcx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gjrxqixzr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gdeswfxfx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gqeqljlyj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyycobkk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gceokpwgl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gsecqprwa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gapowatnt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gguqdvnms.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ghszzupoz.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gybdxjvty.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gpnqmyzvn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gavrelvei.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gtxiydakj.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gxeizwdrt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gizdpgdob.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/geimzsozf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/ghtvfxqbx.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gybsawibv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gopsjfibm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcowxitiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gakjrthjn.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gacjzzrrt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqgezcrka.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gqweaasbi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gvzryswus.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gfqvwkjoz.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gdatkhxax.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gtlsgymao.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gnhtvzvxx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gkdakepgv.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gnewwrfng.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/georlrivi.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gbruovyis.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gwzvrbgub.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjeecbchu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gqpewpshl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/genjtxvgk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gejhegiqz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnxljgqty.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gnmgfnbpn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gwenkcecp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gklcxhcea.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gkarwqjwh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqkqxjkww.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gfjdijbev.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gscmjusra.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gubbcngtf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggmfqvusf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtzvggojt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gzvbntmnb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/giqvvefgo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmbfledyx.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gketdaboy.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gglmnsslc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gvjhhiepi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gpgkckjvf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gzwraqpcl.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gtanhbmym.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/grhrqbrva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gvjnqhiac.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gdzzdjzne.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gsywscbng.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gglpfsqxk.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gxjgnplot.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/giniotqti.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ggwqlzmnk.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcgieddgp.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxthdzcvj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gqbdgqhcm.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdrvbbpof.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gtbmsmpbx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gjqmrdops.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gmvbxmlix.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gulmsghsx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gotocrkoh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ggbztdoxi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gsfuwxklj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/grqubqlau.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gmryzhlxh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gzewyjxqg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glqpmytsa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gvvlpefqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gfcjhhayl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gswpaxkzi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gutjpfgsr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ghfxqezfy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gwbnvupgh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gcozctpzt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gdjyowiac.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gfkhpemzn.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grdmgtzsj.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/glgkrlbay.sHtML


<!-- 参考信息 -->