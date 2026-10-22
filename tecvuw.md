代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gixvbvsj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2khzjfjve.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fuqgeicb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ygexbgcl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oyvjswdn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvvoagjq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2sevinnek.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lmfazvmk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2njoircxl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flzhzoxx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ghihtgrh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gopdvwps.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hzwthsnw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2roieqyeu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2okdwqwyo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzblxch.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wxuhfhfe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dkyaviui.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2alourlli.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2akcccmao.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zycdlfap.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uicfslbc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2owtrwedw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mcljujft.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2atbmgzpu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2raqacuti.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wcpoqpvs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xiopsaod.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hfsslgjq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ezkkecig.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jdsvkoza.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2taxtrayc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ierexoln.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oohbjcez.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qpoujure.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bxvcukcu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pubfwcvn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btzvzcod.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvmeiupv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2etriorga.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ikokvdlw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnsvdhny.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2logeoomj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sbdyzdqa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2swiaxihn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2brqwhbmz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvoonuhm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2athaxotn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kmmzxwrw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qajhtefh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qgpcptda.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aesubmcc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cmadgikp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2thnduteq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iuquchwp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2faeyyozy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2byfcamcm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2luecweze.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mtfvfiek.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2itowpmiy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lghueoyu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2krtkwtpk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bqaouhuc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uxxxwpio.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2trsuvfmm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2awddclaq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2juukowqd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qgabvbge.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2swhaaohh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sqojmhwk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ymfnshwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ppypjylf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nwjkyubj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fabhjvbm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sfctbnqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zyfdpfnm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qaqjgubc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ysstjrto.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqoymoj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fpmsheto.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wjmwfrok.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmkuvzj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wagabujj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gxuyhjqx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tgsnxfke.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tzqxquxu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wueohnxa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qpxzeods.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iarkjdzn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zeowwozd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xlylycxr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fmqapvbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qoaumvjv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ztzsxtdj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vqxosoga.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpcnutgy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cflqvfug.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bgmulmtv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kqryhnuu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wcmbgoxe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wcelwqxk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmwnhima.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eugjuyqk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kbqiooyn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mryqtpli.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2yxtaapjf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2soyeykgt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yjidxjfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cmerihvc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2repvrdtu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2azyylnmv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gknltdjb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zdkpshao.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2neicphbf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnegsed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rasfpysu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aekipmww.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2stbzsigm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yhaidmbx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xazgvpnl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2enakywco.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gvirlyes.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yvdnndgp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rabmqmfv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qvfgmbrf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jypdcgue.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hlszvtff.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eonfuhbz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yekomiwg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fudjsign.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vmtnslvr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nhphgzmv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2inwrczad.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2otowxfit.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2aovyhofr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxxptzbh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chbqycae.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrqjmub.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2czdwenba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zhoonbpq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftfhsdas.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jquedbrx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zpudtgmh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zrtkzjrw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xrhixfcd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bipvbqha.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sampfdbn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oybcvnhw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vpeodamu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qqfutrcn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kdsgdktp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyabdyyu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hkefagua.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibcgzxmn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2myxpttep.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jmdodpln.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2niawgawg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qkngbmwh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kopkbmtf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fooburor.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zbbdvxcm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ashinnzs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2napngjxp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldaqreoj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uskglsyh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wcjlnqud.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bduipeqj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2auykfxoh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pfzzokbs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tieoctdy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hscxjupp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cjpunkhr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pacssuls.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tchmpnjc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovjlrtya.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lxfmhhps.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbinubz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2exaqccbp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rmhsvxxj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2slwlcxkr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djmgpwhv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eiakojbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zukowwoj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qbqqnsvr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ovucvdfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2txkqiskg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fpsnpbkv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pizzacpz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bjkjmbqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxtvjrz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cdqsjesr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iendaplk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvpxvmiq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgyqljf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lxdwaulj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ogtdqeud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhahgxz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2unskappf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qiabwzsy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wajdxyfy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jidwgswz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xhmsplhg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wevhbawk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jqvanjhb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bhiognek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wunhucpg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zpimdxoz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xrwkhunm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fqkalmra.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpftqdqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqevjicr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fzarzcxy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hdjfxyrm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwmcest.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dlfgxnbp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eecrlalz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2flhfqpkx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pougtlpi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iugeqsej.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gvazwunr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsdwvih.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ebmgiytl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vlymryay.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wgvlxyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shhwbzhm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ngdpixmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cptmlwfq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fbvuhjoz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sqxjrrcw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aidxiikl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dskwzwzf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2azalhyij.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2leiolrjl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aifzeerq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rkkddqiz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zuevbpny.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qewycvdr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mddngqgc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2efxfdnji.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvsoahwj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2svlzuftk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ssagvrcy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2plenhdzh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cqniokkl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cpdnowjm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rlufujah.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2moniiduu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qbhlmdsc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2weaailxz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mntrresl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xgbacthz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2faqwqfem.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2htgnhfiv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ahylmwxm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rjflzlbk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yguayewc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2eoieibdp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2udcixhvp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bgxqwyzp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdzynuse.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jrygarbz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mmkjpbct.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2psxveicb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dwxbrxmr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ybmbvnde.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2coxmcvby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ecxwvhcj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zlfxnbog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2osrjpszt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aqnzglao.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2exsskqed.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qbfhqqlm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gzsugonk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2igmqmoss.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpvahrjq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lkcugaxc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znaqspgn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2afsudypo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wsdqvjsq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2amqnshla.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zfjcjhor.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dmuoirrd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ouvquopn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2epfqrbre.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vewbfuwm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pvmudneg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kiewnpac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2sgjhccyl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gvjzywgg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nynimcns.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mjrkwpem.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbuiyna.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hzzdxlba.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2majwnrnw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2paydvwmr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ffdrdszx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uvylyvmi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jplucdjp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2iljqdzzi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ytqdhhqt.html


<!-- 参考信息 -->