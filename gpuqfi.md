代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xhfdnsda.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xptkdksz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fagyyhwk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hrrqlffp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mhnqyjpg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jbwkfoqg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3auqedeca.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ubeuemcf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3meunjwac.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3agwncygn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mzgfrppq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vchtisog.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nmrxccmw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yarhjxwn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kcismgdh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qbnhvwnj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3thsgghnn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hvsgpyhy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypcxlvxi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dqlsoqhg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3akwlehit.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gfcqxrxq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ifbfysvk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vgqfezid.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iywemxcv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wfarlait.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkjevun.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqsmizjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wckddafn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gouotwse.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgzuxbyr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3okdsfdzy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vyifblys.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3alvzoafw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uhavwmav.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dbwmbcln.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bccropjj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3deqezxnz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pjbpiisp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bjscgllq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdadrdzw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ddknsckw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kxuasffx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dvxmufbq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uimmkjiq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eyblgwlx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvcmemff.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3otssrcqg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jsjfrcqb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hltmjuwb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3caaeqkgo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bobapiog.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3klmkblsw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cnxrdlkx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xhgrlzmc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qedpmseh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ipfbopkc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ptshygwp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ubankjzz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3fzyyxakq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3momhfodz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3semullwg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcklmei.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3homhywev.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lcukptbv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qazatomq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxgkboke.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oaddymlz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hqvogcrf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdwzjhiu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bjxdtzmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zrvbjhxa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sdrtflua.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xowudhcq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jmfifngf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xtdqcbuh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apgfiulu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fayfijfm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pwxqmgac.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xxeycmhk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3skvsgvlb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttgbcwcb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qvspsjdc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oykdykyi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mgrxamje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mddmeyxn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3liblbizh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3krpzlahq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dueqtdpn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3akaauvir.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqhqmru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dzwfedhk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oygvqifm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sibiijmk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzdbist.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lahmaxhu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ionhkctx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lnrwtyuf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rxaumkhv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udhzdhrq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kmffojnw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxffxxgq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3edrrhvuy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kvgtklbb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tpurwdyo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ovkwcksl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lvlpnyye.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hkyyuaej.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fmftkrhy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqvxhshh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ticdudfl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wppxeojc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pxxkmjzn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wuuiovfp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eihvgdad.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lbzdusvh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3klrabxgb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tkasfoka.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3btkalein.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3revdjdzp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pmzjqlmx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qybutgci.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zcvbgdma.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dirimmln.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymakanjd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krprqsnc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qstxflxy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nvnznlkg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3optbcoib.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ynwoutcl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3guuyoafw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3besqdnhq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zirqtlsn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aciliask.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqkmabrm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fbiopssz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtrhiwur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xxgqxjpd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zyoiddju.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hlqfmtsl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aswcynny.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zdkjwhvm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pqvxnmou.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bfopfiba.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wpdzfowh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bdslmtmy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fogmrual.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ibtsbwng.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kyupnhjr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yzdjebxq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kghhnyqz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ecngzfxc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nwrlkzpr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qkoxgrmc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wuljdylw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fiuzwtec.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vzrxkeal.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tawhaowy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kkycoxst.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pfvwgobw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nnxksjkt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xiunsmvg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ssbsuwed.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mojvzxwn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wvobtohb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nqxzybyg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ipujuuvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xrnyaiju.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3otjdzlpt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qzcodyqz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzalneez.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3virlknvu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jdzvycwv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3norfxffb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qsdiesng.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zybjeumv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zcpbtzmk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qobgterh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pfnontts.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ykrfxksv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qqggvjkl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3beizcjyn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cttfiqcy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ecdownuc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nxgqbkvq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vtviumnj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twzyevuj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vnqhfrqd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3aubawska.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nddojstl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fuafnjsq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vihapehx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vfnsvaxo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhrvuto.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wibuhcdr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xztxbbet.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yccrshwj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oyapbiin.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mqmimqns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knkkiowm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3opggmlei.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3snmconev.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rcibepuj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vxhjbqez.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3useqfpbq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3swwighnf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hjwrlhjt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kazszwik.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zlwiozlr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3crzqvqfw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jtkputda.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lyqtmupc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ghdgvulx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3msktyewo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dxjzbwkq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qagicqrq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dxmvowbh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxzzllar.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqautzzl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zyawegzq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3svzguxms.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpfytxg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewiglhvw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yhpteydv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3scndpyty.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eucrlzeo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3alagvzgj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qxstzokx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3otvnrlbn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3abmrgqhe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3owtyprbq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjibysm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxcvhfex.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bahmhjwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzhvwmvw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgsdldsn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3maoybzcr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rufxpnmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqxikjvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ickkpbvb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yblyqquv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtqgaftr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3efjaitax.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3boyzodsj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yvezanip.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vbfojxel.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lcecnvot.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nhvcpwth.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3auzcztov.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yltpazag.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bimhpcfz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3avnbjukw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gehhlzxd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3azbjiibm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pbwxtpps.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wrhxvspu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tsggvwvr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gpppqgcy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbhpwlpp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mlppraeb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tsafndyk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ebvjxwfd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3byznhiqv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uctorhlm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xadtxzeq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vpifxwfd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zuaplqrn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tshbutdr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3oklltnsd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vvwmbbfp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wdjrkfvp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dqjtfjao.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3eedeaknr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ixrdgtdb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3psffdqlx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sdxllync.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qogbhkki.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gacrnlks.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3edjrhwag.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lpxrfknb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mkozagli.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsbhqar.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsybxcit.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fljanwrv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjxsmqtv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hpxwzhjy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdamwxt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dwvyldoo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qbvcsxqs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3grlnbirc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eqrynaex.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pysevslf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjnxvuy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3smgkjnop.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oyhkcfpk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hmwqawkm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rzgzkjcs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nxsuxuic.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nkyhyjpw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3clrkvoxq.html


<!-- 参考信息 -->