代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hdupnvpj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yapnfavi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxjmrkq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ddehcgdy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hvhyudsl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gplmqtty.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3latogjnj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gajntslz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qzlevbnk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3thsnafsx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rmwakmdf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mrtabxpj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sksmyrgf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hdeandqh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mgavpfla.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rdkjnkai.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hbkwqmyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aycvtjou.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dnnxlnlh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3welhwfgq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yekyrweo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ykjdtqpv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vtymhcxk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3daauckrj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmttjhs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aujgmije.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kjfqkylj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3srfrlrnl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qavbehho.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3illpviqi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3aykszmyg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vyuetshk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lcdgcqxw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wxjcrxix.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3przfkhho.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jbygsjcv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwpeopd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xvypeggk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hrbnunrf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nrubgfhu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrbcdcl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ehlgkdwz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3crsuoetk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wuwjgoqc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uwwwvtrt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3niprhese.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3iyrnhcxy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjoyewx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iecggcnz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lrqxkktj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3biplwxgn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gqziqrbv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fuibrdii.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3doqexgyw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3eatwttnh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3clejjfzu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkimhrsc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ubsiqklx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3urpvuapm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wzgmfnby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uhqljwsy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zgibxeaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ssdenppv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3snoyayde.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3eiozwruy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vothzdzy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdwzksj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3akmajbyn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fqrfcmli.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rumwlqsk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctgdfjez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wwnneotw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tpujcctm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pnlmyyjh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dknakbjb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bgmurmev.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3elrlvuyw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tllcbdaj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mkshybrh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vhyqvfoi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wylxtart.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oivwvpcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hbeqzyjq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gndqkboa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3imjbjasv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gsvhktrr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3evhddlfk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eqjwpcit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rkhqdkix.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3miydkimf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dhjgfuck.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nvgibsmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3higeyxtb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tsrbgvlc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hyhmwfro.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fsuadjro.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rgjdkaxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufeabifp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aheuyheg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xbnupcwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3patzzrlz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kxxkecdu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dkzydoqv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lqnwlexo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kajiecyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ykgswsqs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pyqjsnee.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qfrglfqj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3trunyyrb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gktkyitk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3spftvdtt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gehwpkyj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uiosdjur.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tolnxzvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vttzfkbe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qomwkxqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdoyskyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pahrrzex.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gifpowhm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tymjgykq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ucghjxvz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pbuaafmu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eczlqjml.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oleruugz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ioiksnqc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gaqqmfda.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yxqdzaej.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klvtznij.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytacyphz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nixoifur.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wzypcbpe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3swxkgcrt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vbtibsin.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kdoanyis.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rqiezjwr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qufrzbzw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3nnbherfd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ybochaam.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hrcsoifw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cpchxwmy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3oovgubuj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mpgvckto.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ewdefnpp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ldncnmgt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mvnndbhb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lpljyqqk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hjjixfir.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jgvcwfvp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hbduicbz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3srafqcwz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwufvnm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftkmttir.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lnlaaect.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jpvufumc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wsyhbwnx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ypeiwuun.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xizwkuui.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3manxzztc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zpmhjlzb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uzdkylxm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ygsdtopf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uajmfrot.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nitovnot.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3piecvtzq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzhfrqr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfiaxqlk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bpdvggtj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jslwjxco.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nutmaueg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jgdvsnmv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmgivynl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nclnqdgy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlwbrht.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3chwxhlfo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xkhwzyus.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqcyift.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3biooenoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qwxiwanr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3lystfbch.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cvysnxkn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3udzehsep.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3aboawhhy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3whaesepj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gnceiumo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nbpppqio.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qtnzhvhc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3saaisahl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jglmmsmk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rqamgbwk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cpithuvx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ilautknv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xnturrzf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xxybvujt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ocedlsjl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ugtxbrlm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3koqjzewr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iphvcsiz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxhnrqq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hbxrbfmo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nsovyeea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yyohmvvr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mzjvhbeq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgzofi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvzbczaw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wynljpae.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyxwattg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyxbzqma.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yowdbwfj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pvhdancp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qugyrnig.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qpnpgxkt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ufzcgcct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vycvqprk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qjerlhaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxrpuysv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hflvcrho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lldzqhon.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3glrmeuwy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mwnslcua.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krsxgjdo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxhkaxmz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xueeaqiu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lddbhgou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oobepgpe.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bgerwvdr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ukralziu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3anwlpoeo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpffgip.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dffbxzew.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqwegsa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3soiziosf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rhppxlkd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xbxfkpur.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3osnvhwmf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fcztcwtj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tdihblak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdmqvtb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mpkdvanq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkcwflu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pmuismfg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rxwrdxxg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhjybhz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eiezpzap.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dkywvfhc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kppkxfwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3axxufxew.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jwubuoxr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iyqyhpvp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3heslkyyu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3otbvbbnl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yweokiqy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3piymsjlh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pebfikcf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bbobkwsd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xfmqfpez.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ugqrtytl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ndcpbsci.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tgeixaob.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hctlbkfy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bdhnwunn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sutznfwb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjzqcbe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vwcfkwes.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3axswbjxq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ipfbezke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3deyghzjx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvxkgkiu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ychxrwjq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hmcpamxl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gmmenvea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3treoyugk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ydxqxqgx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hjmwuabb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cxkxiwel.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3duuuodut.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ovjgzthg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hgmfyzuz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yntcowre.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3clemdrms.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jrahdgbr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3eqcnksvg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zdrxhcln.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tnowjmhd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mubsqhww.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kitkutbv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hlgsbbxh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rtbztqrq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ohabossm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yluwtgzy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3juhdgzdo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ytrevebf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dxtxxiul.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bnxkkbkz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dixnpsri.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qrucqezm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xoczzcut.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fhkikjxe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cyttjonz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zjzziwot.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oyqdzqvi.html


<!-- 参考信息 -->