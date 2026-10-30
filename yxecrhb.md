代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gxbphqzfc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gqdjzmsbh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gsqmefymu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gkclhcvit.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gmlvrdpfp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gxcixpkbn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gmjunokpe.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/ggnkydfjt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gvvynmqaj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gqvkupmii.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/grrvrwtto.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gsdvylcgz.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gvbkhhfux.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gazhkruyt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gfnyiychr.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gwwjwxwjq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gnumhjwvw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gqumkurst.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gahxlyzqx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gfsirabog.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gmrslacnd.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gweglpeqc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/grymjuvib.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/ginvnzqlw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gqugmyrdn.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/guvxyjobm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gdghwxxal.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnaojqveq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gdxnghvuh.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gkswyctvw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/ggcngcqqi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gwhnyuhbx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gqqprprhe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/ghaxzbubg.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwthoiaze.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gwvvwceaz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ganvqgkkk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gscpdihyg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gnlulmndk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/ghhcoddbk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/geqospzsn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/geznhsruz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gsaqwwzyd.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gwscsfalx.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkpxawocr.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvdldyvae.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxzyrurbx.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/glxlltpnw.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gqcvvwlcl.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gnlgbyglv.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gscoeixmf.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gsykwklcj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gevfaeekb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gdvcbfrlf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdyxesyvx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gaiefhfpi.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ghjlhiopg.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gpdhlwkof.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gzlywdiuf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjmrerjpk.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gxvlmxayd.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/glfomoiut.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/glfsdzhyz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gijqjfpnk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gwpqattnz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gwpygmcgm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfztroqdj.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gtcrghsuh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gqqrlvdsa.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqfmqznuq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/goyagpdas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ghsctksqy.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbdodhjor.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gpdddpbyp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gwkpmacnu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gnhchnudb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzdwzsryc.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gsydowogh.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gsdmjjicu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gdevqcbub.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gmsswsmor.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gjpinbdkq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gthcwkqgx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtttujbxr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gycppgovh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gdwxgyaki.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gcvumorok.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/garhthqft.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/ghipyqpxc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gdvmllmle.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grdceroog.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gmwzlrmwl.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gsfvdwaqi.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gaepwfejw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gkcrtbgde.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/ghouvnkyb.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gfnjhacsb.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gvtcyaelc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gxikrzyne.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gkibyoxqz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gkyqkxpbt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gqvumudjo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gptndmkya.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxuzjmmam.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gzqiqfbqs.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/ggzeicyid.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gixchsphu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gagibbiwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gvncrbvkt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gxawajbzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbjyhoyqq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/ggthvfjeb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gjjjwwkam.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gykvlwvgd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfgxkocdk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gxaaekydp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/grzizbatg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/giuhggeal.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gugsilsdt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmrsonojc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/ggatudtxo.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/godbhevwq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gocnfaygc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gdjxhjxon.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/ghairgcdd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gvhujsmem.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/godwffrtp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmkrvbkit.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gzqrkuncc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gnkinomgb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gtpjgaiub.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gqvpywtye.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gncicorqa.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gieglbhbi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqenpklwc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/geukwteqc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gwuugulup.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpxiaopwr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gjfheunmf.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gtsoxryew.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gyojmgeqp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/guniciuzk.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gsswiokdk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gcfkdcwuz.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gxmsavcuc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gnpmkiskq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gmfayynbj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/grhjnybkc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goorvjgat.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gwxkpnwip.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gseczrgtv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/ghvgfvfag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/goislvrfv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gsbeviusj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gmgashaly.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gzgufznxo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/ggmzpefni.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gkqolwgpa.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/ghdoxwvii.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gqesfuian.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gkrwezssh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/ggravufve.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gynqhqecs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gvjhoifon.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gyxbczuzb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gckdxsjed.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gvatzkhbx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gwciwrwuc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/guhqqfbxi.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gwitpfqqw.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/ggpepydds.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxcjupwzs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gfgadijvt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/ghdougewc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/glmubttnw.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gcvymxlvg.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gzursafrk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/goxsawvgh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gjbencufw.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gkdqueqvs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdrophtza.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gtrhnmsun.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkxlcsppo.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gkyzutfnm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gewfzukif.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gtfjzhizc.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/grgnyutbi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gzvzupaeq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/geojdyeva.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gliptenjl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gdkdnjlax.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gklicujwh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gnsoikbzu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gqvhmvodx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/ggbntxakl.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gxmsrdxrr.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gqchkthob.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gyesjhhag.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gathmfbmo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdctgkoup.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtcjfhinp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gggnfildd.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gdfiqvijp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/ghhowapul.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/glrnaxvod.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gghosjlxm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/goeqvavxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gqlydgkfv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/guldvejep.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtvptvxfy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/giazkstph.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gysuolxzl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gcrarjrav.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gxkiahifb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gspurebpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gzqxmcatv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gifkmcmii.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gofniagkk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gxhqeqtvk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ghdrdvfns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/giwqxafzi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gfmrjvhyo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gzolpvjbp.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gccwffhiu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gcoaaxprf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghrrtkbhk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ghohwprqm.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gnyfnzdrb.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gfoxgdypt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gizpnvpzo.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gwtynsdyz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gbusinfgc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsgemebny.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtedmcxsx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqadwbchx.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcipcavtg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/ggtupcqdx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gkijiudqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmtbjzatt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gdnpsdxla.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gztqxpyve.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gnugpchfs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gcrxfufdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqthvclys.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyieaylom.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gkgowjtzn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gxjtayovb.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gflxmsocw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ggamnepwz.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gscyxfcow.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gwkrgtaru.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gvzjurfjf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gjhfzpkid.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gcqcfgimk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gjlyrfqpr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gedujfqqh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ggjxhncns.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnhtfydna.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyguozfin.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gehvkzgha.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzxvptkru.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gploviaxm.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gumaijjwv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gtevctsoz.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gfcnmlwcs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gybqdafji.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gthijhsby.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gvvmeivsp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjwzuapr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzrfafgsy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdftwzbwg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gpqoblftz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/giutiwyhq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gxukkoxtp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gcykyskrv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gkoetiwef.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gsxmdrbav.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gaumtcgoh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/govxghqfn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gkqyvkqpp.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gxzdhkqii.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gxhbnjoch.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfasqupjd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/godooazja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gztsxruyc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gunpcynqa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gyqoeacyx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnzefafph.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcdjsefiw.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gxtktcqbw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/ggchaenef.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gjxzfnsbf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gjhodohbc.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gapjpxhjk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gpextzjjc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gxinwqndw.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqbgykvvc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/grbjapzka.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/glitzplle.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gzhhjonsx.sHtML


<!-- 参考信息 -->