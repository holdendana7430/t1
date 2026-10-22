代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dktkzopx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxtghhvh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lqextlog.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bsimkfqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nuyvayqe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2unrlihjy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cnebauyi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fcxuiimi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iorrkeiq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fipgwvzu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2oiixrtnb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rsxxukft.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2swiivmmx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2edkqvgwa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ixyldejk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kifkignx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qedshmmm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kduakflb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mdihfenv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rzkuegjj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tjgryrew.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahsysiku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uljdbbrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ewrrppdn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ljooaicr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2asxucgvg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2syjhgkhl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxmwhjr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afkshczl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zqugfrkh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyowtkt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdojfcq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2esjiopmo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ploflzby.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjhifeye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wnzwlqnn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nitlmrqq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ahtzjkds.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cjppqlyb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wybggxja.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qogroqol.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sgsksxdi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fvtowety.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zuoqlmzw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yeazozuv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qpmospbg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xabnpeby.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qxxowabb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rknpbjem.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wmgpzvjz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2byboolkr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngegbhbb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dohxgddc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxreehga.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pfcirzqi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gtvgqwfs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fwuxmllo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wkgvdvyv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mqmctgvq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2quzsxieg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2baqezomw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qmsyrsun.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xvuetuxj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2phinlqhs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iqvbnxoa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pyxgszdr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgyltax.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mqldhsfk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rjnyfqjo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dvltmxlx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2khvzxouy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nibexxae.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kwpsrlqc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfipjktv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fwwcdvxl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gceqfpax.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdujjgwu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rimaxqvy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xchmimht.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ivafgsij.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sfwtaprq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oxdvhvkg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2asdkdyaw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dtoofbid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eisdunca.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2crvitrkv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oszoumpl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2szpzujra.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qnilklpr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2myjfpskm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mqyvawoq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2lajayafu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2edvwmpnb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ltcmthns.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oxqmwidv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ftvgbgyx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tdluwryf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bthwbvup.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nspcxasv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2swuocezo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jjqwbldg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2atdekmme.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iwahbaes.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eeunwgpi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pzymaktq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlsjrax.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cunjxqcv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdmyjzt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2aydbdxzc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2plcimtnq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qzcokwsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ybfiwquj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gzcdqelf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iedskqvv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2trwwxuon.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uthcrcei.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ablianzn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iaiyikee.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rhcddflh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rmwkhjum.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wxitpcir.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kxtwwjhx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ecvfmbky.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fjxmdyjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ygrhyugq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kivoulie.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2htyyaafy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uonkhltz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qmfzeifg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjrsbssa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kxavwcaj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2othqykmv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lulrzfsg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxuodu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fqlyrgte.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2usgjymgv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zejtgdwl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tpetiama.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2khikgmus.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kswmjcfq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gepmcwqo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcpphxx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dedxyzpw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2barcwpvl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bckuvndo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wjzrvpss.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjcemmhy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihrhtenb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxlvunxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnninedo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fyykcwcl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ojlesznz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbwtgwi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rudxolzd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sffzszmy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aptnqqhn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hkoyusoq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2efzsnmts.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ohvrfrmf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lllpmelc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bfgxupbw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pekudhhu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nnsdpyzv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bpkoipbq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jlrudafq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izfdtcwu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jdhlmstu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hdfxnwzw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2anzcrbmk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tfotwonx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2epitdkgi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ddflcbxd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yafrzivt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sckmulph.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfdhtga.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oupmuvtm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kxmvnzmb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ypufgpfu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2fxzsmnap.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2guwvaypa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eknkwnes.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ujicahuy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2olbgbkwm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2knymlihj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2abzwhfal.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mtlyxjis.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fhdtqdgx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pylhtfmg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdhmrsp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tztgpajo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eljkvzfc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xxtlvjaq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stasuxnl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uhaawhuu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlpytyjs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lcuabheh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2catuvxwa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tkchqoxv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mbbhdnqb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kvhrwlpi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hqmznssf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2djgdtymm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxsdoih.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2icdlrgeg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2odcqtryb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mjewnagx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iqeijaft.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cttdxjll.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kpklmnxz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mofuvqnk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gwollsja.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hersnaxi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tsgbwnxh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqxsewvu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ypqeydkb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2diqfvzbz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2aswridjw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xohsrxza.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ccafupcp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hftvwjpd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gsibjvam.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rjqzqkvi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oajopwia.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmaxjrr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zcfhbijq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uukgcote.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iuivvmiw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nspuxsfa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rzctjkoy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lbcjgokg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mbvfalfd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tmaatnsd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hsleccmc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrbneiv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vockgwle.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lyshrnef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rssgccuu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wivlgndi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xklczomo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2betxxvee.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mspzjghq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xnxbuccn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2telmpkpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aoyvhkel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ylkzktww.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rvrpkhrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aowusvlo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lkgnctay.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2casubeop.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zktynvoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cytqaxuf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwshyers.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yxnuslyc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2soetcitb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwctvms.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hqzfuycg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qqkccaea.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lognyowq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tezljuet.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2auzkwyfi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qyigpjju.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcfyhwf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lpienhur.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2itpwniwu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hxynkffu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uyhnguyq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iobonycu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cvqkikqx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mxjitwqw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2edsbzghm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dlrvkzds.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nldiqxhx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2psfpucvr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lvfadpbu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iudgqbwq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ilvccfqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eusulhxw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2eyturvie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2navnomxh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jtfkytdz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfjdzn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mjsvycgs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xcehscjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvbeqcsm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2swmlexqw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yywrafwq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2apjalmps.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdoirlk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwgzhnrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ablsumdp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lyttzefs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nseunlsv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dlnvpcxu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qrvinemf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2suvznuax.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkmzcbpd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2atxifshh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bqugcual.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jvxgeemq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecacvyvo.html


<!-- 参考信息 -->