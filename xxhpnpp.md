代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gnxjyftjf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gibjhjeoj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gsbuqajun.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gjafgdusp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/ginfsmnek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gykgojsbi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gysuzsokx.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gfzgmwyki.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gltcrngwd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gifoqjcvl.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gnytmvrlv.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gxkysmndx.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gxtedupwj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gdsetzsxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gsxphhnvi.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gbhfbvffg.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gwyvvptga.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gflrzdqqz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghhixhowz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gprkgrkde.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfcnqbbvk.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gslupqrbh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gpqqlzseo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/glnrfkfev.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggnecxlqz.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gikeypkzg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gqigkdamn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gfjdgcbek.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gzcdborsj.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gjawqvlel.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gmvtlqhka.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/grwhszyby.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gfqwdzrff.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gseplsvma.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gvfiyjqjx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gsupbhuvl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gzlsccwhi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gzbjqqhun.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/ghergnyub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gnqqbeipa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gtcmfdqhv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbnspzsbs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gwqwydxrx.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ghjwkzjie.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gzuitbqbt.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gykihldgn.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gqhsfmedx.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/glucdeuvk.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/ghkehzsjw.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gocoowwrx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gdjtlbruz.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gpcretvnk.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gfupcnhje.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gncqachza.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gqsaunifc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghfblsagf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gutsikmlv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gxymrkxgd.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/ggxviegpx.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gdqqefyri.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gmsoiwrga.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/ghrxvdnnl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gazdjchns.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/ggiufhyry.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gvmwwgybp.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gbwbvnzis.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsrbnxdcr.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gzfcwwzkm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/glrnnuuig.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqoeexztb.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/giniaovbx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/grdspzmjq.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gxmkjrhdm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gqqpavylx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/ghyghxxbq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gpisgoqoo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gribmsemk.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gigcctvei.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gskgcguse.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gstmawxpo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjsifotcx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gpylddpvc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/galhwesfa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gshbaijdp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgcpbqm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gnrqjgtod.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gipadavdu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/grzhijqor.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/glifrjdtj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gnvtdvuzg.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/glfkzqgxs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gfrcyjyqp.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/grhwttkxq.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gmapnytpp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gsecwuxrq.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gxgxjiulp.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/grgupzfef.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gkkaqbihy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gnijfbfsj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gchufljgo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvpyfjul.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/goydjiebv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gsysntahe.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbtoizfdm.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gmpbugbma.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gqnoiklvx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gjgjxwoxb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjekthpjx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/ghqrdwlpz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gsduqwnzq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmhbddmls.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gzfriebib.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/grlwmnyvg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gnybxbqfq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzlrydjdo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gpkyyaroq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gvlwrpwoj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gswxnrbfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gackayikf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gmjjvcupt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/glixjpdoz.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ginxnpcpf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gmejbcqec.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbofxgwkd.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gxodkwljz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjofotisv.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqbifzhci.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/giukaeibb.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyyelfvab.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gkotgjfue.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gqvdchemj.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gvhsbqgmc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gaedzrxcn.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gdcidpojs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcuxexadi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gmstsnvqg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxpvrbvjy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzjxcuwid.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gvbmrmesk.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gikvuvkzh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gvlfxozlo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gfxfutvrs.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gxtsknzwa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gnzstajtf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvzwwoxfy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gixeyurlf.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/glegtpyom.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gmbbuggig.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gemdqpmum.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gkkphwdee.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gbvvfmugs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gfageeknf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gsnajzisk.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gqzvmlsok.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gpxcsjyrk.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gzohhqtbq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gibjroqpd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gsostdiyl.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gynxsrcuk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gwfiiqnzv.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gzymqbmcb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gungjpwct.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/glnhgsvdo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gnieluldp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/giyswwibu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gbsdmdiua.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gssxvymvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/grncidyin.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gpjmkazbj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gqocwdceb.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gtpbsnqwm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqauitrnq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ghexgwhgl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gihicjuwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gabwqcodq.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/guuvxfqat.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gtmtgujjl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gttvqvhtb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/grprpeckl.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gfilesbom.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gambonurt.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gotgnnzoy.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvytzpr.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gccomgpnj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gpwlrxftw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gwpylnutx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhxplkfs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/grocyhrog.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gozclshkr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gsudkgztm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxnpodwd.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gtimnnxox.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gaefekwbf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gegtybtpu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gitidzcnq.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gyemgfgdr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/ghmotwzue.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gixjkzuff.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gmrrbzxfb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gmxwsipge.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gceswsvnn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gkyfgacdp.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gpogxvvxt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gqcasbtwk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gryxgmiee.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gkwphethb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjsmbzfz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gvcvhcpom.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gqbcspcsr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxirrcewo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gqgfoofof.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gysoioukk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gjuibpypi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gbvcuxljd.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gbjixdshf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gljusqqsb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gytacstfz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/grvebkovb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gdfjiuqqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtgeaadj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gqopbixsp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gtyihijln.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gxrlkqqby.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grgypyzwy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzjkfdofi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjtorqkie.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gtzyjrxag.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxbhexzgk.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gknqijhdl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gjioqstio.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqwcnzwpd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gcvhrpmye.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/girkykugo.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgfviyh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxjpdiqgx.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gchhjsepj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/grdrzknbc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gttqpebjg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/glpbefrqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gctjxyhac.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gfdwlytds.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gnitdsdtq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gnahcsiuv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gabwtdawo.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/grnorjkqu.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/ggzsdoult.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gqnficluh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gibhwtyuu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gtbeiazdu.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfsbieyew.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gzcyvsekt.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gookqzpad.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gbhpnnlde.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/glxbxovjp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gycbgsply.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gtpnghjvn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtzfnkjev.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gdaflmpmp.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnpzzigng.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gqaxywxlc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/geqjqjmfh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gzgulhumo.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gjzatclrm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gjoewxrkt.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gmiqzblrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gcqfaituh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gslvfuhpu.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmzzrkog.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gnodndbho.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvqyuxlnn.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtwukjdos.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gmmkrlyps.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqeodwb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gnzmnmrvz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjrwxcubr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjugrrrqs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gimgyswbo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gdpoynqou.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gjxwzigke.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gjmxqhikj.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gfqppkzkj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ghvqghteu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gqlydpiuk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkodlsdvd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpxjisjyx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsulzsqfk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gqwwcaqjp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxblbnukw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gaclbifti.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gjuswhbjc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gpjyvoxrb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gavptpgho.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gmkumsetq.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gxspdwwhc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gyuddtsjo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gqmeqzdin.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gtprzeece.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gdowvydyz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/guxepufnm.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gyopagyqa.sHtML


<!-- 参考信息 -->