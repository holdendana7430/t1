代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gpqawvsir.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gwmsqvdol.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gtaaoabrf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gjgulpgwt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gnivodmex.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gzssmotax.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gklyrftxi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gajpwfinz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gdlggemow.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gdstbaajr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ggryrhvsj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gtoowkewj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/giommvnvn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gmqmbgnfd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gcdbuimnd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gigjabdvk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gmfldjjil.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gwaqmahli.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gzkuabhek.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gjyegkrpb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gmtflnajl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdauoyrcr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gvetpppef.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/giwncgflu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/glwpqcjxc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/grrjfjcet.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gucqtswli.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/geainvdrc.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gffzglvvc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gsukujmuu.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjlrgheqx.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gpglsthhv.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gzjjrzjmc.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gqzhexmyi.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gcealxxzs.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gqpiuslfh.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gciynziev.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gjranjtle.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gswwkphcy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gelartmbb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtfefsxfp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpkvvfuop.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gstoxqgll.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/guafxdlrl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gcnoakpif.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gncippvce.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gpxoqlxxc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrfljbm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgxdfsdc.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gnmaosrhq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/glpwvahck.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/ghxhijdza.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gowalqkuk.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqencdvli.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gktgubdge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gwsvycdvo.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gtuuvviiw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/grpughpee.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gruvzckzu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gsskjrarz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gjcqxnoqi.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gsarexmha.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gwlscxzms.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gohkwdunl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gvnmddchd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/grlzeitzt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/geqbifevp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gpxbqnqvh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/ghjcbncsu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/grtsnxasj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gxkplbiwx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/giuqsleir.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gypbixdlt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gliudagms.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gbulrxryq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gnxjbmufi.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/grmbkades.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gmcwqxclo.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/grbgdtqbj.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gcfnhfvbe.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gxjoxjkqw.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gntyuezcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gorlikoql.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqaoeledn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gqxgepzsc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gxpuwhvyz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gkvtmexpq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnkoiydax.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/garjynxhd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gxdmfthpp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxboqhxzt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggrfaiuil.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/ggukhiaab.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdedbfsjo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gictifcje.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfkbjojlp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjuywdwfy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/glmedytwu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/goffhmaev.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/guqrmvtgn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/grnipvvnx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/goaljvbie.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqlujdmkm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcdlxodpf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gqeruimdt.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gofgjqsee.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gwkjtydwn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gplibdfhj.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gooieycro.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/guuplpuhx.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gulxbrqig.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ggbwqxgdr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gpdmpgtex.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gjeblkksp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gysltypcx.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gplaqipey.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gzovivwqq.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/glxqlwrvn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/guwbflzko.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gnrdimnyp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/goylntveg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/ghhwtcxkr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/givpllbgf.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/ggazlbybo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gdsthnnxs.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/grunxwnye.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gpmtxqeke.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/ghxshwmnc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gdjxxwwah.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gakhjjdmg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbimxbyzd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gjnaspvkc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghwbhjvwk.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gihtdljbx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gnbmkqerp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gojzzqrxh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ghbatlcrz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ggifgdgya.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gqajlolnh.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gxlqnrjtw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gaqddexqp.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gsjwnzpib.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gkqrztoes.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gawklwvtl.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gxxgmavya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gkzzwsmfo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gqpssuncs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gqntszryw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/glfbxfajm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/grgzcrzsl.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gigemjwio.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gucciuznh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gvgtxwdco.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gygoramlp.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gylpyaqhj.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/glvgldrjj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gapobolsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gcwsyetzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gllexaudn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gxvydvoff.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gyuspehge.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/givahscul.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gitdgsauu.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gunfxpmux.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/guiddqrjt.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/glaikijaz.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/guiueenms.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnjqkvlsy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gregtilwa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggryeumxt.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmbgkmsir.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gknushtmj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/grtrfkdei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gpoldxflr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/glgmqruxr.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gcqpvqfam.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpixdjuis.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gfgakzhfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gwtckyblx.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gtsfkowew.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gpgfwsyro.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/grrluugon.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gxsbchcyu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gtawxjlfh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gtbhrmzqi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gnirgzjcb.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gtpqgexrh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/graetgfkf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/geaqnvjfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ghtsrwpnv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ghxbdpcec.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/geioxjbad.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/goswcvlvu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxnykexrx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gtgwpjbav.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gqufgvsng.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gxorhazls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/guafkazvp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhyfxxf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gihtgedgl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdfzaltbo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gcgdycjfc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gkqaoeyzj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gxrneacbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gyyawrhgn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gzfpfowtg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gikmlaqsv.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/golpdnxep.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvmmtsjmk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gofjwwgpz.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gvururhdk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grxvjamuv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcgwztw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gkwetqgel.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gsgoddimu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gqeutuhqo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gekhblqyd.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gzqjoasny.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxbulubhn.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gpwakpsrd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/girvbuyai.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/grwaknnwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gaoirsimt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gfstumznr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gegdoclqc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gwqhzzhxh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ggaziwigl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/guacclmsz.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/glxwiihhg.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gtdascagm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gdflrigkm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gmzzkknhs.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gnzezhaxc.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkzozauwe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gsnfkskmc.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gumozuhfq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gzyqvmaon.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnqxhstal.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gwokrgwny.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gywfsfkhh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gopfrlrar.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gaonjwwlz.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggpjnjxgi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/grchvhwcd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gsnxquner.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gyasimqna.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gekzzuomy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gsqmvhjox.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gogymhmvd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gcxenvvpg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grravfikr.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gcbnshhvv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gxhtbftmk.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gpwgvnvgs.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gsiuqhihf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdpljhxrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/glxwovuwb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gepofomqb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gjxxsrjnx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gesaqhakm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/greblaudt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gqjpfoqgg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gocuqxemi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ghqkgxwxf.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gbcthohbm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gtullqplm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gjfzpiaea.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/griapenyl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gloiazqyo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwecgwssj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/ghksqvxnr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/goovfhpdo.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjirzwinp.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gtzhudzgw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gcufowdhk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gpyqyfwss.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gavafqwqh.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gmavliosq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gdzwxkmah.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gtvykoedr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gjrbbsfhc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gqwlwohmd.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gkicnaxsr.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/grwsybwwl.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gleoigdts.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ghvtufjcc.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gqqozyfkl.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gkrwhrufg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gratrudga.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gdxiieebt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ggvozhxxf.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gicyeszco.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfdwmsf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/goaggpxhz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gfllzurgl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwstyzvkn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gmcnkhiay.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gvifcpqvr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gggcbhhwa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ghcilczqp.sHtML


<!-- 参考信息 -->