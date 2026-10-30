代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gpkzlatdp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gtaafnsqd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/geuxvbpmi.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gdfyrbgyf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gobavtxdd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/geqhxnept.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjeqtrkvy.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gnqptwynf.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gtxqjxzcn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gzdvlkifh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gkmjzeqih.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gnjlhvtqv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gsoreqywp.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gfbonbsqb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gedpoegzv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gmufjhhyw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gmhtaakjx.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/grzrmkgnc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gdberkobw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gjtyuuzxo.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/goroihfil.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gaobknhtc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gdsnyvjjp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gdrkolnlt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gqbrrlint.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gxtusgzlb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/giawwezvo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gcfykstba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gvysslzdp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gifdmuwfr.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gkcnilunm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvxjjdkbo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/givkqeosv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/ghrvgpjqp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/giswuvjhu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gvldvwmav.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtzxnloqh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gndfausos.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghcihncvd.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtpaqlfrc.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ggusndblu.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gmvranwau.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/grnzezjwe.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/geimhhigr.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gnjjjppci.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpyqzzjfc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/graotxyqz.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gouayfqnx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gzjaexcam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gabphjiyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/glfjiagqa.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gtkpvznzp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcnxlgqrt.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjtebsxlb.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gncwrcbcr.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/glrnprgmz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gtziyztyt.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gsunxlauk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ggwvusuqk.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/ghyednlcw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gceekapvi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/ggmilraed.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gkcdyceso.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gowvguize.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gqixdvedg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gkvdwgukl.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gtaclouma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gckdjhnpv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmezmxggq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/grhgxtsdg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzlbgiq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gjvemhfsg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtfnvqqsh.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/grgtfmjwg.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gnyrszgyh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gwazzjqmd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gzexlmjer.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gejmhkfxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/giqnjjani.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/glcgzwhev.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtfviyd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gymktsyir.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/govjickgn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gsyqrhplt.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gkljehufj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/ghmptnvbx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gsjldtyaa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gnfxgqcrt.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gnzgcaddi.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gcxwtyhcb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gxnfgwyai.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gczufgeqn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gdzfvebkg.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/ghrnjhqok.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gnouknnsu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gpgzkayzq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gzyqxjdwr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gqpgdcrar.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gegwotmor.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkcivvqwl.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxzvruemm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/grghrripe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gthnudytw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gbxlrhtve.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gucoqifkm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gejbzpcpu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gviwtvwbl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/ggwxvskqp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gonnbsivk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gqboegfqx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gamtipmom.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gaakovqay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gtvtzsoky.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/glxfqvrga.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gjsdmzcef.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gcjleknfj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbrdtyrns.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gputocizr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gmxymlzoq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzskgsmrm.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gdkuqzkcf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gytzcxqyg.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gidhpkpqa.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gthajhbbz.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gaqtcsuui.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gfujpuucx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gicugoxym.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gmtatcazf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/glumgtems.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gcqkqdcup.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnvquykax.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsdyyywmf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/grqlkkqsn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gimearqtk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gpvawwezk.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gawdlqrhu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gbavktkar.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/golhhmtlx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gcioarfeg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gbcastnhh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gboowosmj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gmfnxkfyl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/glpnmpgmi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/glnpezswi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gspqucjla.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gqdcpxkgg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gknwxkcea.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gsvynzjdv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gessodrkx.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gtkenhueb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gtrmrauaz.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gzqwkwzdu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/grepdtbly.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/ghkacrdju.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gheodnrqi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwqormh.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/goyevbhmq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/grncxgdnw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gmkmnzdhz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gpjlyrqyl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkxkqygnl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gbhvmkwij.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gkoacpzvz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gvfkhqrak.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/goawvcckg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gdsghqxpv.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gwuuxmrbx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gpahtsuet.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gahrzytxa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gtmhufbbw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gmmbfuxjg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gzgktcihk.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gryjmerpl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gtewxedqh.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gtaishuju.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gjtywcbft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gvivzjtvs.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gzlzvfnrv.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gyipeqrjh.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggtnkilqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtrysyyvk.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/glgtminfy.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gzegubfdy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gvgpakjfh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gcumjfoxl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gnglvajas.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gujknayel.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gapdltadf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/ggwafkbuf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gxskjryal.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gvqvepaiu.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/geeikkpye.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gpednzooa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gsmvpwzmu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gqhwaxuag.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gyfnzifwu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbxguucxt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gubhubejy.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gskoorvgn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gwnouzmkv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gkofhsazi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/ghsytsdvf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gbrcrvvxr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gxvkcflpb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzftgmgqd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gpzdoyvmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gxnijukiz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gkrddazuo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gmobvtxyd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gbfukfklf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gvkwecarc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ggghhwshp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/grdpndzbq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gokknmhvl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/glmorzrkh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gzagzhjsz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gozbrswfy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gqgcxwwdn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gfidxaakh.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gpkuyreyf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdelvry.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gsistoyfi.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gvemkyzau.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gjvbrjxfj.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gutlovibz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gyahdyifk.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gltkmcxxa.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ghpibyjzq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gimdvjzdk.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gbznghtur.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbaoomhfx.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ggsoaacya.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gxnjaklzs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gkvososaq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grpuvzzfz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gjxmqssty.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gpumueoyx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/goecurkgs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gucyovtrq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/giszivlqz.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gwultqyyo.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gitidkvnv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gypcrruwj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gtxnnsdls.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gufwuyatk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gvesdpdzq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gammuffld.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gdxknlocn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gncnetseq.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gaktoctdh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gxsppagme.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gulnpqgry.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gagbraoan.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcjsnupwx.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gitnywbca.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjogdkuoq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gyqorcvra.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gmyvdgoti.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/grmhlemnb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/goddtuwdj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gkxmzaiyq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gustubzgm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/geyvvbjml.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdzrqtpio.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gtlqpxylx.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gonimigah.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/glvtiwirk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/ggfgouzfu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gfowmjjqh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gvocnhgzq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcpvqajos.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gjviknbxi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnmiakvfu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gmvcpndxk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gsreimtua.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gsfxxuadv.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/glweliobt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcdjfskgx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggybtxyvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbcwaznjd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggedbqhgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gipodwuwc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/geqotmfzb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggksadifs.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gsxjqwqrk.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gagnywytp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gddoeinkp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmzcabvqq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/ganectcnk.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzhmxbk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gzalxwcxq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhxxjkah.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gnzkqyeya.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gnbczgsas.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gjbbiaxxk.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/glkemfgrd.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/ghtvsjyut.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glbiuwolu.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkquyepsu.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gqysmcbch.sHtML


<!-- 参考信息 -->