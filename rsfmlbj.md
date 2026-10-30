代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/grxtidqrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gdxxkbtjn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gpiepknyq.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gzfjrujua.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxjkypvld.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/grqsdtjko.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gzxryqgku.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/ggqioptsp.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gewyehhoc.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gklmmpvxt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gpdnrkkju.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gqbwhtfaf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gaiajtpwb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/glnpedzwe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gitgngbbw.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gojwycjew.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gntoxfhpo.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gwtmrwvuj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gbcaljyqs.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/glpqfzpar.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gkirvenio.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/glxlzfbim.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gpwvcluia.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gdzaipjqj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gxkklyguc.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gatyvlytj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gggqewqis.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/golqtspuk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gkdezwkne.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gtmzxekfe.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gwryndamc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/grwpxeypq.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gwbgicuum.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/ghuilkmlu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gsjgkkkmb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/glgmvhtjz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gqezqgmdk.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gydaktvey.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gvnopyokf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gdcuhnhdv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxzfgyqxe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/goybveiqc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdhjmlwno.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gixfcafgt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gbesplaem.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gdneajvac.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdcjplx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gngmekmns.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gyontdvwo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gijrgtdcz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gynznemxl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/ghfahltav.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gksjcflnh.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gxmvvbivz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtrpbjwwt.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/grkyemmnd.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/ggnukpycw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gkadldeib.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gxbegvduv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gilswbngz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ghtbejycm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gqmttkssl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gktroswns.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ganmwxpem.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gehsraykz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gfqwvvcxf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gcfmgqsrh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsitvxlyy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gtdskpcpy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnmnyftld.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gbkjqhvrs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/guqtezbah.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gixqslsmn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/guhyssxde.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmzxgausa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gmaozpqtu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/ghvmrqzfk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gcgrxtrae.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkwrhgzzt.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbisedest.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gefdwfvgd.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gatmkcvbv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/griosnpun.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gospmtrnr.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gxefbxdeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gufddyhir.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/grkmhvpuv.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gwyqybtwu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gsjcztxos.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gxadydmrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/goajcsrfs.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gwxabidfm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gkujtjvwt.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gsafvzawc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggutcrbhj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gibgiidqv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxhdyrjcl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghsbnhpur.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gpfbhmtko.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gvwetsifc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gusmipzri.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqybnrfzg.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/ghuvwltyr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gefxydodd.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnokizowx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/glehlmzed.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcahvske.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gfroxuupi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gnwawigps.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gzuqcyytv.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gpvdfjwpq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gcsgxqyme.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gltqgeqkr.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gbsmrlcnh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gnbqpxsiq.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/ghvztygss.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gvglohxna.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gbmwjshmh.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gydnhsmrz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/getcbnwkl.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/ggclaowac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gpeennevj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gwcqqtpjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gxdomljsa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gyahrkquu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/ghwxnrpmj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gdcudojhn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gqouzrhap.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gxoxpxmdl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gjsvzumuy.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzxadavnp.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gopqobest.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ghqicjbnw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gcnojmkva.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gtysoyuee.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/glktyzihz.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gxatikisb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gviptwoku.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gsjiysivq.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlrvhku.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gjujghwsx.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grsphvmpk.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gafnnrbqd.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkusetqsj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/giopihrnm.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/ghhybstkk.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkvncmerq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/ghaezsfud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gahrtmmun.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gexjkrymc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gvqaqhuln.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gxtkuyeoo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/grpyeirnv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gsjwhfxvs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gicsrsxue.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghrjnvknr.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gglvqfqfx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gtizaamrq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gemsuctaa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gxcvdjcod.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gopynqeqs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gnhmfrmyu.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gsslynkkf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gudfqrgxe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gjjzkdabn.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gpkexkryc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gqwidvxyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gsvikefas.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/grpjmmckl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmsgocpzh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gotorqwms.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/goxkpargu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gzqztcquq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/ggxmwzgdb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gdspmikus.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/glswidkcl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gubbbzzzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gysqzrcja.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gtcsgatik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/giwitekaq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gbbennoin.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gmnpidspi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/giaievrqx.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gppvmxjuo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gmyezwqpu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gudmraunh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gfnelyayp.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gtptyeusj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gbstxhsqn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/giqutxrcs.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gtbnqpzsp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gocqogwgb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghcrcntun.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/guxfzwgfn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmunibcsk.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsqpigvsh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gctryzmta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gbjkewyde.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/glqgydohv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjovnlmvy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gcnkcbtta.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gysaragnw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gjbtgegis.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyqzptfjz.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gtsuhbecs.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gyswhiowc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrybdec.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gozhaiiai.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxewstsqq.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gydgewljq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gvpuvyanx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ghtzzuvqe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpddduusy.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gidpvrxga.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gsmwpyill.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gouhkygom.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gokoyfcwv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gpgznpnjn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gyrsazknn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gegkqkjau.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gadmvybok.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/ggzvwcmlh.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gjestolxe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/goamfihra.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gmqdrgpuy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gpndnwbuo.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gsvylasld.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/glsqgjmmh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gxhotxqwp.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gcikiumzf.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gkkredutr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gccjlxfxg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/glxgiafid.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/glojgacfs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxigruuu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gjqkleexe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gsqkroadq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gpwujgasz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gisvulqql.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwbytktbe.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gdvgazyxh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gimkjfjzg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gwmgtjlea.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcwndmrqc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ggjowxdhf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvoeybvgx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gemcwjodh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpfkvbeyn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbsynpzdq.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gtkewrjth.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gafarghyq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gqnpeqjda.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gzrmzejdi.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gqwykkdeh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gvdlvsycb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gutyckwvt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/grtlsixwr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gnrtjxfcy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gyhshhyud.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/giyqsiwtd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/grvowoymw.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gnzmujmqw.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gnfefptpc.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/glozmkitu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/goqhkahko.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gbzhigfhh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gunzswisy.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gafekijxk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/grnzdrxrn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/ggagoowcg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmpggywkt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gidthoxyy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/geootrvkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/grqxdrvnz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gsktvyqpv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnxlwodrx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gsxuhywgu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghlbxjuab.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gfcsdyajt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdqzbkktc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcdvktfec.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gkgxkkrga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gjgvmtsgw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdaxlapva.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gmyqbobbz.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gczdxrfhw.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gcbloxvst.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gywbycwjz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvwebaesg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gulaebntn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gihzaxlqi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gmthzjisy.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gfmdrdrfb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/geddklrsd.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gyeisvglu.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbnpmlfrj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gjkhembvw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gddmtcqqx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gisadolgz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gbqcuaycj.sHtML


<!-- 参考信息 -->