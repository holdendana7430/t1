代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3swbrihkl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tvepmiaq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gxsuxsvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uorcnlpi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3iomocvil.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wkgqnzlj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uootckpz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3huabuwpd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3imqfzbia.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvkdtnr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3anfiqsta.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tyimzoee.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3flsqxkpc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ipuadxiw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3twimikcv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fpvxpbts.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqjspyhi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rznvagkd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mdlfghzd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ldbgrclr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3evihwzag.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ehgekhbv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3niphvgad.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjwtwlq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3amppwimj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jicwupoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3olsnfkkx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mywsmdql.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3biqpwpfa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jfgzrjci.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ckyzqpxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bgijkunz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rasommfe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qlabbsxs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oefrhnvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xtavxeua.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvmydpdr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lfnefwox.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xsxuucbz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vtbvypca.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ufqttica.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xvcgmuvm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dxacvgon.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gcuhzspt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ltlzxjfs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3klkapdov.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bxilctnu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ukovzcgu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3erqhdiqz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3konegtxq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fqbkwwjp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cmpbgtfg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3huhgbimj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dqdcqfhp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qvisdutj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3htpbmwqc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aodnjyof.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vfezcfih.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qpdbiguu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lsrxkrxx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zkptczve.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3btackkzv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vjuruzem.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3majmaxoc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vdqwstcf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3heipgpxo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gpczreyc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rrwsksxz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oafqgeau.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qctfvsqv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3otpnvabo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkggij.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3prqdhqen.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wkojhitr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cypvrpzv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3snuimtxu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uuextxxr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fmwkodyw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gxgyrlil.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cwnveixe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3azykdgqw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wipidhpl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3npsgrxpw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3edrzpxvn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mdkdrrkq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3recsploy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hbrkxvnm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mjngqtcl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gmewuarx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ddfndvek.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyhgabcu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sohewqrc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vryfomiv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dgponzeb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3eumiucer.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bjvawoea.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pbxiusmq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uoldqsxh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dimkhftz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3quqdgqfs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzuryfjg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ieagzlqu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gdwanbwy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxmalbm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xejntoil.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bbkjkfzv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aiukppuw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kngrozjn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzyxvwwi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwurxsap.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uejgncws.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3znnufpdb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wrgeaymq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rqndksyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3voqmcios.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cvxouhds.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zlqqyzct.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wwyjvmze.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjaewcgd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tfpuytlw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3plmqmmve.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3amiwruxi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gcvjmzgh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvysqqtn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3juxjjcgz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3djvxyyvq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nhinkowk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ardyriku.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vqekkosv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ddwtridw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3dumroxhf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nkipwtie.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dgicahtn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3utdtklkw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsqezwvh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3syqpqfuz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmwcjrzh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oxudtcbr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bykjkmgz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3enkewsxj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lepahdso.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3oomiogft.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lyynrkqk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvffqtxp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vsrxmxti.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipdbmhhx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3amnkmldk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3uoltpoze.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqgivlre.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cshjnrzj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ababkpqh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jgamxskm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3crrkukmk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wxerduci.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrosmu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tjbbjsls.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sbblgzgj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vbjaahoc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gusczhld.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbzbtps.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vkmzclpz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3oztizmmd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ruoeaido.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jknnnibp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3elflcuof.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zeikkdye.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nvqjsdsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgrhbbw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lewuogur.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mdpynkef.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sufgwdhv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3noswqjyn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kvktjcoy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sioevmga.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wdbuvlsk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gsbuoklu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yqilxpvg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vaiuhwci.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bnakekee.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3avbzjkbp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cugowhyi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tetfwhkc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cqnxswcq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3godvixiu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3epfhasvz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzxcocfb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzrkvojo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jubyblsg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bbfjjkvt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mnpnayrn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdrwngpb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mwuvvvbp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kbnccjdq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfbgiko.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sixwtzvh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3busnqcar.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nzvifrys.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eowkktyz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqwfelm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uamtjshp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3swbsmnph.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dfsipmlj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3buonixky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nldgolos.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnkxcrd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hemyvulq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yqdfbfzd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfytjiio.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuknrshq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rlxeafrs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yfongufp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mhfjyyvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kzmmfggt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zvvtkehe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kenpfkel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zhpvoshx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yhyggiiu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tchqbesb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkpoixrv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3klxuekii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fytzhrtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxxoqym.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kqemfouq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3cgyxzwho.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jlukublu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3visubrpg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pwdcgjuu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tbnkinou.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3btijsyci.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3whdlkaxf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kzedmoai.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3afsvilji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udcjgfpy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xephzbmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdfbgtuq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gppzrdwl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3crctupxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acjqwona.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jxjfsgpr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3topdusbm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tutmnfcj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3eycmsvcy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hwlnpclk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tprmnurx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vfyiwonb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3twxgcsao.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwdzydji.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwmxdyi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fpjimunf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odzzdfpl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sbshibkx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3folxcboc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zqhjnkqw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cvmnmfpv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lgbzwqqa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fjirqjfy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yaajahox.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmdrfwa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wnthzkku.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ebrosqph.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3bambixtl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fcfstinq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iqdupiws.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3evzcexmv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pasyfbjf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bvmzyopi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3stzedcob.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqlstm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fguuihyd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ldakxxqi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rtwoyblz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3umrxyura.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3izbxykmx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tyfsmcws.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rxrggcma.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kpogblte.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nmotchse.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jvebapzf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3emejuwir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tzpoktvd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jmrjtpya.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmigtzpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhszvkdy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yrxnmrnn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgxzbhkp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3obkottgm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nvociofb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3brwmtvxc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vmsuqzjz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nzlqihlz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qdqtkcsq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnpbwqm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kknpzbeg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwxomm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3miiacyfw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqruizb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kanqmzqi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xieuuecz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pdjxrska.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pevhdbyt.html


<!-- 参考信息 -->