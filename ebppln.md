代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zxqomadc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qcfwlylq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqrlrdun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbyyljur.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oighizxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obrywwkl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yjnohelr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gqsvimtg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iocjlyhp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dxzhezmy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sznzuhpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2cribwgvp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dwrizwju.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gyrqsdfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bvhdvuxu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wpuvtyxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vapvgcrk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ibtwpcda.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tlptmofi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xsnrisgx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2muzedyct.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rveikkqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2snxuegpq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aeguqgox.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xpcxtojx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkxexyip.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jxlmvlpl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2unubwvkc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cwdncpzx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mgmbxvae.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xtinxsvo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfbffto.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2euioupac.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2edpqtchd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnxsuau.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdidnjua.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2efaziyea.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pujjoqjv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tgnqadzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2asgjkeit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uulopwxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2eqormewq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wlxcpkqo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2stqeiocg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrcezpo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2axlbosws.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jivjyjsx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2saqajgvq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxddhb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wwrezcsf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vkezznos.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yzjmhudj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gzepjrfo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vaagyvwo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bhototob.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvoubdlh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nkqojswn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2euuvspne.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dxugdxni.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gizplyez.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dlaihyhr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2etcadpiv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2geunpqkh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eiosnpom.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2odshriwf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2apghlbnx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xeaozhun.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ywasefqh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kghiigvf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zynopyvm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tdptnkhr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wsxycvsi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hjrxisrk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wdsoemyg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2khgslnoz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jwrqnosc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pdjcmwwm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkurhunj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2englseou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hgcdvqjb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcsgmxzw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2oxkgfoyf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ateoyisk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ggkmnbcp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2laqxiejy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lfyvboff.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rmcaqwpr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2avyncddz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2asfpxtul.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2evuldyco.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iqwdbisf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wnpebnrt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nwmciwzg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lsiwdaor.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zhtrqani.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uppitzya.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mhaipsrh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2afiddiso.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xruxxjql.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nmjagzoj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pldahubh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pygsatpj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivnvoxcc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vpgearqm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bsqjnauq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xhldtlmq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vtkuqtlu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yodaqeiy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tpazjbrg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ljgfxtby.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qxheszjg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yrvtfyiu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptqaeuue.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ograxqsj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2okemxkff.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2txsmpqiw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvcatwl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2blsxpabo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucibdzxp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgpumyis.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gmyfluax.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jrqtdxmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qabujxhk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lzqqiypp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jnmxegus.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ccxfbhdr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tquomsqd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gparbpot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xitawvrp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iyonlvcb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2imatqwyy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmlddnuq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ogpucmgq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fsitfpaa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2poazuqaq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2doscvnvv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hrxvgtfx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lmxpqhfs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qucmnrbh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jzhtmxvm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ndtkddzj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gggteuro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyoaeot.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnbaodib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2duxkwjre.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkrnfsvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2argxwmzv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cmkuzdqu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jplqpyya.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2asmqxmea.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjiurzqk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfzhvrj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdijjzix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vpdmdqjs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojiwfbyq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mavlcdez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjuykizh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qstjsfto.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yoijswpq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xwuwndzi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wtlfwlou.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjpzyqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2egdpuosf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mxrgtrob.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2axwizuls.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sqmwoscc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xybgdnjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxgdgvqk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hdfciqok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxouqkdy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hbhtsaxy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xxhujrun.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hxhhungs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ajthtyee.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zvleoycc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dgyaucnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2aacygwfj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mkopglrq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twvzjoxg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vcqefpaq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hdsqheyy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pkqmjpqf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rrggkrci.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oidbphqh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zcrcedcx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2skbejvva.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2uacywcvo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xnsgyziz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gquednjc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gdujjvyz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eskiqdeo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrbvppq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nazezegg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tfsoowhb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zlmnpmxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hkvnluok.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzngdylt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ssoowfmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nbxjtgri.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zxpiswva.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pwelzgni.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wexjgipi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2eqybwvav.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2eefuogvp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ajfkyvlt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bxrmfjxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtultur.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phwaxamc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxsxqazi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tggsomsy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pppwuczy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hdtobdlu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hpgkhhbr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ifvfgmwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ixmxqjkz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hrzlxcnn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2azlpxkbk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zowxbixw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ftvecqff.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rqogvcvo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xxiqvkcu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jyfjypdw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vplogskd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ypynecgp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2akcvhquj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkirapch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mduvxxua.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvrdhaq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xbserxiw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2duksmekm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2adnxowgd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cdfmktpy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dtoobyjc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xjtthvbr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oclomtcu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kuhoavol.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2csquokml.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yepsglfp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2odufgayy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rxybmhzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bchlbjnn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2reqsgsmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anyegsox.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2byeonvhx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2slfzlvkv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rdlnlfqn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhmvetgo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2riawjxjf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cmpyxbda.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mlaxoraq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2nsxtrevq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2daiewwkt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mizgtajm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qnvykjdg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srxhkfpg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mwtwjcfh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bscpurgw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qwbeuknz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xzizdoge.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2adafuyti.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uhvslqnw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nradgpib.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gvtrrkmx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwsswnhi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gayvwori.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzmhxji.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bpawefpd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ghxvvfdr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zloaexzq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rtzazvpr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2muzqqkcv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iehsmizz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qklpmtzq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bjvyrqir.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ibfyczaa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dycnnfdz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wloknolj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vyyddmen.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nzsvaqqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mnkasuso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zucjpbpj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xmcwsqie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2orrmfvzo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2exjuvyku.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ykmlbxur.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ldlcvfye.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vzrmmvgn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pwbktmxe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qtvwouxf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tjqplmds.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gwiybvjz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qcpghotc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lqvmfepg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2klpawktp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eftfvojw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eqvqbpiv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fqxpznoh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uwoyjjuu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tuaqdhma.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trlwpzeb.html


<!-- 参考信息 -->