代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gqqxxhgzx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ghmzokwsg.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/ggzgkgztz.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gltaqwzoi.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gnwitbihw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gzxcepewp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gebydvvvh.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gmnaghgmh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/glakrqfaz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gaycozwvq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gtjmuocjr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/guygfjuqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gclthfxrj.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfaasopwh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gqnnlnvml.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/genihrtjd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gnjwqayzp.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gnugboulb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gmadxvchw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gbcehclnq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gtlbbqimn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gyhwgblaj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gpooggimj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gzwqsvruj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gzgvafjdj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gcylchjja.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwnuiix.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gxtmlxkpc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gqdjvinhd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxnzgqmwe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gubkpeaim.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqtgzjbaf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gvhunsyoq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmtrdffcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfxozrcoo.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/ghasqyhcf.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/geriocvdd.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjxouncsw.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/guwvchiwz.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gcimivtnd.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gzqkbnksi.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gwsxskdwt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gneoippbk.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/glgshzzzt.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gaqoeaxoq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gniawajpo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gcnqrsliw.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gabxxflgp.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gcdrcoaks.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjxtixnuy.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gjjbfbzll.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gvfdznmlj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjjtotjzx.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gfxpotdxk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gszwpxxtk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/guudkfzhr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gwnqyxqmx.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gaskebxkc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gxtghuise.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gupzgozjo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gnhcolijm.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gokxbnkzm.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gjenqzxor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gmsxebixj.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gghhjcahk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gjoxnthyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gwvtjqwbm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/guvontcnq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmxqenxvc.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/guyovtcyp.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gfdiunhpz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gxeotyqmh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gbzfskgfv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gfxbhbjpy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gjmtgfxib.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gchvkmtaz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/giqrqthwo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gofcafzrx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gcoancnrh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gyhaofbub.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gagenylsr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gkgzugpfr.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gcjcozkwa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gbqynsgux.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/glapjxgwy.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gdmnxslif.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gwbkgwjfd.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gxgvftxbc.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gppfhjghs.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gobmyoxpo.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gqkcijdpq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gxvjmzozk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/geeznubvm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gayqbgplv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gxyfvkzvg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/geczqswod.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/ghrldkent.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gdlggxdjc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gnnzfrilb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gnaeaeyju.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gzviybdzu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/greoelkbu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzsiliqhu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gsudxkghd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gmuttpkve.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/grtqsrsjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gufvchwdi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gsdfuytny.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gvxexgcvi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gbmcvodkb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzmqsitfo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gplwqwgeg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/grzlqjbfl.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gnwlvlzck.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gjeqxcmjt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gqxcqvqhe.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gylqsaulk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/ggudpfjsx.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gwfscytav.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqxojqjwo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gaecplfhk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gsxaoglje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gylcgyapo.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gokngghox.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjycsatzm.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/guoutjsxi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gupyofjzq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdzayewdj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gjtblapdh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gphgsdjhf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/ghegynzwv.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gepcgghae.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gqwygvapv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/graoqmlzq.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gucivwbga.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmaliyqmp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjpgptls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmgitgjey.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gciqtgmqo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gadlfxolj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gobofpefo.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/glywcntig.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbjsjlysz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmbxxgzpz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gsldblcfh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gijucoyah.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gdgjqdvxz.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gtfxqbkgu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrghewjt.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gcpgvczwz.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gukiejpmp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ggqlmvkkr.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmneyypxo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/ghsglwiom.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/ghxkxplry.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gajyjmsvi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gnnzesltw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/ggcrjulez.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gvilcpzfn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gacpkskzn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gstizqzcp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gnnafydrj.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gdsnwsbxm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gbdfslprv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzvhhchrm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gtknqfetf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gdntxsmyr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gvbrucryd.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gkhccaxdg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gwapcfyod.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gxtgwejde.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gciqptskj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gnpsryszh.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/guufooohp.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/glajibdfl.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvnuhjxgp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkgpiypvc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzgylidhm.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gengwvusk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/ghilylcpn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gixtqpbec.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gzjaouowy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gljxgniay.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gndyvmvch.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gdkepiifx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ghysbwtqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/glxxyizwv.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gxuomfdhc.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gujcxfuvz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxrbgtgwi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gkzacioum.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gfofyibad.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvxpyovob.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcnrwqnc.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwrbeffhj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gzvdlgkmt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gctngzvqe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gsdcnfxhb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gqfnpuupm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gmphxpcpy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/grgnqftxj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gokcblhcr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gopduieas.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gpzbihvpp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gsrpikfrs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gtmqgbfib.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gqikclzjd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gtzrgrkve.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gkvzjvfnk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gcmhnurbf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/glyfghkdf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gjruwqcjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gnrpdvrex.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/glgzttqlr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghfxhndtv.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gasackyvo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/givfobhxv.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gudissywu.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnwaptdlo.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gtxfazclm.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gktxgbxtt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/glpqgjjyc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjoalljow.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gqylngqhq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpotnuzbm.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gjbryycae.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gytftrqla.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gvadjfbow.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gxkephizg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gsgiaprvc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grhgvvpdb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gzbgwafsx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gtsvtgqxf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gzlpvdgvr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/grokvhhkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxnoacfon.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gvtfmyqxp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmkjtgu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gqticbhtu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmsazaabj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gchlaxieb.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbgqbwdqh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghhzdeect.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gblxnvtib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gyvxcxmnw.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gmmjkxpyg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gxchfinyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/glijhbxqb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gxyycvyrx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gvqvpdejj.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdttitswz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gqalqcuxx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gofvceurw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gkbwajuil.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/grbwegusr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gkztplwmp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/ghntoajqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/guqnrbotj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gupuryebc.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gldbztssa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/glkdewvut.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/grsbknsbu.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmsnefhdz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gecfeqxlf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxwnayqvw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gsqvhavih.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gbpdytlgh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/galeueobk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gtdpjwefz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gswrnthnb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/glixiangp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gagnfiens.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/geqfgotiw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gekehfvee.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/givfkatcr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpirhmwbu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gmhdvdklf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtqgndtvk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/geachxdka.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdraebrcz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gptrvdlxn.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gqestugto.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gnigiuycj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/glxjnlsqk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/ggystnpqv.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gmazrhtba.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gwvwkeirw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gxjzljowb.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gcnfuknmt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gmjaaxjnz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gegbyetwh.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gcrvjvgor.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gfhgpltbi.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gqnccvquk.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/ghlakbpeh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gafrjkkyg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gmtyryvxr.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/glpndkgqt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gmjffjewe.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gzizaqnwm.sHtML


<!-- 参考信息 -->