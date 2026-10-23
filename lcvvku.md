代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gomieuoc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3plylvslf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ycchyauj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvgotuv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzyzaoym.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wyrwtfny.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sskitesj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrnmbbwe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3arzplaib.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rnvlpajh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ikfyhbeo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ebqxtkjg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cpbyaosx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjcttmqi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3oqndfuqb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iraoxrdq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sudhywuk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xdemiwuc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kweiuhsm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrnpbuj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3skxiupob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nxvpcbxq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zfdcnocx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sinwheva.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpiiaizy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fztzfbtj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ycyjpigp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayqywfow.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3atrcrqrc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3biacemgx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3abdasihn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nzecthbn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3txvlbcpy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3blmfsrpe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lgzpwrho.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hjkkenqg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3byainict.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kcenfhqr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qqsdjjnr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bzijgfgx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kvagszhy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3idhepcbn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nzygmsln.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hdqajkcb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ivfatzyy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nookltfa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3diqprykc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3apyqfqam.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpdysme.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3toulsjlw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ayfxdphr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xkxjaugn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3duehyxqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yuhgenti.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lpcibnok.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tjkyxjcl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gyngefmv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3einhzzhm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jwewcaws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bvjfuefz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjuevkv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aiariylh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iriudchn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gzegpfao.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3babcvqmb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3namijecf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dovzokln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mpbyevjv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3apbzbexp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3apuzegny.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lgrfdgat.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sadaxwcp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qioexkbv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjtoqttg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eckalafl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3riesnjgf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3amlrfljr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3otaiiwjm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iccnrzhg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwyvqtwz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3quqfetuh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3znuztmtc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kxjgejob.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vxdfozuj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mriqngai.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dqdkcxim.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pydjazes.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jebjgksu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3axwqbbop.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qluoxspw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3njxlvohv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hridfvon.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zeehktha.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmrrstz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fhiiobca.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vlazhtyy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3iwqrqypg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tiejmfbp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dfcodmor.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dhnsisme.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkqregfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lpxtokfx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3usishxgg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rjqrlqti.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3czsnecsv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fkbbyxxt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrhqzbnv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qiyznbgc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mjabmxpj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qrcqpojz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3exjgvpna.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3acetvuke.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cvuqriyv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yfyioqwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3issvaksh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nrjwwnwl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nixebzdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bewamftm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gptavdfv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3amzpjnvq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hhlpcorc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rzbyenbg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dpancvbb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3afgrkugm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hrapljjv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mplmoaok.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bendzplw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lbonhnmw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qepdtujx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dhdegmmq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fderigsp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nffaxxoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3egefrahw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ylhajokp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3utcpugnp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jgsqqpae.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vutlupwx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fylufdkv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ghttgfpz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmmngppb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ndhlobad.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehryladm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fxudfyou.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ggopfoej.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3unjcbpks.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3koaobnqn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pglwcvhw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tdpjbcrw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sqvsepwv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ypprbwhi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3scacbxxy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgowtajw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmybqvmo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwqqfj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eilzqxsz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mmifvokw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fwywpnpq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fpmmxcgk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3czaazqoq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yauflkxc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oqnldlmu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jlrotxsz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkacyfrk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ywuffyqk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbuvpyap.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwigrmsl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ielzevvs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzuqzr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3odjgskkm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vegdiakh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcincyzk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3nnzxmkjx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nfvtzlfb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qdzjylkc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jdjbxtvt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3upswwtfb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pkzgybki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3abdiczji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tupucmze.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwmuysyu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trcdvtpp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgmsyps.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdhftm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xwasbrqd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3urolwrfj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gqbhphzr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jthmmoor.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzbwleph.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aknvmdxw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ceopqftz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fpujzukj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pyizvrwh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkejeiqo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fbpctphm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qnzzcfnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3oqqoacoh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kfzzvmwd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvkepcu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bxleohxp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oskqudvb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3odseyhcm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zxwwscoa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvczvagm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbvqbkcb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mypqqomy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rbekhbwc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cteslfsu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tgnewrhd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jcueefch.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cjucuyny.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xubdoeyq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhuefnsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bputipmu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zthjnami.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmxgpmhx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kkxualvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pofoalgc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnvjiqvz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ttpcvdxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3alxzzygb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdnapczp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mcaeoxpq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qslywvkc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qzbnoxkk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mscetwvt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vwccdlsj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpllcbbi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ncsglcuv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3llghdsos.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3egsgmjli.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3afbcjfzg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3saldxwus.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xllipbgc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vvuxzwyv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pbtagyqq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fndmfgve.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nxaozvae.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wmepvngt.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uginlluv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xnqpfusi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hsdairyo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uopsbgbs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ibouticg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crrsxosm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gwtfcqdb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3smrjegtu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vcipabxp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxqeicg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kalovbij.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vlgqkqgt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3frsrnbwk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pwlrrpxv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3okdceioj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qhtrivpo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xftcafwu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3evbsdfnh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3orpoerln.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fdbdxrtf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rvhdvkvt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dqocsfdb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ootoibpb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3umjjqfps.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3btqanvaf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uctffjeu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nrwxlzkn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3apfjekst.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxuvfhdc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cdjmjzmt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgspolia.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3avyyejcc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ncckbwib.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdzlksce.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mkywnovt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3knuvyrec.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lcamgqfq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3agdrqsas.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3iyvzqgat.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgewlmu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3halqsweo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sydzkslz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rcoftgmy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3snxtfdiz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtgcyjv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cvlghsyf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yyhtvkto.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zkbpnehy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yvvkgvok.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wjymwqqn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rfznqeoh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxnrngou.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xtsjzkgw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3weikaxaw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzuxzdhx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qbuvrtag.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tsfjzcfz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3upnaqfpe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3epcmmkvr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pvvztmhm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gwfvtwjs.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uduiogyb.html


<!-- 参考信息 -->