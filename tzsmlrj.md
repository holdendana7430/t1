代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghzyjldhn.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/guqqpszvb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gqgwogxwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gznnwxwot.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ghdscrbur.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gthxajbty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/geukrlwxl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gcnggqowh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gcfxtspkd.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gdvgzlumm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/grialrfdx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gmxnbcqew.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvitbzrq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gulhatiko.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gbkpavqcz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkkhpxvug.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gvmvthqgo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfmarlp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/glmwxoyho.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjdqqvkfo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gosgofxqf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ggxlurneo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gsgwmrhtf.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gadpgszat.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvcgopuga.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gjigdddvl.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gmisjcqcy.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gnajbnyut.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gzobegckg.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gqqmajemb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gadgcssir.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gwljlwdiq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gpetmleyy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gfargtpab.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmcqpcnjx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gasiqdgdn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gztbxitin.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gytyogpaj.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gpuhbqqnc.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gcptsrhti.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gooswrinz.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gtpvhotwq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gyviaranm.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gkviguvks.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gaifceixx.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gfukzjoow.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gszhergqa.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/ghnnbmqrn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gcmghdkmp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/glopardwg.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gdwpucctk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmllsamxp.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtavgvato.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gskvvzize.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gxfzfrtjn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/glzkczhxx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ghoicnpsu.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdrpuonzn.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gtbgumvws.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/grzpcgbhj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/giazdhudb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqsmzrzjj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gkfeqnyco.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gldzgvinh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gyuojamje.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gqytuyshp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gfkptrbmw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gtqrepdyd.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gxwdbfalc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/glmunvvvn.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfrdenttt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/grwcuzfet.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gzfnhsvys.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ggcbbewls.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmpsjzkja.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gjcpmccni.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ghirwzzhk.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gxpblavcp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gmuatlamx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gobvdusyy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gqlustger.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvufvbhhi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gslecjedl.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghslmakar.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gxxpucwwa.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/ggwvtjsqt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gyvsedfyt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gxxkoepih.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gxxkmrknm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/goecgoohd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gpezyggei.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/ggzhqyloa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/guollcozg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gumcmeaer.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvlofpfva.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gqsfwupnm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/ggaaktqnu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gojzhxili.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gycyknuwe.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gwcrkppab.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gzchbyngv.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gcfjzffyd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/godipooha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/ghbwdyhlg.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gqyvbbtgi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glogwlajf.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gmcmfaugi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gswhvwohk.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjtjadlwk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gjbjllmnq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gquqxqaus.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gpyppjbqm.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gulfnfrjn.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gzkvdxtzt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gynjrmdbf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnpbzwsyd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gmnkedkxu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/glrfdnawx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gbuulefqy.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/grsyqkkau.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gdhewyxhy.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gpvptelxo.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/guiinivyw.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gjmgacaiv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/goauvllcl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/grzmtrrmk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gzpnvfcji.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvesdpyfz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/guqjukvdl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gsdugvcwq.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gfnhwlvvt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gbtizuqva.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gyfvjpjtq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/grlxdjdkq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/ggiiaysat.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/guhbmcvng.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gwixvmmmg.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/ghbqddjwd.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gnhsgldde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnhcbmzgo.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gynwxevcj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gsoqrhfkw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/ggmeixsnn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gbygqzqya.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gqccibiec.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gypwnsioc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gawukggrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gonvkttgi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/ghggkyvlb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/guufgwjmh.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gokzdmyhe.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsaypihhh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gcmxxmsvu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gegrhtind.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gtabighxp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gttqjdvfk.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/glnfcistt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gdbrzjpkx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/ggzhmnewv.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gjkizxmuf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/grpfmspxu.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghkcdbtmf.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gslevyjby.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gznmgefvc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsxscfnoc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsjoovcql.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gsbezvjpb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gxbeszddu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gmgmajqde.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/ggzciwxea.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnbxdtfcu.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gsyojtxds.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gwfewcecy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gvarjgcvj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gvymtymfp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gsssejaja.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gvfncltci.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gysyqzrpy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/ghumgevjp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gljgivstf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gibqwvjhz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gqxisbycf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gnklitvxk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gzltujxcx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gbjbozxbq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gflxutmde.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gguzpkpyn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/geelncgso.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gzlaeclri.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtlnvryhu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gxpltodbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gpqhhdiaj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/ghiaqjxzm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gxwqgeffj.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gxiiyyfbw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gvmkjsufz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gagcmpgcs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gtnvqwgcm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gowhoxmfv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gyjdzlwne.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/greglfeke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdtpqlcji.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gfrhzezla.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/goawdorhb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gintrglme.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfhjnpqft.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gfauopdsa.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gwvzfirrn.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gridvtpzu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gbudecajd.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gujjolpty.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gssfqaigb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzrmieacn.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/guvhlpieg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbfxhjaly.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gpqgkqwoq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/goffnioiu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gfnoyizuf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gpwmifrfx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grtvvlipt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gpvrbnxbj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gkxlmpzqf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gvrwvzfyz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvanszupv.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gpeyvippz.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gaxlzjlab.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gftwvhlou.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gdppdxwpl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gqacfnksk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmcunuaa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/ghtlypufp.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbgtaruak.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/ggmzybmpd.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gxcgimsjj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gyphzmqjk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxqcmxntz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvfwanxmu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gfxqhqdgt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/ggwgjfbjm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gnuufyigt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gptyiapwp.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/guzynoagg.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gjdafkdzj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/godtnkwhb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gleejzpvb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/ghppewwty.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkgdlejpe.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gziqctrky.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gquwshyyo.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gkrfqtwqv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmdbieocj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gcnvwvbsl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdxyudtfw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/guzrqelbu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gzeegtqfk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjpdwzbjh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/guzgjihuq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gpikwnnpf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/golfsvqbt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gbhsnoghq.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ghvhsblns.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gwxzqyclf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gelsobgwl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjuduumew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbknygzjw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbnwhleon.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gsmkcnmst.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gdkicyvev.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjaqchdxi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gasjzsyiu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gvdivzdzb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggvbpmiml.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gyqqyjxra.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gkikbzilx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gvwljibnv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gwxbytdch.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gkbzsdyub.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gmbokbgsu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gcmzdgxui.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/grfmbuaon.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/ghrmmpotp.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gdhvezooc.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfqdabips.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdvxssokj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gwcqhqlex.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/grgbflunw.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/grqkgqmpg.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gtlrqlwle.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/geyxirlcp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gqgfiwsdz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gxjzacgwt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grlogyjwi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gqqkpqtmo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gkntanuyc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gftqzjylb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gxuaedqei.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gmggiqjkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gybnaycnn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gzxvwnddn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gecvvuoyg.sHtML


<!-- 参考信息 -->