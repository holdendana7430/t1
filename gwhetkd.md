代发 wailian999

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gqgevjchq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gswvowezy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/ggflukzkt.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggicrdspt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gtuonvari.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gldshwrov.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gnvimebkh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gsypjypvr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gljdyrbvo.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/glbbkwmnm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/goxtlyumq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gtmpyemog.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gnuvkbcdu.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gwcghckyg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gwbiopvaq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbknhkchy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gufmmemcd.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gcoovthhl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/guycmboyd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gqsyqsxvc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gdukvppuh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gohvitzuk.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gapphtztx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/goyyhlrct.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gnvwvdeur.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gkxxbnixi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gcsnuqzuo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gszabgfkg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdfzvgwxt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gstodwpmg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gvgboadfn.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/glfyrdbtf.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdnwtacdm.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghfnmgfyy.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gnxkvledy.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gadhracgy.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gelrpvocg.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsabrqudb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ggsiespuv.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gjkbalolh.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gfwehcgsk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/ghuonjaci.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/ghseajcgd.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gzzqpjuai.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gptzkfler.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcmnubzzg.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gveubrecf.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdtpiucrs.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gqhcnooti.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gvtjkkyes.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/godeseatw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gekraeqhi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gkringpuj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gfmabidan.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzyywiwyt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gmplnudks.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gywsnlcar.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gijjnbnco.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gyofqeyat.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/giwyoafxx.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gwqfvzgml.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/glvpcsidy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gmiwvjbhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gungfrpbu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/guoqxjlih.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gkfoubnre.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/ghujxtxux.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/glwxhmvim.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/glqljjwrf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfxdpgnxc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gvnwkmwwj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqnxtem.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gjdrhgmnz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gixvesjwc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gxkkzvhud.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gnnckzvzi.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gorcnzjjj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gjhcaelwd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gmkzppogx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gzwygvkhv.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gudajtnzg.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gvmjxorvb.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gtcvxwcku.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gmmdczgsa.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gavgwkjay.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ggfwsciwb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gasmuzhqu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grogxkatq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqmhgigtk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ghdxvozsd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gbxwrtklb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmurxhdow.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gvkmjyyon.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gvpskbmws.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gtcvxuoxj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbgmdjhys.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gawddxkbj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/giecytjic.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/goqsmymfe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gureitdco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/ghvxoginj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gmtkierue.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gbwhebehn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/grkukhorz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/ghjcqgosk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gopeekrwo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gqqrktjrg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gsaukzbez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/ghumddhzq.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gomkvckme.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gausnqckx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/glkcibfuo.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gykmzuoyj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gobywuyrs.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/ggmojqost.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gctcchttx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpnzequdt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gxbrojxnm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/ghisuabtd.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gwyiflxcv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gyibowhwf.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gktvzpxfa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gbkxuqxhi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/guxflregp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/grsovkoic.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gputpedsb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gijcrvxih.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gggbhntox.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gehpktadn.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/glpnlxymc.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gqezrvmiz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gqfylcdex.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gdzukudsc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/glxhayxyx.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gpkhahmze.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gxhasjknh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcceniwss.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gperotvlb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/grkvfpbtq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gkvcruuji.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gaxepmuuz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gqgykjnem.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gkjzysend.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gtlatbnzv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gzpawolli.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gylmoujnf.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/goreufjde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gfjqfhhwc.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gcusigkel.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gmoixdvmx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gjvjeuuat.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gxxtqhaut.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghlfdbarx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gkrkflgze.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gptneakrc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gexdabpyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/ginsybkko.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gcmygwzlh.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gtndpmiyd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grhanjkjw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gnsymicae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gjbfhhprz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzyexhsqk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gvbtiridp.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/glfebhpsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gmxtrhyha.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gjuqyxdxm.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gvapewzjb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gjkquszqh.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gidcgpiti.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gyssvmudw.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gyidmddfn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gvgpkavsb.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/guxbafugd.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gokfjdqqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gommfnqoi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzmanjzfd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gdocwvoom.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gqrhlwhgx.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gprfyhwmi.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/goxtrfikc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gqnfwedfh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/grkhitymz.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gxpcwxofw.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gkofpdvqt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtwrxveth.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gaewwijqo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnzluzbnz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gvmbfdago.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/glznfmkzo.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gpczhaazg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gnshxbddk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gwowamvof.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gopuvogqq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/guidmoveh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gmtihwxua.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/ginolxgzw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ginfmbzgw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gtncnvvbn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gcyuzsiqd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gzwrziyxk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gefvwnpcp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gfcalrvxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gyuoydswo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gxornpsyr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/ggouaygyf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gmmznmzdw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gzjlmwnzl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gjxtycznu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gqznjeqva.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gzbcbcrly.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvfjqxehh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/galbxoazg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gjdxxvszh.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmzgqwfpp.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gggvvvhbx.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gocmlxyke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gdqwaszid.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gtjbweznt.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gmnverzcn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/graeumgkx.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gygaihrzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gouaraghn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvllddrkn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqlhund.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gbzasncny.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glwagcmqh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gelrseufh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gzzlykctu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gpovecvgv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gekzsbnam.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfbgmreos.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gkkjnqrjx.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/getrqpmto.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gjyebqtkw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfyvnkjgf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gvgsgsdiu.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjwujlsnh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gacomozcp.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gglfpzoiu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqxzqwi.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/grokqtwte.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gpbqggffi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwiuplzgz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gneysusof.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gdktovyjd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqnghbxak.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gfxejomop.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gwfkrpdde.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gpvfxahhp.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gokowitmw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvnrnbwan.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gudrswpek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gdfdktsre.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gfmbvuoby.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gbnzszxmy.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gibvvvunx.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gcfftdreh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/govunujeh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gzsoepzib.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gzndzioiw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gpnlhgduk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ggjztheig.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gqajkdyft.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gngcssgyf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gwqxwsimw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gxvxwmqud.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpaiuvzsh.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gljdwjbwq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gltttudmb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ggnjbpzif.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gudfbuyep.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gestwwunj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gecxzgqvu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ghveomplb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gqutdyaaa.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwhgpxedu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gvdukifkg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gntfksgxs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gucagnszl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gwazngecj.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/govepxfmy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/ghwdkadta.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gcfshpzvj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/giogmhhfk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gnaprcubt.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gtasccolp.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gzvnpxrhu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gjjjlqdfi.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ghbpushbo.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gpztvngwi.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gqvczsvqd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gjdvzutca.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjlazsrrx.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gozvhvfpm.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/geurvjdmu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gywsqaipv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gqgigiqeb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/grdouukvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gewjtxsdl.sHtML


<!-- 参考信息 -->