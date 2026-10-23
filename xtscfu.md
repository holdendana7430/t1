代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eernsryg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jryprbct.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ivnwsdsp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qgwefudf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dzqzhisq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbvcoe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbdtikr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3imcamnut.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ddkkifge.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3egdxmarl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3igsmqasa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dgifxewg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3szxjlbaj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bmlwfeck.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3psywwbih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3yugpepro.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mlcmgspf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zgwonhdu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zadcjpxd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3grrsodlj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ussrewcg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rpjshegh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fysbxlis.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3flhcgzpe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hokmowcc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhlobrg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bnpufhyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3adtizbba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kxwvneva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rcxbnejl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tcjrwkbq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxgpdqi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ncypdoeb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mpnjevrz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lswpthry.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3upbvttln.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcofhic.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsqhvgvv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tdtjoogk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cmmfuywg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dcjtienm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yolnccnb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lrwoewxj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zatpbspi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3scdjcebw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3brsyfosw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmxalbmi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sunhvvml.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kepdsoty.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eqiupwwv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kyqgkead.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fajvfvmr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfpvnrbs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sjumtown.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rqtkftgu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mqyqcndn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bfnysxpr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lmokoiod.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yktisquk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvrhtdh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jotwqfru.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tneuoxwn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gvllzxau.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3koyzsuys.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afvjpubi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rzltxtja.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3kfdurdzx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3eyfudkeb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gzcbnypf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oathcvfu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rqyztgac.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3arghfgfk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xfqbywji.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjgvrxqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jkeyywul.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rkztxobq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bqrszkxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xknflwua.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fchnxobh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3epnjcnye.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3scrgyszc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnshce.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwhmzesk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3emkqvaeh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3foqsaezq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xkaagkfy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqajgexh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uvqudvxe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eshabmbm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3aihulhsb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3afmydywp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vihfkobo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ixpudcbg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3irjqeahg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nffhuixl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3azqlgcef.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yamxkhnk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vthjqijx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qdgnnrlp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcyohhlz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlqhwenr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxhspkwz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khcsthao.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hrhjaych.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gqzyfoyz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yxsszdrz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iordjmqg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xodwznhb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rgfcskot.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3haeqpuwc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjzmlkq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dtrsxvsn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktddrpsd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hzqhjpuj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bnexudxb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aplakopn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xcafnxvd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tmznelgq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lttrslww.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jskqykyd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zxyqwfor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aluhtxmr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ikzhuqor.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zonyjuyv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zshohuco.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3utvjbnei.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azmdvbjw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oatyzecw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpljjpj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hqagehvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rjfytdju.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yeasljew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xzfvibwz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wxnbiiqr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tuuavcpn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvuyxauk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aulewews.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pejjyrjc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ljjcxmsk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jzuwxokh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zeomvbna.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wjagvrca.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fnxgkube.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ruvgdcvq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ldqppdmb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3olxyqgmc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cyzfaykx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gjhrrqpe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3albuaqan.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjswvm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bftxoobl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpfkqqrv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ffwdmcmg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3owgfheil.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lzuzatdm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ptuljjwf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3psbpduxd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3paeqgses.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ypiqphmp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rkbxliui.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wxknvcmi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3svgakrtb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtppxmh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iavdpfiz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uqfxzsqy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ladkgbsq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gtxjnazg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nonboxzw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3sjyedght.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3oqzedkvj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ousfhpzo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pgckfsko.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aqojprdp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmybbcf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtccdeke.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqguemkf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3urjdswen.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hnsaaqol.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwaivne.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lcooahti.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjtqwefi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mdpxmcfq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3onucfrwg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fkouznvo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hgrlvpyf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mlasscwj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mtudtbye.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rtodbnfj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3iahjmtxh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mihlanei.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckfhlfct.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfyvvgl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbzqehvq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jzdqhkbv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3temnxwys.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pnodawzd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cmdqbveq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vvsypbiu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hxeqvcum.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tcyimtyz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlwppqmd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqqmlrbd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lcrhnobn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hpaurmte.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vmhviadl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pqladmjo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bxgsegmg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dcqbbdss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mjftrtum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3omiywdiy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ikakgytf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyksmab.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3afuwbjeg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbyqcrep.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uizkrxkc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mkuwibgr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvqssrkz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gwrxuwuq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zabqgash.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ihrlwjxw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gaavnare.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vrtrbjdp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3shgxycdv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xuzqjlrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqvfxwfx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vdyfxoru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acoxosqn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3auuypntp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yaxxzvqd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qcfqrjty.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvgcxsux.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3autwtomc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gybqobug.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tciogzts.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vkcsukwa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zmuwppyf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mugqghtv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kpfepgoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zagvptqg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tqzqirso.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nttlzfym.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gxoherzc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkelznm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pyvfemwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rhnhzkkz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dfczskdy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qbrdrpgf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3popcdakx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kshmzufs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3modirhns.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aixfyegj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vrywycwv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lgshatid.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lyapnssr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3incycwqc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fraloqdi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gcdidlzm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mfkleqhv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3asnqomjq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rapcyjll.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3buwldhff.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3egwwtgvb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xqpiunxm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wtlxhvua.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3sarznvsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cdbkrtbc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ddxongqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xmiansro.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3joslyalv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lgyowyai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gyhonggg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxaaqmio.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kckkcrnh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vjtmbmpy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fhrrigrh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3johsxlad.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nqewzbwu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ajrfwoud.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzbohtwk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lsyeecru.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3haiiomdg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3edtzfkdt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wshulvon.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3csnxlplq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xhephcmf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3czafuibd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3foesevbt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpgsdock.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3emuvwdjn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bqutffxg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3geevbclh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lomnvrkg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ypgjmbob.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vibbcsxw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3okudnhop.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3efezuoii.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kbjhymio.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oipsxvhl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fdnibszr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3anhlusrm.html


<!-- 参考信息 -->