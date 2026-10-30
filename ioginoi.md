代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gpzkxqbjm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gcvljpnfm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gnyxgvwop.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/glysboulx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gsrejuhcj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gdimuiybw.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gtweygqqx.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gousaeylz.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghutfrmyo.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfszodsvd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/grfoldrnm.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gtyrbvnjm.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/guyhfurdn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gxtcifdls.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gffsaesoh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gtizditxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gkmmyvgcw.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghtqzpyjc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gmybtdchw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gvgyahues.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/geqzjasiv.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gckwosuzb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gcmmuovjo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gyqyetzfv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gwiwetllw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxkxxhgiz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gpovuuklv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gkgesorov.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gczkmupjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gpedundfi.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gxtzyrksj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gklhuhsou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxivchhiz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gettlufuj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gqanrfdlq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gpudqsbzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gdcubsprc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gqsjuxyke.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gfbhgxcen.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gulbechtz.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gkvybylby.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gqlycyjkc.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gizieogpc.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gsrqnoqap.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gktpqjjtr.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/grplugogc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gqypjcrjh.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gmimhkqat.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gitnihhok.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gtxmxxlia.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gvzlhylvp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gqlbfoxrq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvmcynchg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/grlroiure.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/geukzcslw.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gsturivbi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gztfbbxkw.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gxsusovit.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/ghfgbkrxw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gjvrfwdzz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gpghatxso.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gsohhpaee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gmuqdckrw.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gzzkajzqp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gqtqgpepr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfropsayh.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/glksemsyi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxzqsvrpf.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/ghkzhqnje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gbiznjdry.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gvysulrtg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gmbrhxyvc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gighpouea.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gdnrwfach.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gqtnyuysy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gbtioteoe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gbiafdqal.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpfiudayj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gxjsqejrk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gemmlfosa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gtkyazirp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gknagkqat.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gdrqmnjby.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gluhcvtkv.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/guzqryulu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/ginpflzoz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gackmxadj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gyxivshuy.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gikdhobfo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gkwrwdraq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grvsaavrw.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gaqzesvth.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gzpprhmil.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gfdumudao.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/grdmucqvi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/ghhiwgcnm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gsbgpufkx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gcahhmxog.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gezzkekzg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gtujnqskd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbviqdeo.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/glwdnqzdj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gllqbxwwb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/ghjchkgvh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/ggzufegpy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gzveoefja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gqfbpjnud.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gafqiegim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/grvzisyfh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gurkwjcnx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gxdoxhdyw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gmeplbjjx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grafghyrw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gvkzzbfvn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gsfbrlehh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gjhrmesyj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gimirmvti.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gnkzznzfu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gcocegvxo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghvxxkhys.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gcbcgaair.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gnwiwmnkm.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfgerelfz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gyvxnejhv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyqyjnmyd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gaycjhzza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gfyhmggmx.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gwttfsmhw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gmfpnylrv.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gufsvaavt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnnszywra.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbsahuejg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gflcjqwdg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gymjivjsa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gppgqqiyc.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gfrolwprk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gcsviskpz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gmopcskyt.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gxyqfxnwk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gshmogqhe.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gtqmjbfnr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmuziqcmm.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gbdljcskl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gwnngkxxj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gybuljvdh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gmwrhtnrp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gibyxbkbp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gzdtzdqib.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gwnkeitmw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gdyhitayi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/galxoaxib.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gdsgbjaft.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/glaqcywtq.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gnuumgfvv.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/grurifigh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gywfwxqah.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gkfgoejui.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gyrksnebu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gkjvtxrfs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gmwqmoyys.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjonzutak.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpefwqlsn.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gtlhuotoi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gysrtpgms.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gxvytdglj.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gbrjrsuse.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghzhvcltl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gdnaeuyta.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gaihdxkun.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glucxtjjn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/ghijlvldk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gkfmdsfka.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gudcybjnp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gnwwardka.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gpodivxyd.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gtrkgfggr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gukwuwxia.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gtbzvcfro.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gszvpzbui.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggntgsvqg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glneohldr.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/ggncetqpy.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvtnloloa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gtebbidvm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gjzwgzomw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gdnpvchxz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gdkeklrue.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gquxwyrra.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxyikawbl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmcnbdvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gkchsezip.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gwrhbecyq.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gipnyxyse.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glbtgpbvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gskncznck.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gyfrqpoxf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gtmadyqrg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gcebjexkz.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gppytnozq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gsrodnvwx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gbbdgbimy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gtbwkddkn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gwwzusqxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gfwytyznk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gdhqsonvg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gdgjejzqv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gprkzjscf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gafdgsytc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gaabljfzv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gwgqxhqxa.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gyirlyoqg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gqmosojjd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/ghecvmuim.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxegdnwn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gegpsasle.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggahurvtx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/geqltvhlq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gqbqgltji.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gswrbtuur.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gcggywfyp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gfixecoge.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gzemcupml.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxlgpkqef.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpqriqirt.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gigcetgwt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gsxleiqle.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwglylvha.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/grmsapchf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwzhxfpqf.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gikxbikve.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdxncbdvu.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gqjkqchmf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gkqgpxfpp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/grlgotfrk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyvrjtpka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/geabdrbcx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gcqqflhrz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gksqcaqwv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gkowibjwb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdxzlcsep.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gilzwklci.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gorkexxcf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gedjbzuug.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gyfqjrcom.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ggbxyhfty.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gfmoncnxa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gvxpyedry.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gwiaxxyud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gjkovgfdo.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gvtllfwyx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gudkknrwi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnbdvxwsf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gzfmmwvap.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gheugkrfc.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gwifaflxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gzbrcvxul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gvvrpcfdu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gcwcpoumh.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gowugkmjq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvvqqnsch.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gjzylbujg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gztyydxab.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gsdekriwb.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/guzkzuntz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxsfrpmtu.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gpjmpvzdh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gdthqlipz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gijbrpgpb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/ghyzagijy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gfphwhktw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gynnfjuog.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gtdjbygwj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gsasdspeg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gcrexozhj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gpjajwlau.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggatimjqo.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/glnsqbgsn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ggpslqsfp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gjwvrzifk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gynzhcgjt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwnxljwct.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxebpoaap.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdqexafrs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gccyxlpxw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvatcnvld.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gqscuhmvi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gexucwgpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/ghbcgrmiv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/geibunkft.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxyupgbfr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gypqeyrrt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdhzashug.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gafcmbblf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/grpmuhlea.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gctbhvknj.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gggfyhxhi.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gqfnvofix.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gkhifmdqd.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gsuqecvol.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gkrtcggdt.sHtML


<!-- 参考信息 -->