代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dmsmsdit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3augkxjit.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fhqcojkk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pyzeufid.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xxatzyzz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqjhutvs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ftsgpids.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iscilkzs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3axwqhusy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3usnhttgb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3anhxpdya.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ajgzxlne.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xlpuogvd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bnwiomvm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xycyfttj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lowombuy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dfapviql.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ueccmhiz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3istygzjo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jsxctulj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3intuesoa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zspmkfbr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bhliwyqz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qvmwgrvu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3toiqvssp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ubffbthc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxzgkts.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ejmijmdm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zbzkmvpf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bgyvqzoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbacgzx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cwqbbomw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3uvfcwkwp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlnodwtw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhwxgarh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3skdozfmz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnvbuqa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovygxoof.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kmwzjgna.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3onmhdncu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3znzscpbt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3itfvsxvr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3liusutbo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xsenegjw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wizostas.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rmfdmbhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wzjdvsyy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gxqvfkpe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpglcta.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ilszrmco.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljeztrjn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3enpkeopy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tufaabzl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vlptoohl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zfqhiulp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uqynqtfp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hmbvbhnu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xiowpytb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dghwgdlx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cnlaiihw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3resrjhyb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3abgjcgvp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yjqozpmh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ygndcgvq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3siahlykg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qonyxqwq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3imibadsj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rqvhbizp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vkwhexvg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sdjavwzf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jwbgnbxm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3uakwklzq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbvpcfy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vjurphbq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bmqlpigo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avwzkkxo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brnqshtl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zpswbpma.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3agsqchon.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aircmbpp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nojgrwha.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nzstmctf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wcmqoern.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uacvoyvh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxjsrab.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3muploacc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fpshijsl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fhrgkpmz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wneddtoj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pxpqctqk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtatqdc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3usokhrmh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3thzyjqru.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3abtomzrt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amekwoqw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qjvaaacq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dfbcdlme.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3esdcwjlz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lklufjfo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vasukkau.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tcissepl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rxttoqps.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbqtrs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lcmupzkd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnreyot.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3akfornzt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kwqecrwc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnoitzmg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plwyxyjj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3twsayzli.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3evxmilku.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hsznchct.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mywhjdlu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mjcpmksf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hltjbkpj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jdflubuz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nmtxpuxc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uxvhluex.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xsevmtbw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ofshbvqm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dnhrokev.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ucqtloas.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhidbrj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ptdcbihq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fqypnpuf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvegjbod.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czswduld.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bfgnjavc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wuwzpavz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cfezdaua.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wttcwggh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cazgxocm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yeldznrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rghuwigo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3sbxdndnj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wrrksleg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3iinlgnxj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kayrimvc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hogencka.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ubwwqncz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lunzbams.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbadqbqw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dgaiglmd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ntcqzqup.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wtwmxnuw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmttik.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ulmhusgk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqtyfzfp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tidtlisa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3myvusvur.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knikjlir.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xbgdflji.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3npirxmzr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bwlgotyp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3imsridtb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hbcbpgxy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kevkswls.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ogjbvuhl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3txnufmqj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hupweyef.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjpwmoso.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mroowvno.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3drgxbrpf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hammkxls.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3siphrjih.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbktit.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3iuhsjyak.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dsdpyozv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ykpiffdz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mtmbihiz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3glqvdolh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3coynmgaj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lytzovhy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3quvmscwn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tywtjqmn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwzppcuy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gmcgaxks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tqlpqxca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jppqwvdu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vjdaocio.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xxmzwgjb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3exeovkwq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nnkrsdkt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rfivbvot.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3evhhjknf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dimjexwv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3utjuwglv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgcocaik.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhnydkqy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlqoupuh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3phavrbzy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jyrffoev.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vaeqjicb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jlhiighy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arhtpwph.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bmyqoxkg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3puywmybr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hztsabln.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ddivvxtw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oflllgnj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ydijuxzg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bzegwdbu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hyaabohs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfljudeg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cdxqbgnd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3itbmhwce.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aperxnff.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3douvrbde.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3agxpjbhb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ilfttlwp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zpkjixmh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgoacpiu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nfvadylp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3umzvzzbp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vklrgoxt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rmqmwusb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fztmsbqc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ixfynala.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hrwrvhau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3utifapkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fxcpcqsz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgnciwu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xficgowb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3saoufbho.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3roywkkzs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gpnoysrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wzzbplht.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjicxvtp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cugvfzgn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lojfkshl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3esadliqr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gibxnvem.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ukezyhlr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kmibmzop.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dvzkhcwf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3poqgmdxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3letdovkb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vcjfqkdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogksdhop.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3awhffrwv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3eazhsmfo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zcrjmvit.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ipltuwrj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3erlelpga.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iblpzfyw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qptpyweg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3acqdghxg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrmuicxn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvxqud.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kgawxzpg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wwiiknro.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ypecludd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3shhlwhdl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oswvfzke.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sqypsdvf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fzqcklyj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ctakothq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3llpgpnwd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cmcpetuy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hxjpuabp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nzxpcncf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vsnwufjv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wyvzthnn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gvurwoem.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tuluoljw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fptoefnx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ocqnjsgo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ffqfatjh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3leussyqm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gbxdbjte.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gjfrwxnl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qdqdffoj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3lgzkrveo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3deigqual.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rrflfjus.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ysfzresj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xnqzxtkd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rpzvfsrs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3houycvis.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nexuvdlv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3olvcthhe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pxqjmsvp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3swznqjnf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jasckygw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3nrkunduc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnjlxvo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tjaanbmf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nznespeo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rybuotce.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3drtpilzx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3edzoiein.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vvagwipb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fpkemalp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vtwiwxow.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jiqhgdxk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivdomhzh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qknzocnl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhwtptn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3iymfioxg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3toefyvkz.html


<!-- 参考信息 -->