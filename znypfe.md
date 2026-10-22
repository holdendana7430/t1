代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzvrewpq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihpbgiea.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixtjmhwo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cakrojgv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hjknjczr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jxuwgmos.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kaslfzkb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vwhmupim.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ssrhptzp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ludguanh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sekoeeig.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dshathzg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hdgbsfuu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfyuiziq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdynvrke.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zhabyues.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwpedfi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hlzyvpot.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lpksmkhm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zunsggdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kguvrpve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lzqofmcz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ofzmmgve.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2odzdfcmx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fonenmfi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bnchaiqj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hqshxslw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2viugshcc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdsplvec.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmmibbsg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ndmysyfp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sizvfeor.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hugeynsv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uftsesoe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2llzgaajb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ugnhchbp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iftxpekt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ikbtglyf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxoikgn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vjknmpvi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2abelvesp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lzoaegqj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pdvgngbd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2invpmqip.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jlxewvpz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xtyylfqd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgmwmwl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2czyxdxci.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xyekagyy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2rgfeswzi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2waoujkkd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lvdxbjzl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wivlkfcy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oaucxjxd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ixtsgwaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vcwiddpl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uooqzlrs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nglzmgdk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xfdkevbd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jqkeaxfn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbttlpye.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2exfnjgai.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bpxpgiqa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vkyneebw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ygdttleq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2frfhearo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lebwnxov.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqoaspm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fqrhamly.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2alubsmva.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bzktujwo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2yjprpmnx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2fretnqpy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iyywpelr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmxgetzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2irwkcnxu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nybkexod.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vjhlyzba.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rbqxycxt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fljnnljh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2pkonpdxp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2eoimkmyk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cqwwfion.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kmzxiujj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oyrgjnii.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2adinplhe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2owabweol.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2apiwwljt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytuwkxhs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lhfmudts.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2njsfmtuc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iuklekea.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iisdbjtr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wghofnky.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzyexqtc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2corcyjys.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cvyiqxvw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nzrfzarw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oznydnfk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kjsaoesq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ynjxnzzq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ykqtpphd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xwnkzchv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uycazoxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2liudhehn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2daascpdt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2npwxpqmp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlggzbjs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uujtilef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2stlgugff.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ajbwshwa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zmzyqolq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qkzfwsfz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wxulhawl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cgcnliwr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qkfdipmx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbhucfxe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ijystlav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jotgkaww.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sckepvdq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvwviwv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tglsnxow.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nxunrtwk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eslerfoo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2laraxvhu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tjplejjt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmbkxk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvixzzfe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqhgljsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvrkurt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbxpydzb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2smtgalvg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjvsidow.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yvupmewt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uqgzmsuz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uvtfpfsc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hfbqezin.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2efxmepvc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yomtxtsk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dqcakjmx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jiposvae.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2idxlxsxx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vidzjjbw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2btywbmwv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2trqnofjn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nfygatlk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dsrrhgcw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pugmzjxx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2htmxalsc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2psrktejc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vavyqddv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ujooippy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uzxqnlew.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ouynufly.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlgetery.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2djnrause.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ojlibnoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sqsxomzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2npkjjffe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iuqaczwh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wkiiwydk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hlrtqkvm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bcbllsza.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vfzpvgqk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rsqojoer.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvrvdjwh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrtnbxbp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kuwrqdsd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dfcqptle.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ewxgynyx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2glqqmzgl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iltlbyrg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzigsbc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qmojdizy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lijvmqwr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ywkqrvsa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ifaxuclf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wvvipxsp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qvqwwznw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2feyejoec.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bkfephwk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2godscuhu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yuegcoib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aqjcmffc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mooaqfks.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wzzxqrtr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2weqnkuwx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dbgkdtrf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xhzvktlo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2puqbfafi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxvhcja.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adffokwv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bexbxczl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lritrxoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dyiskqrh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gwqdjowh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvchgti.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ikjyguef.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2oewwcrnh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mcjplyzh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ooycerpm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pbdrxpvm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yrjqnbjj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ppmyibzd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2smztkzpn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2droihcow.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pavskgto.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpajkrya.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2klncxpoe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jdwcufyb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zvovrwfu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ynxhewem.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ebvfpoyo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aidubzec.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bhjjickj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jwlnlmjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkovlejs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kzxqllkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucdjvblx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2meqleqxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2omneesxu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bpxcimlt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2okzrpcpb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nmjvhsuu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qebiebws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dcgfvfig.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hiuavriv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qarqercs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vidhlmyh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rynbvhkp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2suzxpoca.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tavxuesn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttuswrub.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhtzcih.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xgshnlup.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2epgpddfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qdfzhhib.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qhxneoyx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bkmxqcgz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ngimdhss.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hyokvymv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2znylfylr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwdcsm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pzblhzom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2pqhersqo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2grthrmgr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aiqfbfru.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qxnwfivd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qiturwwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iyypqyfe.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2suztrsle.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ebzccnmh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2amxjzjit.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ntsweufr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qtuvtydr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fppsvski.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ybohdbpz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zqijwmfi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qeokurpp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dfwzksbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ffuscnav.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2saklgisv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ccqeejuf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gcjyswpx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ivdxgjmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbfkdxoq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2irfsptgz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ukzjyitv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikumolja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ukucucgf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2deqmmwda.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xugkunmz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gefczubb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hljdkgew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yijqrqxj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfowxbau.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ikbuvwqn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tmauxexj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hjbowikh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtgilei.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jkymwsor.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgcrrvs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mtuoqnbm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqhmkwf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ttzghezv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ufgdipbm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wafomivy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bggfpryu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uaehuyll.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bihwlpcg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hevjvttv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2laxmfife.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ccjxrszu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tknojuql.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pbkcmtae.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2juncnrlj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gbbseobo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2adqvcpgd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxslvprd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mvtgadup.html


<!-- 参考信息 -->