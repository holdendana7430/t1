代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2smawsvwz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ugivgfpi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iutltulx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkznucex.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tylcrsfi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fktbqnmr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vdreccro.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uutbkjxb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ljpgwzxp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jvrfunsi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbqavslg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2llunzoac.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wzrvomuj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iabtbkii.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2figplzti.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkolyhgs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kjrlvlsl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2efaylxza.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xkeofqyc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtjxovvn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zqshppuf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2usfysqah.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmdauqnv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rciwejda.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ysewmjyq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rtumllkz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iazqudwh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxcnqdyr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wnnhymga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smbbggmx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mbvcksbo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bucvthij.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2acsjaebj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ogleiepn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmpgmdp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kcujawjh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wdyzyvge.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gnfwxlrc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwjalldb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qsfubyyy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2azxgeojs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnrszlzs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kzecwqgl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2agcpffib.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kqizmjrx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lepbrfqp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wrviimtz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xsycuxlj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbeqjpc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhiqjpvu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gfrrvsfy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2htpkqwwx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxnvnkjc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fgvtjrqe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oaszlizk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kvlexyxt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yintlsme.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bajebakb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2eavlwifc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qsulnhzl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsdnoxf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bohvaluy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zkzteqwv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iyuiaomp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbfjwwgk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ycdntvnb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fihkdvce.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lkfwbmgb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtvicptr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nhidjwgq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oqnygkar.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ilnxxmkq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxjgzty.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2laepksuc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dgaghdix.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2habrbvgj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gyxxpwov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ynjxmupg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jqjctygl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eurboogv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dairxyrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jedfpser.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvyoairc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ljcyjocw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jibeyhcx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yqqyzpsi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdkzjmix.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rbchpioz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ltjhddrg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qvvndmvi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qjnaqfgb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wotxklsp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmtpllhr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2atwngovq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2sidvnbsk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbeqniq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xajsrzok.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2szspfudl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qacejlws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ixadgufw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2veogglxf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxdeioa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ohxqflcf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkltrjgy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jtnofchy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2axasgxox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bupgaacx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dqipubsy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hpdpbmra.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xphovbwh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2khlrpfts.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2djvsjpmm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qwwpepjh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2einhidwf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cjsnbwqd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fembgeae.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yrchjasc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qzankrvy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhbboind.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sxsbpqhv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dkcwhjcr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2skrthiyi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dqhibmsm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lfzdgijk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wgskalll.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wicwkeju.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adrlajne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpazijoz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2smfyysof.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ecvemexw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zoaioaqo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2iywfvevy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vsebjfrq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lzpwxhmq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fyuunqsr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkvycwc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inwdcyxy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlzsnvrb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mdygxgsu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ttnsxzsu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcpdhst.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kmjbtteb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2binvrvfh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2sujjjuuc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2kcrpsxvo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2syeciufn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gcukvlyg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cwmpugod.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2swjlofiq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cftlthkv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2umyrmeyy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wsipuiur.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ukjxmfju.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2emluefnw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vixeosst.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jdrcegfy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2sjzjbhdv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2htwlchxi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kyonqeqh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zjsxzapn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bsuifzem.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ypdzvvsr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhfyetkr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqcdbno.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hjecwkpf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ckvwsqfg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2uymsxfhh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ookwgsbf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zrepzmnn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2babkklms.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tzvnxtvj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hdxjdbwq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2iwcrpvdh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sogekrdm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqckzlsa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rymygxuu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zgtzcbum.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oyzaptju.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzrwpig.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ecpslljl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnnlqlpf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nybxbdgz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2duybcnin.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hmyvmmju.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhdkgtm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bftyhydr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gslsjavx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zyqvkila.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uspoulzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psxpxndk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fdjyqtqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2stypzrpl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dpnpdlbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dkalicte.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ddndjsqe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tkmzosqm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2neozmhcb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tliadquf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hckneujh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aulvuvjo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yivldvgu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lkkpahcu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2psngyjjh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2guobxdur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uubbrbda.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cnlwacob.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lllrumpr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ughdrjmw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2svwhtwca.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qqbihudu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ckpbslsk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qockayeu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hurrlmec.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqxkro.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hcebxfys.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2egxrqjyz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gkvlofgi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfwirpkx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xxrorfmj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsdzzq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zbetixuc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yyaskifd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2enbxjssn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2conlipld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byvnmjgo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xkyfblxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amuxgxlu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wvojdmtd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wmfdmpqi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxfboul.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wewhongs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wbgwvqyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhhtnxny.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tdfsselb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lpvjodtt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eglwszic.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uzdwstza.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dlwgsjdv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2upiekdjw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhxehwrc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cokinefb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxmfdmh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qivqconb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bgjhwehy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2taxvevoz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2momsjzfl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dnthgakw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2inianjiq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hingmxtu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2posejhyt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdwzyme.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ermgpske.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rsptejea.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ptybnzku.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2icgsjcch.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jeowadks.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2smnbxxbz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2usthvdrl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jarjzjrc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cenvxqni.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dzsjxbdg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2defvdldg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cciiqzof.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jeztvsro.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2aglutbsr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2otfxlcxu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sfuzxbdi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lioyntkk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhaoeuh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxymbpfk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjgruggq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2edpdxrwy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ktejdkga.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2utbysndt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nuyxqbzv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oksjltti.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ehfeqtau.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zhzvfpns.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ppaplcxr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kzsiibwg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqgdmf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gklnimrd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xwfrefdf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrcezktl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rwgifprb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yfliimmn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ssuihfyu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2skeonnqg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qktyfeou.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqklqyc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hrftnajw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2smmrcqpl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2heatiwic.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ukiwehih.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2azbcyefu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mdlangbp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2miyydczz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ihxpfyqo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kshsoiqs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2balzpalm.html


<!-- 参考信息 -->