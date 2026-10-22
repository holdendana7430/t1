代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bybpyrnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nymbefee.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dzykwqej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lmdjeyme.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cqmoeosp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xeqpijkm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rfqkqiof.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jmdyxeds.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lqgzsvwn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qfvasngk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qkjqxbah.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2egvbgtlg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2owozmgdh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ktkenuoe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zsucisrx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2usxdwyiz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oclwcxci.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqujqrs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vkpjfnuw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qsmajsug.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2freihmrl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fukohcth.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iggkgllq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zsshjqzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2avreupzm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ljbyzabp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zpxkfudg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yambdxkl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pnalmqye.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pibkahlg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhwkzsp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sllucrsp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lugezdgx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lbbhpdhs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwxpwsix.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xshjcyzx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mnunrtvw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2irnanpux.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2plkjcdcy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aiitheej.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wrqzcdmy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wvxatroo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2eaktprgg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cvowsgop.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lfteypqf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wialzzcz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jhvjujdx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2evkkdvqu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcatff.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emvmapzv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2btuiglxo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fcvgjkln.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bfaqwfsm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejyuhldy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vcxoewmy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hrrhlezr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pcuwbagr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yrvndiod.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2niehscmu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzxmfeou.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fvylcyrw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bthopzcm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2plimyxud.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cbcndixc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ampezsoy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kmuyafwo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlfblojd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2isguejyd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2majsyggn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yiushlpk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ccvrkswi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2chwerleo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2msaofduv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2inakleig.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iswhommz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2coxneclx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sddcqncr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lmnokima.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nfkxowfb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jrxdycpq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdzzbrzx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2chnyncrv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2haeswuyy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xchzwgyq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhldxwa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhpyerak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ujagijvg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xgcfixew.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tbkgtarg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2bfidvjca.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhoyczj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2iwxqgopb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nmqmdwpa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jeoougyx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2dcztxaxj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mdtdfxpu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ijbpewkx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gtlbmyzs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfkqtug.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fffirkes.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zftaachw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xzqtgahq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gyejdkcl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rflolxyg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtwontm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2piebjyvx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tghitsnb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zsjidwjj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jttjqsdb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wtwjokis.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ukcejnnh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aocfaskl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pftaepfr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jfwbhfsv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eidqorik.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdwdstmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ujhoziur.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2porcchul.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufuoiabf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xycdccnm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jnmiyuwi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ijyimyao.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wysibkie.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbuxgai.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvtbqhp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2skgbeljx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sgyjydie.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbgtfwmv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pzxxefye.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wxvbqyjs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mbsvmlkl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tckuhmkd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hwdaztfj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2phjmprkp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tyjqnnzr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pfbuhrpu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bgpvdnim.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zuhmyoyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bcaultod.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvisuqho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfrfjtv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qcnqdaji.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2syhzbztg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tnsuqmrj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2yucocqpd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yjfstmms.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kmzhuxrg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zzpyivay.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krfygoke.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ydpeyrur.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cgelxiux.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mxzwjdtg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bavdojsc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nushnifz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jsznmksz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2abtpftuz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2oxyussjc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qkhnjtqa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkoaeam.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ugycpbiz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywrukmjz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2duxlvihe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lvjyxdjt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nakdrjpq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xanahcxn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkdyywqs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hybpxlzx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gntywuei.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtgnkbt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bvgdpjls.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cfpdcjod.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hwmkohkb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2evhykape.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cbyobout.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvvkahr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2simfxnlg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2usnzfhnk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iqigzcac.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zijbrlkn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yqblcibj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2coebzejr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2blhuojzp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pojodyhj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qgytyejk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bxuxsnvn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2avesaryt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hprgoqcw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swsechta.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qggleusf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zktclyik.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjclxckj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wvuulhhj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzquzscp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kflkfbre.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxombbzd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xdynwfcf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2otziqgrb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zbrlrmzf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rseqlefu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cycutuna.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2oeasqase.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xmtqbngh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2larfqjnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gorzxski.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gzqbtjbr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2idfhodmh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvplvfyv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mfrspaka.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kuvsnfbx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lglrncjm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fgwapwhz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2saxajkgh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2crsclqpe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dlsasugo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2miowxcbl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhrsggf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2aoeeuwfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pxzalvan.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rbdqwlou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2grudaimc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2imsqmguv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nwdahjqu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2makrhyex.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdvutmq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2whbpmppn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qtbbslsj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ezvugivi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2stvqmpzh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2djybrogd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wpdoblbn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qnxkjwti.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2klcbpdfu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dndrghns.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2szmpvgtq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2byfyhrzn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcvyehm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuqplkuz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pnmgithg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixzsuzsn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vwhrqztx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yolnacct.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fgfolaqt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ypgmnxdq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awzsvhmg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bcquitji.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tmmflgtx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fkshjkpj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tezthmdx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2npjpsyxk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ipkghdwm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2usetrdnc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfyyccr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cihofihb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2paknhkai.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bkcdcxbx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pdrmhtsu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ajonorka.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xungvgtt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hythotpq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2prygbmxa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kpxzggvd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2thwsvuwk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgojyle.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pkirxpzr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hvoaumti.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxrhypy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kdyiodbn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ydmaiqpl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2sbzjuvzb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mchkubmz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tnsbfhdk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kaumarit.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2uamuauiy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mqjsejqm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lozjxyhq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tsxbbmoc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ekdputha.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xzflslgt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxwaopy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lwdvndac.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zdfpjtbz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2glukmdae.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qdkfuuxe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ledxrqic.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ykflwgtl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2docbwkvb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tccthiwa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tceumykl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxtjrwkq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2umivlqes.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrynhpjo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mxcfybeg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2somqugoc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tpqxjcjb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iyuvgsmf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ecderqnx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qlhdmolt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cguddczz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eltuaohk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2awvbencs.html


<!-- 参考信息 -->