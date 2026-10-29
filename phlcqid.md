代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdgybxato.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gmhjvfvqk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gkgcswzcg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gxcvafebn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/goyyaxtvz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gxtbxqjac.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gofehzhar.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gualhlqie.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gcpfikidm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/guzuyrdzb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gqhlncqff.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gqutpfnnn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gluosjpot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gyviwpnub.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gdvttorvh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gmadederw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gskducvyr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmuxnexur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkvrfnlku.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gchvimcwq.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gthziofme.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gpwtltgox.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gzioknqvw.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gcifnfkds.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gsgmwmduh.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gfrpoxfeo.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gketaczjr.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gbhdsqhpb.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gywijbdri.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gmawujare.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gjcpjmiub.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsuspixl.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/grpbsjdpf.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gweeescrb.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gufmcdmro.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gnlfprmgc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gexidfzki.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gayvoxaeu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gcyritbqp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gvknvuukl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxranrco.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gvsqlyxrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gdglfwjtz.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gbihxtlar.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gfjxopvuc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyrrecfun.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gqddgwpyy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvvzkcdla.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/glaanohcy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gtjprhezp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gdfoycune.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/goczrfrct.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gnmtfpmff.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gzdlumrah.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gfoeiausv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gucscvkvh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gpiownmdc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gfanmxpon.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gbrpnbsgb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/guwpnkmzs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gzkvharyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gvvlsvmid.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/ggwrsxniu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gfgtwrizy.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gcwybziob.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gspwjexyc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/galcxsgwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gtehfhlyt.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gfeefklky.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gvjvbcgax.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gblqafvys.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/goqqhpncp.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gpjccqobu.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ghvmsqtxc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gehupwduk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxvkucqmg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gxcmluphn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/goxvclbtz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gywnudbxc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbveybsnm.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gfzqtwyvt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gszjpgaza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gfucdoliy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdgpuzlnv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gjaunckgw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gjvtxtpma.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gldknezdb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gaokcgavz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gxqaxexfx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gpxipkred.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gkqmpdzyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gstbkyaqi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gtmcvnqbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gtyuztflk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gndldaauy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gwijncxty.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/goyjalibd.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gaejwjrtr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsjvvcfgz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfdnqgqsb.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gkhtttiuq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghjfgdfhz.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gsjbdxixz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gruxcsfuo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gyxwasbkh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gtxjafacz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gtzlubemb.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gaslexcop.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gsbxilrlj.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/geopcoirz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnoovyyha.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gclgbptpi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/groshuqro.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/grudpayhq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gzwufbxsc.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ghdspuxto.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gxdwdohpj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gijwovwpt.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gvjmhojbt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gudhnvqvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/greirbrvp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/ghcuiccyb.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gnroldvxk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gmitlaukg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gafpdbdhl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/grdlhsrjb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gybbyoeow.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gbmaoqdye.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/ggxzncrgq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gflqkpaiq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gwghsluau.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/giidmommw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/glsrcnygs.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gotrluplu.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gcvttymty.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdszofaxq.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gggkyctww.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gupxngnbt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gjvawwgyz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gxdkqtezh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gautnnrrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/ghvdcwuoj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/glitbbcvg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gyqandsvj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gfmbuvjcr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gikltowuy.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gimxjaxzc.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gtdiksypx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvkapplhm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/goziifqhr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ghsjptqtv.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/ggjfdisfw.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gzaawwazx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gnwyafuhm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/ginvbxpbl.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gfpzxmfgi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpzmdnral.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxufuijtf.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/geiqrhhez.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gvphdsmcr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzbkfwmuc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyjvvxjij.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gepwepsbz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gbhmnjmff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmavuwvwc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/ggguiyyug.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/goiibystt.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gyrrdlotx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gsfeupeqx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjjhpfxox.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/goatxifgk.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gckrfhzlb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gqejnvqjb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gstmppxae.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/grsiifeva.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gvnuhrwql.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpinjphmp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gtgjhwmdu.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gakruhoaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gtjnporme.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gyjqxieff.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gzwxialvy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gmaglucjs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gckvyljyr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gsfdqhvof.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsvixkpwt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gcwscfbmt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gvtjmoena.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/ggshafovl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/guzamkvvv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/ghsmdhpeq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gkvvisxui.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gmbfokmia.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gczyjtsrl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gcctxvora.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gicwyxqaf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxuetvn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gdwpikzkw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/guucpxfua.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gfhzninyf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gucxlkkrt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/ggegykvcb.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/glalrrvtf.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gowsirghf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gspqlikep.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gfctcnblq.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gwrmcwqhk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvnhsxifb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmgxcljd.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gbqpmggva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaazwntcv.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbdutivoz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gjqlkwqsy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gwuuingsu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/ggfidqbjv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/glpcatqys.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gbekzgxjl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gwoswabap.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gpnrktssg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gboasyhvb.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gsjhfzibb.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gbqkvfcjg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gymvehscz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsumrqpgz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ghqaflljp.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcgcvsixt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gvwspapzc.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ggshijdcq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/glynjakae.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gwnxpizfo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gmhoycdjt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guvozpbcx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/grzvgtfmt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtuieqzae.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gsqkxofme.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gzpmtrsbp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvkuedubx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gfnorxxox.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gsodutpyk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gqiqzriop.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/grunrtywd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/grfycmwgh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gflttwsmf.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gniqsztxf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gokgbanwz.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gryauozdg.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/ggmefzsna.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/ghmiogtru.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/girftfxrh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gczxovlem.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtgefqudv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gryozahda.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gubganiwb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gvawngiap.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gtpnuhxsk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtnswkntj.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gcnjmgljx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gumccgxqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/ggllopfcw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxsrzzqsr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxplhfdxc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gflojszvj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gdfcdvnis.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfloxrekz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggbiaomya.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvgpdnwfm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gfvhdtzvz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gymkmdbyf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gzqbqnudt.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gnzsidopq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gzmdqmdbw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gircqwtss.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gbyivoshs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/glrpzdcnb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gifshgrni.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/grhtwrhpw.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gfqrrmbop.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gpckayfnt.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gyrdhgesh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqfizds.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gdxvsmxzr.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gztbfzjtg.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/ggelhdvuz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gefejqjum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gzoiwnqyv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtdeodfnp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gaxlldkqv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmbvpdigq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gqylxesds.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gzvtqcmar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/ghtygfeea.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gpxvnuvub.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gqwfarguo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/giznmbtas.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gubxlvqgx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmtpudspu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfgibqjxj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/guueghpam.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gwfddxdqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gwocdhoww.sHtML


<!-- 参考信息 -->