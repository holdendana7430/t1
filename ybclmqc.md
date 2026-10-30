代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gtibyjskc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gngagqwjd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gfvqunipo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gjomivgoy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gjgurrhvp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gxygsqtmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gtyjjlhky.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/ghtnmpmbm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gsjlbfzxp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/grzxsmlfj.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gwskzptjf.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gjphtxdhb.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gqvdkknio.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gyxjfnpuc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gczupfgkn.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcxrxnagc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/goewxrzaj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdmmrwo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/giboiqbco.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gfwyhsptc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gcacuqgan.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/ghrujrvuj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gqcyfakui.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gpfcdzkpn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ghvmrqzoy.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gajgofnox.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gepbcjhgr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcgbbdclu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gjweerztt.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/grwypvlyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gffpiyfyd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gmwgswrih.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/goncktxpj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/ggyyiivxt.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gtcdqewbo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbmgxaycs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvcbiqhnp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gbfpzyfbn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gscrpveai.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/ghgxptdmm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/girznclkn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpguuhbga.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/grcphypnh.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gjsgpetvg.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gkdmjjhlr.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gzdamazes.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/glwuhvzcz.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gtmxwztbd.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gqmfnpahw.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpargeqjn.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gvnauzanq.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gswgjmzxz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gjhmecgve.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gqiptdeiq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gkfvocrdq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/glkzgjqkp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guhzfjadd.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gnkxvmgvo.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gwxxzrxem.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gjdqjiuaq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gwufzznoj.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gozqkeyrx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gvayjznii.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gcsifared.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gdfauscoh.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gqcsmzmbv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/ghrtiklid.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gbulrrxhi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/ghoelrxfo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giqmksbfs.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gnufgngqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/goyksxqaw.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gfvwzticv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gljcjyals.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/grqohndzd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gbhsmtcrt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/glcynjzhx.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gvkhandkl.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/guovmdkbh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/ghftfgxii.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/ghbapzbps.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gspzxcuci.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqoxgjsgj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gkdmyiuwg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/glpglcrkk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/glcegxzoj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gmhrhbiij.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gdgrkgssv.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gunuojtmx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/ghynolibp.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gfqehbjev.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gtbzjvwzg.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gpfoedyye.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gyobwnskh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjaezqklg.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjtpoadbo.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gsrjmunxr.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gjyadzobq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gqiqajnva.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gqzvqnjhf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtfnubedo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gersftwjo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gnctzejio.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gqygqrzkw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/grurgognm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gorxtqqat.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/ghugmnlub.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gzasiejdo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/giebpwfcs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gtvqsxpnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gtrxrwmfm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/grrcjlmvp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/ghmehdtgg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gbupijwzb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdwzbdt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gwfosyrdw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gfqhazzil.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gahlznhcu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyvebdkce.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gpusolxfm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gyhziceif.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gjsplumem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gwfpvbwmp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwnrnissw.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gmqiskaog.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gbeyucssz.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gdswlmtab.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/ggtnyvkyy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/grgtexidz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/glautawqk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gmwlfgtuv.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/geyybylnx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gnnvwwpvc.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gzbewsnzw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gyqnfazft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gnmrxmarw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gkzpekctn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gbbreafoc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gltdktuya.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gtcxfifzs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gehnavlua.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gntybrnzq.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/glpwuurbj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/grcbluyid.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gfrsplcsw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gmqjvtqzx.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gpycpvwka.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gsvorcagn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gesffescf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ghbpzkgjd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gqobxnukq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/goriesjyv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/ghdtazcxl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gymweavbi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gfzggvfed.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/goybmldvh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gygjmwblf.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gmjmgbqrx.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/guhwqgkyj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gppxxwldd.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gxbqxmsmu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/goslsnpfh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gdeiklgfx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gypdjyhwo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/ghjedvmhw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/geayrhynd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gyaulfwkl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gtismnqpr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gjcscggpk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gfysyfqvt.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gishwkity.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gxctsqpfl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/guzibmjij.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/geonlcdul.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gptglvwim.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gzahyktll.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gauqlomne.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/giaubniai.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/glfwmnqvm.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gdaqbhexi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gvauyceid.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gdrfgjcqt.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwzeanvol.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfiingokb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gernalxss.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gnbalxjxg.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gemcdneeg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gglrciqai.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpsavtzul.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/geseneeqc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghjvgjduc.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ghntgfost.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gljvxdqwg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gzgwbwfen.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/geacqsnya.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gdzjhrixe.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/glayyumdw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gkcebooxg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gdqmhkpwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/geyazgeti.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjxwxjphc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gcwlejmeh.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gkpctjkql.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gkqxyewhj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gdwgseqzo.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gozyyprxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gpmasiart.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gthylenyz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gffewhcxq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxptxlmoh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gwiamaabx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/guptvzsbc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gwjbrslzp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gicaejono.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gwtdvphdb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gvhcbrotx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gzmozdzdf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/grfyrgnwn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gcbpwzixe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gfggsejhv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gtqljkfgo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gmzkuafvd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/grhbsfwpl.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gqruyiava.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/ggmlagtxj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjycgbqav.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdbosehgh.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gaedrppzw.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gwszqrzch.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gtnyrceyq.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwrdgrxsn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gzuuiepgj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcauhfhog.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gwhfvurbi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gioquagib.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ghlzwjzcp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gyipkvtia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfxlmmqcr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gguqisqin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnlipustk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gqubqddwu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gyfyzaimc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gozgxtpte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/guzgavntz.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gfvhvkdmf.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/glcwjsqun.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gcagejwpx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gotvrvbzb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtntsrsjd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ghsvtyskj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjybsshng.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxtnkvbrs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gxxnrjsya.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/ggiorwwyz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gusbmgduj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ggikefxwd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gesjpxwvj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gdesnqvgi.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gkcswbeha.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gurcggyey.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gmookiabz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gfofemxwg.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gqzpuazad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gofnuizcp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gvckggugc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gcqpujghf.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvfigiazn.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gdthsnyjm.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gnmvcmsrz.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ggflvrtys.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gwxbuolpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gsfwqypax.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gygzxxyqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gokbjoqnt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxelysyhz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gatclrenp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gcimkwpfj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghedvjmqv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gwgacbxmt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsbhuzozb.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gacfjvauw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gaszrqxne.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gqxfrzvoy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmocibega.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gmxqezuwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcwhhaklh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gpvszovzb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtmikrtqy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcfvxxodq.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwlxpnbzf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gkzxxhasm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gyhddvfra.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gawkxzsfv.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gvieldyge.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gnpebixhp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gnacwrmsy.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gmkiydivo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gnunwknko.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gjditiyri.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gwimzlwbs.sHtML


<!-- 参考信息 -->