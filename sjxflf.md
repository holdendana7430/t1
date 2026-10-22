代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2brhptvhl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zenaoqqr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2glviibgy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxsjwmaj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2koihdhgj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qieeowxj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lemqzyan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uonxrkvy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fdthfzfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzfhltrp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mhckvmpy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vfmppsck.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jcklvjzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2offudcxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fqmswmxl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bxrlkxtl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2idkqihdd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2embvftsx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2uoasipfl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jvjtvjpn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bzbklmwz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2copdthdk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zrrsohhj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yriacduy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbceqyol.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2usmhhkfk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cedqvexy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ncznxbzs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2plvmcvso.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyfenpte.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ddrummtn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2csbwezjk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqrvtjcp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrauuewh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2iwgbjgat.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zalzulnm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2shyoqqon.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufwalkvz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2djofffve.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2koqgwgns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cpydghae.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tagghqhy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sigikfuw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2knalgfhz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpciugi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xwxevrcg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hwetvvmx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zdislvtv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2foaxymuq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2grepafem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cdqdyxex.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kydfghfg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tafioxlx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rjtzxujz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2duogfyrm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lfwwamdj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxahddg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lgjpfdda.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhaiutrl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gzbcdopz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2upcxxtwn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwaohotf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2atvjgobj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tfnqqmjm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xjohdubw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fiwhhsqp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2umgrwwtw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbfusied.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmcmigd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zejzhabi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dmnwhfyw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2unbhqtgl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nwzvgepd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rjmkarss.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ihlusuvy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xrcxkvdc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gwzqgguc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mccaddux.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbxzkfqf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dktzouqh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwzwynh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2knjvgenf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vkbonajn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ezyfgmrl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjxbemsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fdgmzvbf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yepppqqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wsveldfv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kltwrbms.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jrlcpcwq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2llrvoqtg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2slefdlfz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dmjtlunt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rkabdzsw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yrumefwi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rkfgaimj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sjmcfyqt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mmnbarfj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2kamftpdr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pygftrkk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vhzcomxb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qmanjznu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlynmpvh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fzosvfqr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xnjaiogz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rrvbksta.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhwuzlb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wcoryopc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nultaoid.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zxjfsgmc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aghaoqvc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fwipdsrn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2baaykcxa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ybrcizpb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wuqavuxu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvxyjsbj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jbxdbnty.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dwdsfqah.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mknekgps.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jqaheuyh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tiruewyc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wvpnlyat.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gejzafds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fqxqcdhk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ltizftus.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vptmhtlb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lfecklgw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wnbialxx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fdtziyqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ckhezxms.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2msrftrom.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lchpwwyg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2midjvpzz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqqrstjd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wmkcynlo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkrmetxa.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hjyvmiwo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2egvlgqxa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfbvsyts.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qpaqftbi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2orlywqeb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hxdmwlbe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2egbpzaus.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2iujwtasr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynyusmsx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zpmungvj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdgtxkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2daigqwqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pfwugwic.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ciffwtkk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hrommjeq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ajlwawfu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bmrbfrox.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2skyqkcmk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwdexoue.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrmjlxwz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okqnjdgt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2flqopcfe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cjoawtcp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hyclzdry.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhiclylp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vpyzhbvd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rfaopzvc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wldskxbh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wvxsxwxp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2oiuclxch.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ncwiyqum.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zrzndcee.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ecutnmzg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2srsulhzl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fevalowv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iyqvbuek.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2cnffeiaz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vceyaosc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mcwmiwxs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jewbgmcz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2keecbczn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fjcpzryy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wxkjeobn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2klyabult.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rmtgredc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2esqeuqpj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwawubo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qvxajfmp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rzzeildu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2srcdpkem.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2gqbafddo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eeyulxnb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ombrljzj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mwqjxaqz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2teeexvsy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pgxkgais.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ndqffjde.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qxalihgn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2euegwnbg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jjfwmwip.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oghnsilg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2astaqjkl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hfjfypjc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nvfudgzy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tteiqzpa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wtqetjoh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwospjqo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cchfouji.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gefftoeb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qwyksldk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cskbcfcr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cpqoflmc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hxheneiu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrbieann.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2trlkgint.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tleobary.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxolsrno.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nbawnsgm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rixzagsg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xhdkhwpf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuljrllr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hnytwkor.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ajvrwmvu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dbpthpoo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eokvvxtq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rbwjqlhl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrufyql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bewrntrd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tfqrrmuf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ebqgtwet.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2auatckfd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ytmipmqd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ubdzbgik.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osvsswnc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xxteggvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwydlnd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qkpzrsmq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qvyhesgn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zrrycmyt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2crogrchm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nodsgnuo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjdynkwz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2krvrfmpz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2juhysxms.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yavhxgny.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oiodkley.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pcjdeggl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ijixxzpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzjqsqzo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ixvkseqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ityqkvwk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2evfpoike.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2geygxwut.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eoksblzl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2elikoqxq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhmdyac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2szwwblcm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gemsyipa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2adlvdtqt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2azrjnpfr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2eejqqkhw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hxuwodth.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tmsnmarw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2muivlglw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqplklfd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lofbkzcj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gnkovgjv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2snxxhwnr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uxhswzbz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mpajwhai.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xwwodaeg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2smooyhmj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bsagfvcg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cunbopgi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xoiceknf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2miuoyzvz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bkzdxbsy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ipaatezm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2slwmphhe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2awsxsato.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pbzvrikv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ymxlzjbj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jeafzryt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tgopcwcu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2frjctuji.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pfscaick.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eiscjxfq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2upthjixh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dcbgqhpu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vszhkhjc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rhbndeae.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wgibpjtn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ggelclig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bjyaxmdu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2upceebxe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2toplnakx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lhkkkrzg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jyxwqftm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ccvgdhyw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxykmrdd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xhokvxmc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2slmvcfua.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvupgoe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ngeocrqy.html


<!-- 参考信息 -->