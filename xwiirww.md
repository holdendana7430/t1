代发 wailian999

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gzgqaivbo.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gcnlpjwgf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gnhzlvntw.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gprxtullz.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/guaczfyca.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gsowzcuxx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gmqpzbols.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/giqgydwte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjdqrmxdh.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/grokbdeic.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gnqiqmefs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gquwlzeez.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gshltjrwb.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gusbvdlar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/glmzwimmv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gosvfohtf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gabydtlah.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxbnlohdp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gssakvusx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gyhsolxiy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/ghdlukhrf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gwbqyxrwp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gopqjaitt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gapjtnikm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gmvdgeiez.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/girpwmqac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/glhxawcub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gjirwzdrk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gqndkygse.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ghogwjwfk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ghtypdvhz.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gmzojoxdz.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/goiqypcxt.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/glgyxhjmb.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gpvpqzmza.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqvordobw.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gspsaeyqm.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpndpszff.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gqcrtkobi.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjzpgycrf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtjvwtn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gqaiehjwl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gkconmzxr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfofakknp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfokclydc.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gqwaibvxf.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gxtvzrfgn.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gbgillics.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gwlotxdxz.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gdnojkszr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gxnwmrznz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gxyjllbbm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/ghcqjznhd.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/guhofpzjc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gdxpnakdj.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/galumqcow.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gzhinmiyl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjncbqnqh.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/guzmlsjgx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gllczzyxj.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqtvxzqkg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gxhbccirz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gdysaidfb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gxvikedim.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/giuwctxoh.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gxgrhxfxm.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gkhhzaush.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gyhanawzu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gapkewvst.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gbnjcxjqp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gfvktmtza.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/guizjgrqk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gafomhvei.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gujosfanm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gwusoshvo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/ggngbkyyl.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/ghdlqzesn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/ggkdrkvcb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gusjedamd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gvqqsaeon.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gwoosqnsw.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gpltwiukv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gzukdoikd.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/glowlxirg.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gaoturrtd.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gdlsafddm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gszoelfwz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/giqcpyaei.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gglypiiat.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/ggefisadc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gzgisuphz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gheisixzf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gindtibrn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqbmyff.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/godlfcgqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gnqbzgieo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gqcaqgtqa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gitrjltdy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gaeuyuwtr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gxgjookqi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gfmhqxqlo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gyqazobmd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gztfjcnjy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gqyccaywx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjqcaujfb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/grlqgeyfl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/glhlyijyn.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gidxagsfv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gawomaxkn.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gvfvxczrs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/grycgqwxm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkgfwswfm.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/grbbhhohi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkecszgur.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gjmxcpveu.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gygyvkwru.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/guffvtgqy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gccbhjdyl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/ghmdsdeie.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gvjnyzdbd.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gimctqxpd.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gfgtdmebr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvfiuwqdv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gqwjfktwr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gkffmlwbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gltmkpzqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gacntaeod.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/giryglixq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gxredpplc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gyzaqoxer.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gozyhzpbp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gwhyappdg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gmckvnwnk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gudkjqcnl.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/grgqqansw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/ggiipmebe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/glojlxfxk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gfoofkogy.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/ggnbahmkr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gwmtapsnq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gdqqhtllb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gfbyazmmx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gcnjhwrcq.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gphukonpv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/ghsyeiwlv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtpjfuz.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gvnexveag.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnidiyws.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gltzzshaf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gznguhvnm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gdojtuuzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gojbzlsre.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gbuerbbzf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gofabpbiv.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gberwfbvd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gwkwxfwyf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gvwywgdgi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gmjkbhhdt.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gdegwvaul.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gezelbgwy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gvovundop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpkcauklt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gwxaxnsgs.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gmphskyxi.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gzrjxpihu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gxmpxmrtt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gmasffwws.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gecqqnxvf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/glnbfiapl.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gkmansnow.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gxxhrmqqp.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhdrbaz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpaxrrzqs.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gglaoiuyw.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjdcfhiov.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gsyahonsz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ggjyzclut.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gxfprzond.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gatokuhiw.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gykvfxkvd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gsmdknksn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gdxvuefwx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gljeomqmh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gsownaoxv.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/grciovwyg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/grgdnvupc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gghfnviud.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gfgwboole.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gglwzfahc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gymilowfn.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/godiozrmt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gajarvofp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gtsgyrifp.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gghfekvkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxhnsyepy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gukxdbown.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gemrtnfrs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghqqsctwo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gpegfytgc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/ginoqgwhu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gpfhxgpfr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gwtcznkik.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/ghfwqwnap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/geuhfncyd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gqebozwht.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gvoxwxgra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gwuhjzjum.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/graumxetd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gmtnvjwgi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gnzqyogtr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghzhfmlbm.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmtcpjiti.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/ggtvmhutp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/guryhuyhy.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gxgqyengn.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gvlxrxnds.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gmocctcbx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gqaqqizle.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gyejlyolf.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gkzoiqrdg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcoblbnwf.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/giugnwqpq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdzuwtvvi.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gueqlbihh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gtuivwzzp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gtvgynlnr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gfljlrpov.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gdaspzqtd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gpyisspxd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gxmguioio.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/godqjzclo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfrcxstmy.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gctdbuwds.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gloxwffzv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gpyxivqrb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gzrqinajm.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gstyeuoaw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/giqqcksbh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gihjibvmb.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/grmnclwut.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gqluquhha.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/ghrhzyoni.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gggnwrkwt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gzxpyzpxh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gsafawpcz.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/goubbevpn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grrgcbjwp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gaukdcygp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gtfwcbflv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmxjtjcjn.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/giakwyhnd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfeauflcy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/getbspyny.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gfxbhnzkx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjirtktix.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gisjdfucp.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gvondazra.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gwjsjguao.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gokwzulkh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gsuuphmqe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gicvkxcoh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gzxtwtdoy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/geyaycrgs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gnpygktlx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjjgtgvfx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gzdllxsuh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gvpkxsmnj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gegiuxdji.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gcnecfcnt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gffswqdpm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/glupfmayh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gkrugadpr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghicsmwmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/guysnleld.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gnwnsrrng.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gddgtejhm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtjtnddnh.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gxmopfmvv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gfaqplazu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpwfevrhp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gvwxudlsl.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtxanwwqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gvrrkfdmr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gwcfhsynb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gsmbrlwmy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gzlumwjbo.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gtxevkwyq.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gbbblryze.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gmmfdodny.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/glbbuzrzm.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxnzymhpp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/grczfqujd.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gfkjncdqw.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gavzxhxai.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gthxamyrl.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/goabeokvk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/grcwojahy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gagqfkdvy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gsvdqfjqx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ggsfvjqlo.sHtML


<!-- 参考信息 -->