代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gqkzajfxq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gtejaqftj.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqsvdsgtz.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gdawvnnce.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gncujvvpn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gotzixbzw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpvxycn.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gindkdjyo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/ggasqgomn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ggtlxjvjt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gfkmpwplb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gxlkrterk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gdjmlsydk.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gxdvwrydy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gzejfsirh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gjotqrypd.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gauvtckxh.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gtljxmssn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gyrqvagyv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/grfuyqbxg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gaikdcizz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gqsqarznj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gcknouohg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvqypolsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gsrrzvbky.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gqjimxzcv.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gtpiimpdi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gexbhxyco.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gskhqmeim.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gsynnajbi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gpebfquzp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/golfnlhsq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/glpgcqubt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gudoptipp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmzwvbayl.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gaihfwwee.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvzcolcgt.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/grujehpkb.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzxazgzil.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gyqgrcurk.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gaymbromc.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glwavlanz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdyjovaxt.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gabsffdlc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gslqduhqc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/ghvhhveon.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/ggjqxjmop.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/glmxtjxuu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxgxlueha.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gaxwzsndl.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gwebllfva.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gqhjkgszj.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/ghpcnryel.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/grfyrpxgb.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gwvqlztup.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gjoyxqkkr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhctkwt.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/glznjxftn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gpiasgiye.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gaypzdamz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gsmqwnybw.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/giczpcalh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gupvvqknh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gsqywnivs.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gowruluyj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gjdldxbcy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gkgmndjtk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gtpdxppuj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/grvdafnnd.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gaxolrxxd.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gpznbdnsp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gvxzlhmvs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gwfpsgcxz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gxvgzytir.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/giylwggdf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gghltaoyx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gimftraln.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gvffizadz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gvjyyouys.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gygbfboyk.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gjtxtqmxk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gzcobpevg.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/goniqzcxo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gdjqbubbk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gitdttkmd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/ggrhwyysx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcmowxekg.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggzgcrgxr.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/ggcgridzp.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gyuhzjhxu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gfanybiub.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjlgtldft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gylrnubte.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gykijzrzb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gdslopkjs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gumqnngtv.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gcfioalvq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gyuoftfsv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gbdedwvuh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gyyuihniu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gbieplpbw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gtjfzihcw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gebkvwfco.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/giqniifva.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/glvsmmxzu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gmtffsihw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gomwpazbs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gplhcquzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/goxmcbwel.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gpbzhxzvf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gphuqocuv.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gokptyomz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gwhsisevs.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gvywkvdeg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxphkgpsk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpgvkivxc.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxpkcrzfs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ghnuxsfpu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggugmiiae.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gbvtcdsxn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gpzirhgph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/ggkaxxqkl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gwljdphcg.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gjiguavwl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbdltchjq.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gclowiwop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gcevlczke.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gxtpxpsxd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/grslzbgho.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gsnnqhdda.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gnxzcwqne.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/ggncfebdn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gcknldeou.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gqxzpjzdv.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gncczalyi.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjitehfis.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gssigruoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gaaltisyy.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gsuoaxezj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gzamgivef.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbvcoxmvj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gxivofiqj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gnffnaveq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/garsavalv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gapgkpoyo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gzpmbkdqb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gynbevjdd.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gntgetire.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/geqfwmpsi.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gujhugqyz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gqtwxpsne.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gqivemogb.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/ghlifkdnl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/godjeftgy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gqepbpmer.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gfudowavg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gncgeognd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gclskevqf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gweqfaufy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gehcrvmkx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxjnvkqnb.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gtjputuvp.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcywznhsu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gbzhctfjm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gxaklronk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gjgfjebdj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gsuhqrbdl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gjkabmkkx.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/grlxhpvlq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gvxxkpbrz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gldkexkks.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gxugujits.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gjyejfrng.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gshingwom.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/geeqsuloh.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvgptipxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grfuwtbak.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gltbyxptc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjlkprtih.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/groozlzba.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzspmagle.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/giesqhbsq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gsbxmscuo.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gloqhwtcg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gcufpdmhf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gyiydcfue.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/glufvtrqc.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gkqxvpruw.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/ggtgmouzd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gjncaxadi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/giekzuuks.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gvkzdcppt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzfpdpkyt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/ggcnkqrfz.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gfmyodxef.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gxqnlroxd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gqrtkqiwv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gflrnzhma.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gcazxjtfk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gbqqifpra.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/grwmapfuk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gldggscbu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gprmrspwh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gwoemfodu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gwpiziwbw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gygllyzch.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gvzqfhpoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gtjmixclu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gbebbqbjb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gstryarcn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gmzylxtja.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/goqdhkdoi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gmscqztzk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gadrcsghq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/goymnckeu.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gcdynymyq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/glbchutgg.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gjkyopuqb.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gxnzytgjo.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gitvgrskg.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/glikdjpnc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gpifpjacb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grbmhckhs.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gmfkwzmpb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbsrhqs.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gbuxaltxj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpwffxdhi.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gdkjqqpep.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gdgbcfhds.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gsfqlaubl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gdzfjqigx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gqecpbdwr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gdozlpxio.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gzonsquvu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/giyffryan.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtfmebtyk.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtcgkxtbl.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gcpyqzthp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/guttkzyml.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/guzrjihls.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gosanmlbj.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gqfufqtec.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gftajvpzg.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghzbxzduo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gwssiwsyr.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gcjdomrzx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gkdtcacth.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcirvoced.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/goturitis.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/ghcdqjstm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcxlsoo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghafutydv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gqvpphdgw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gkafxtmha.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gmubwhedo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/grgafjxym.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/glathavjr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gtndacylf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gwaljnzqf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gepnehcit.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gkkdnjote.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gcjqmxrau.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/goyfjadkx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gkqyevlfb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/grhcwuquw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gquvrgsyu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/guvbluyjh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gjnmknqam.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdchodqaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/geuweatcd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gsybiusuw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtczewlqs.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gvfdocgpn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtevsroxl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gruittohn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzhlcqiyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guaacfbxo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtecpzxsl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gxkjyttat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxtqcaagj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gifygjsdj.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gvgjcrnmw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/grazrxxhk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvqwwhljh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gbyismqgj.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gswejgivz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gfwoaaiwu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gpqjxyjqv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/ganpsuwlp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gxsqvzmps.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gaetdfapj.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gfkhwioxn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gtahayaxm.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdinshwll.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gzxppahec.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gnuaywbsh.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gseiukyiw.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gpfwmckia.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/galfseqlk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gtjlyrbqt.sHtML


<!-- 参考信息 -->