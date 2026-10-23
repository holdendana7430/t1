代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xchcdyyc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zmbjhboj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kazkztet.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fskzlvki.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqlsteiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3goqevkzp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ojnedkmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uuhtbhau.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dqqojvol.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hbvsltpo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fzpngyir.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qchcekuh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cjkmiwat.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zvrrkvim.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3igsgzkau.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wbfwvwhq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jcpwcika.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqwjiypw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3amcayjzh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gsnedsfn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hydjbvlh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhgpprka.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ohnxugzk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3giytrxhb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gbchxzik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wznxsckj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqvkdvcw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufjnjvbj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3erxzrhqw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdethbya.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jnqegupe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3awncqmpv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxakvlx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zwdbdbmm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ickproun.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rpplstjn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ecymvmym.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gdjgiikb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nnjshisv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mxygcqlk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfyfccky.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwyzrrsr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rhscamqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rvewcafc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hkhltnjl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ufrgpeef.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3yqbqoizu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uyxcyywg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kllbpxme.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uxbswknd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cyywbbmt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3psaqlpgp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gweqeere.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qgntmgjd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eyasdibd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gvhijfrh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cdgcbscs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tprklvjf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gpalfefj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmtlmz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dzozqziz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uzlkazjc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bavvgmww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3elnpiaen.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rsrogtdt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3opfgujen.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ducbnsoa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wlfkurqm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tlgigrcz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3oshweucu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rsllreoe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qhlpqujj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nfwicxyy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fbrdreea.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tazeinfg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eesucvzl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xitgjuts.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fkgykrgr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jpgjqdxc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zpqyfvwe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3iedmzzjz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjudamfn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nqsdqdnh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrhpyhek.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zpaffhzs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fxnbbbjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3osoljjpr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vcgofdtp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rdugmuuf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tanrlkdn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3igostjcl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nbqmnlzu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3iglbnlfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ejygozki.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pekgivdn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfyjqjfh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rbfbvwae.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qokhlwvi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbyavpvd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dtgfozoq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3georlbrk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kfshagvi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hpjymgok.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nljnngyr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3urghtofv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3pkycrppr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twsrqinn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irdosivs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3asborbjm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fetonjen.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3clxmtiql.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3oobtrebr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3njapkvbt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ylbcouae.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uhdefnrr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfeecui.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fylbxmai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mrauctnl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dyssstqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qtykgpei.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owsphegy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rashastl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vjjcesek.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ojxrsaub.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lmqmgsai.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oiphssgg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3drfwebzf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3opaywvkk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3faabtabh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbngnjby.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dsmvflnm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hyufrrzd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nznthdjj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3azrdpkxl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ptoirxfm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sgcmranq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gjkhtjsh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3futdjdus.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xbhynglf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lvliwwdg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jleatjut.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ytdfmqgp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjwihgli.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykxxbrlu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3muektffk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oqbryqzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jwmlowhw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xlnsjhca.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bycytjzi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zoqdwgqv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lpgykhxt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gnycbbsx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yltdyltr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wkqagnrn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zajkfrqk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jeyqfowb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mkdakisn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3taignvxk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lofpjbew.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eixrosnz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzyygrae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gocbxstn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhfeeplk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xdmibqdb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3erjvhapx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rtxnvlvi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3buliplja.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ogqdsjjt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3evcfsrta.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rjypbktu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tbosapar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wantctep.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dujmjjyu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ippxxvjq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fwgwdxpi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3etwqhjwa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3adogakei.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fjrrnwdt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iibjiwwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gxwzspju.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bszjoswc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tvttghyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kmlzyomb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tvwaepbj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3marrlqgl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zplglyuy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gxcqaicr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vwubajfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhojnm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzknxlhy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3msfeirpm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrapxmx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mwjrsulz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3onumxrbp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eaxkjiem.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wqdhvkux.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ymmbefkw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3innddfsw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dttkuhhr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uhncdidd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fmropfos.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jfmrpbgl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3onjfbzec.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqpxslh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxcpnpqa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dymmdvxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnefbpye.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hajsaxdc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mpwvyoqy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttvdqkbt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yymxnfjr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tzkrfyhm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwpdhjye.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jgasuntr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rwmrtaor.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmqyjnlt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbwjjsnh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3otsdrgwa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3couqyebj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yfgndiko.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dcgtwthd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zkzxgrvx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iiixgcmh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vtfnhrah.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iedoldxz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vcdwntge.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mxrebtja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3meivezkg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bgatisvl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnrxpixm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3esjctnil.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qacthapi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3efooehyh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uantcwtz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jtjrqjjj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3febnzkvj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vkfyikaz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ehmacptf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3somjmvgn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qkgwcwbi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qzfucsmc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ggospsru.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oegcfoue.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rfnbzfkv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhiibbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fncyqvij.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mbrkdrqo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ieacmolf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3byhilipg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xvxpdbxv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mprdagpd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yokbgudo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3igklpmeb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uswnuupu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvmujmnr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dupbaaji.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bnfbbvow.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zsowxgzn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tykzvpmp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3teuccchj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jcygydtt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uztiownn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ulbmhnkj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3squevlrl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zzeyjkgf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tttgsqnf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3mnynreez.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nbppeipl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rphotsbs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgptnxj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lcopwcvf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwxyuzc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dkpqvkco.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bugtmote.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kdsnfkiz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lkwbqnao.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3muvgkrbk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3igeqlceb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hdkthssm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dqzysqco.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tifneptu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uojdrjes.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jbotpiwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wvxyvbht.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hllfmdzj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqxhahha.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hcabgtfg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpmvvsd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3eiaittuu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cipouuxe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3laktlvte.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gdfhtpxc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kgteynqc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jwupfnic.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdncvir.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iropyquu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3oczatgjw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yymjkvjv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3okgqkpxm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hkykputs.html


<!-- 参考信息 -->