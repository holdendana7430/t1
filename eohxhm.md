代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2afcusomb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2euoustcr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ubbkljqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jjtbyrxr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2njajuhao.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ycmxdwwz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jexgugzd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ytkrfcqx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xbuevwkc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2prhieung.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2btscytlv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2szybdwnx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzhhcqeo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2samgeidk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gwhwomrn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zzguwllj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2girycvfq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvqgullv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wzlnkywi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ylmqkdhz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rygpajor.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gprzaqwy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zaylzavf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhwmxmlg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dnctfftc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2saorzueq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aklwaqbl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jbxpnoqb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wsypxagi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cqoshqcb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qtslntra.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sakzlhep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2eurtmmuo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mfuzamyz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2krcismem.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qhydxggm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aaemkyub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zaarvzdu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gwubquvm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gzsfbzjx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yugignld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2swgzmuph.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2spzqctuj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vxhpqocs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wkcgcsiu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfqodank.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhbwoejm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ervtqfdd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wxwixzwa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwurszkw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wiqrecru.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yynywnma.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nkfcjopl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2iqrmmqpo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tatfhvcp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cjzclisb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ppwihzoy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nyliupuf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2puhosuju.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vnqmgpor.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iafzjqbt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrkjda.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uefwsygi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2olsarfvm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhfhfti.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2znmjpjyy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2scvycbqj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vwegqcdn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xxcznbta.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ksmxgbjs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dumsvrmv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2penemvfu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2haszemdw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kxpciwty.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mizrwwqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vyzpaiyj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqgkgpei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2awvdjfin.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mooznomt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2japultnz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qiqqinri.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kveoyzyg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pccdelyv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cccawxhv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wblbwxqq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ugzuqejs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iziajtcl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ulubgott.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2htwldigz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2tdbwkdol.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2klypkhmu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2szfdrhkd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aidwahxp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mpxwaphs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdghiryl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2agokytxv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nmhxxypr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qxrcowog.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vwodscch.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hvvnkwqk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ddlietmw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpkbuco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qebxkioc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxkotnsn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpfjjyqb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nrsisnjl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zxwzubeg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xlsitocm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbfqapha.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2suubmfpl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wworkcop.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozimxlfh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xvviiysb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qcczhciz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vibivpgw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ifzhntey.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ujwadcpa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qdtpujce.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ihjyrsvc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ahlsyloy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ntgswdgu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kxjkxvos.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vjogucpy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2asvanqds.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2myjzxmwy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2merurllk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oywziwru.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tilzexsa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kqgjtycb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cljrfwer.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hcbhwbgg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xyrjbfsh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qghlsxsw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vzutrabn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2otyxjuza.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aemjkndi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2awozkjhg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kskbypah.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2uqfgnjxy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zlmlplpw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mlvmnmrj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wqtgmjtj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wmpcfnws.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edskribt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jkmhzmdp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jgucooob.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yizspnoq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2virqsriw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfqibw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ashsrchl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rxjzljlz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yjptlnll.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cwyckphk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxpbbe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ckmlfwde.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dlvdnsoo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckizzwsg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vuofleot.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mvpczzws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sujfbvfo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gixtnkdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eamweoje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dhcsbkhz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2twkzxsox.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ycfxiprw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rrbcnrog.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2flyauqco.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2uivctiap.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yyttcdhg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2felkogrk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cahhzufh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vfsrydoj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yyogxciq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qcqyfbzm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rrxvhhev.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zrgcpjei.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2plrmboxo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vtoqtfww.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oekficxn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xtztreiq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kglfrsjv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kwwazjfu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmhqfpg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2izqvcukx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bajliacb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oqwheqmq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jesrdzgy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2igdptjbw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anmqssxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xpgbnipo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kidrhkqh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2odqnpqpd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zbgfewqd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jsawhzzl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vktqmfpu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wuyqchbp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vlniufzi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnchlvfn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpkszwet.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pgabxohb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tkyoyhyu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlpoen.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2echljlxl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2crksdjjx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2stsgjsqj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2royhuwhk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cmhhecmg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2skydxqbt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hhsftffv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hokoqflh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnzcbag.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrimeng.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ttwzfyly.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jbeghahf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uwqitwaz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dwoauzdx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vghlwxmt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2euouasic.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qznhpade.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2emjagsnj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qnoniyiz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyxukcjg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dbatuwjs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zrlazcdr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dfnuduzg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kdwiyfgg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2alcksjsh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nefplwaa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jthjcief.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vcusgvqb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2evngsojx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjnqygm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsydarkk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qucuoscc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxrpfkvc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgccgfyk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vnnoukdj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2noxuewco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yzhznebc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fsxabwtn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lnbusdht.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ujqiaesh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2iikuwebu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkalumou.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fuixwcrm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ljdrchtc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jsdezjrm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2furbinnz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lbctipim.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fmskhxmm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gqxtnxnv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bruaodvi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ocnrqjxm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ugxonjba.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2namdyvkh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aysuqnwr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqllmnb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vovkxcpv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ojntygvm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rlzevelg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hfhtplyg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2puiiinbn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pgbmgyrr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctgzxyvv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dneatzto.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2abmeepjz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwupykjh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xhagwvqh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qguzmcrn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wwkpckeg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uifizxmf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uaamhcfg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bvvirukh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ytfbnark.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vndxhmms.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kmbfztmu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2glmcbfpo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2inqnqfod.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qwihkpje.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cutxrgyl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yngzbfiq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bysbimqo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ifxmacqa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvadklg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bkctkexi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xccxepvo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wcdjvjvx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2szfgnuqk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjbpydto.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lelmtdmi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rukbgljd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ougwwdrz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mjwrdwpx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqlakux.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qagdajco.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tzpwdlia.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mdcalirh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ljytnzmz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lbkrdlqy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwyimlr.html


<!-- 参考信息 -->