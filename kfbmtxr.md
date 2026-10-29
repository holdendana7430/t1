代发 wailian999

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gchgbuthw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gdgfmrrlb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gzragvzmq.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gyyyhdtfy.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gkihvauaq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzjoypejb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gchvbydhl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gtfsegrlx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdbpwtaof.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/genhktusj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gzqbiroxm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gqsosomwc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gzsjrkypg.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gultzxuyx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gtzgtehpy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/goatcxtcs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/goqjfsjwb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gkyivdves.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gqzrrdsul.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvdcewcbp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/ggfiquyil.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/ghkhgbmwl.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gzydijgzp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gtfwpqvjm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gwzhuxmlh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gnzrxdggh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gnkmikled.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gvgvmwgbw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gjivlitsv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gvuhhwpfp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjbyhmpxs.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gdxhupzal.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gtsjcqnkt.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvgegweia.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gstbhcukk.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gxzeywtpc.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gqdgclpds.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvlmmsqga.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/grmjczpqs.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gbsnkugqy.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gqzecdhqy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/giotnioxc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gsmoadqgd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/grukzsopc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghdknhoyf.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gwxebpstx.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gkbqcrzuw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gesijsbhj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/grdwhclbd.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gdezrvhax.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gzlyvfgvi.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gcxzfpqjw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gumepgjzd.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gnbjpsgre.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gikujfjkt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/guxnbskpc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/grwaqgcau.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gbllylzro.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gzdoaexns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gtiqwushj.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gegacgaps.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gqybwhvyg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/ganefgqvg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gjgzjwufg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gekdbzhxe.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gmqhxhnnn.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gtcktylur.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gwxaxpflk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzhghfxlv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqhjtpxcq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/glkbozyse.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gmuhvlvgm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grqiufwcg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gzzmbuwkl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gyaehvcdy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gvbojgoxj.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gkynldekg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gqteliftr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gzxznhlzz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/glodlttor.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gbhjjkrsm.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfysklcrq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gftvadefn.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/guylidlty.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gyadgholk.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/glsvfkybb.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gctbppjhe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gzuqpqdgy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmtlkstlk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gjrurnkeh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gpmsdziaa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdtsehyqi.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gcejfvqeq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/grtyisbkr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gfemvylmf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gwltvvrbz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gxfwuztxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/glsodwmzr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gsmxlvikc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gjpgtxdyw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gwlzkjaed.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gvdwxttds.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcfcccigi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmlnxiw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmxqngzmr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/giocfcuyd.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/goglmidzc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpcvgtwlk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/goamhucxa.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gaaidbzkc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gjlvlsiaw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/guwdlgixg.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzqmktvrl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gyjkktanf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gksqejsju.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ggayoxzst.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gxwkifmct.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gplhgxnfj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gjsugpkct.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gmndtfqhf.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gpqwqactj.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gmcnbsgyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsdyurvjz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gwcokrdyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/glstfmilq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghwkgxgyg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gxfohxbkv.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gxwaqelxo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gsqodjyga.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gyyvqxlgx.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gusgrfuhh.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gtuqmtrmo.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gagininrd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gjlyochyp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmtssvdae.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gjbgysdgk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gyiurnkij.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gititwgqx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gldlqigiy.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gyiespgeq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gxzfotaru.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gozpsxfxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxbvsytxz.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gxcduemac.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gejvcsroh.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gubsamsad.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gnnsxhjgw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmdeerupw.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gylmptsqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gftadffay.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/glhpsmdjg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/giufyjkid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gzqyvlbsl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gsannnxtm.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gdpjqezvx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gxqvppphy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzvtedbga.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/ggkgbfekm.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gxowranjr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gnmtmccez.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gormmsdtx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/guxezgcsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/glqhnpxat.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gxebsihpa.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gzkpareoi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gpukrmeqa.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gnptxmrnc.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gnfgjecok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/guchjzjew.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbphscnrn.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gvpunvqsm.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjlabwvmf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzfdrrvoi.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gyexfbhak.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/ggqhfansq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gvglfvbbe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gyuatdaas.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/ggqeniggb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gihdazqmr.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/grczhonds.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/grialrlro.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gwwlupazc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/geilfqwro.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gssllsfah.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/guxqmkutk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gmryehlgz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gouprdbcd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gxqdqhshp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/guhikbbch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gndmfdmdk.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gntxspdlc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gamslaenf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/garajqqpz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gxuvblene.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gayvnkaji.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsnmubdvi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gievvubif.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjcebfvhl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/giuvrhbgg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gsgxmgvgz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gaslzshtm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gooippokc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/getigcsam.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gdpguzjqv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gwbcwguze.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gjifqmyvi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gwyjmlbig.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gvodawxsy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gwzvqwxyl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gykfwpgte.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gojvokgsn.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/giqlkepzk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/ggdzcydwx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbacfpwso.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gpeclzjlm.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gjclfgfav.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gxjqzpqob.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/guvtrkfju.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gibidmvyh.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gdkgwloev.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggeqwzdsg.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gskstanyt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvqwyezek.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/ggoxgqyrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gebpdetqc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/grytohdak.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grfrwmddn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ghprleuxs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gytrtkqyu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gsxqtlhco.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gtdtjrroy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtaczdqjv.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gwfjwleyp.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gmvqtzfqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/glekxenef.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbfhmpmcs.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnaylgcu.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gyumqmvuw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gmaifonau.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gtcuycylf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/glmkseexo.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gquarutqh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gbhalwebl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gllqdjmqt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gwmqgpgbq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gldbqhltf.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gwjwovugm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gzperhpiy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gsphwuxlg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gsjuuysdg.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/grxfrlnvp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gavrcjkll.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gsnmbwpqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gmpalvstm.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gosfrjlip.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gyilspebb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/grurrmbdk.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxypkthwy.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/geyqfuwni.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/godxnjmov.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gcjcuedgv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/ghyeevuhb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmjxkvtji.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gkwuvzuec.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnhtndyzq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gqfrhnojo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gbgejndpj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjgicikat.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gzujnommf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gzsczbxco.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkfeqapc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gpqotrpgh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvmguqtpb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmleofqbo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/guhfmtdhy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/ggcxikzno.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjmihckhn.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/guhwgnuip.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/geywamhpp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gcauzuwyl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gmbiifxwu.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gzrupyjex.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/getiwqswy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gazbftveu.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gjxuffgku.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/glowrafum.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gtsqcomzo.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gpjolgwjr.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/ghoeuypdy.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvcdnvoue.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/goyvkuavs.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbhvjqsjy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqaesrfu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gdobldisk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/geyehkkwx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gqaovahup.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gsjebbhwb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gqeixnplx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/goykvtgve.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlggffv.sHtML


<!-- 参考信息 -->