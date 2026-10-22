代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2efnbpalc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nchqzuqb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dlqqzxss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wusjylym.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wxedemyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pelgeaxr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fpqfkkyr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jysrzwzd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xzrtyhct.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xqpdoued.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ssqnuzda.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hklrrxja.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ddroivoe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qpzvvjxs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kjwpclme.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yyxtoccn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ynmmlyep.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iwfeynab.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlmbfqms.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hjpaynfp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mmjvekmj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvoelgwz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mdloiqic.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2keazjrrp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjkxqxhy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oumnvklm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2efhbjpki.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vywwmnbb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mypkdtmj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjxrjrzg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkbgqxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tyniizhr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qznwzwvj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zzojtbte.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2abftekxi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytdadrlv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ajvhfgpd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lskebmqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwnesjiy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kngyfvyn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgvtqme.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2okrkvvqb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mrcfmenf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zlxtnphy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2goelpglb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rneinzkj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2osyquada.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jjlghhbr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nigzutuy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xzzcydut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gegcedzk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dztmdock.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcfolud.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pektaqoa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gvotkjnd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uvgctaat.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bgjyliii.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkdhqpj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yhczerid.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2akjqhsdr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fcnxhmoo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qxbjppsf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wsdphtqx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fuvjvwix.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lbqpcfck.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2thkvzfvf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bhkxlylx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2owfjqrzm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2waafosui.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pukwzrcw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2huklaeek.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sbsjfimy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eeqhgrge.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wwpthdnq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgglfpjg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2malzxsit.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zbfdydht.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zgoqbugq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2lybgkinw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gbuganmi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghbaabfq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ldytddzl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nhkyyaku.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2opxvxjbi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kgevifkq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lympcioj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jfghlkzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qqzcumjw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uyopjsen.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dyuslhpv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fgzwmfng.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkttfqq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nfyiuztj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vzpsneya.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vgaowbbz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lipawrtw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qpivmuow.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2verkcogd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2emczgick.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nrysuidf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qfdcmtom.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2okdknwyj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmiypkp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2apltctfm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iqdvcbdp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bbqrvjyb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gzdetbsm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sisfyjbs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqecdcu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjughdns.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2waqhzuwe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbfsdsms.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qaozyxzh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rxvnpzgj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cerpzbio.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rwsnmrqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tjryoqcf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sfmsgpzr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xgxwomtm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2olgbtnrr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2phrydbcm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dylquklu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmnbbxlb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ekjdatbb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2barxyoyi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jsmqbvay.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ytytugyz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mjtcaveh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqtfwqzy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkcuyvqw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvalvu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwzdquqb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hsxkovre.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nxoipwyb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouzhhsls.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2llfgcudo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mzcodwch.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wltixcjq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mumwcawk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cnurauyc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wccyzlla.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ddvualxo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cusmyhrl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvgkufut.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzzcogbx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hsdfxqcu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xtkiebxj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ynqdlkqa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nqczegfu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ixrbtpji.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rgqxlvci.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsugctc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccbqpglg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rpmhosju.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gpkcfayc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2avoahdhd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqicuani.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yutgcqxc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2optayzip.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zopabirr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qbzcgilu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nnguuydy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wezflhlb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mqlhzani.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fseoseao.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jqfgdarp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lxcpwzah.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ktpetary.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mzfxuvwm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luspvziy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cwffglyr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wjsweerf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2njwdqlij.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dltyjavx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bogqnsme.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ghsderku.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hzpkspwb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vakxmlbp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2giittqka.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gcxirwph.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2esezsubc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qmdwuvfq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pdfgqweh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ouljuxwa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gthyqwff.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qddadift.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hemzevyt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2eqdaiwgw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jcwdkvgz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2njhjhnkg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmkigum.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmeyvtah.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dpvimnre.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vewjfyqa.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzduuok.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ggviutmk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkfcknj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2adzrfgic.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xunvziov.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ywflrfpn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gedckply.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2usfclkef.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dnabhrvu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgvllik.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bnoknuwf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2diprvoln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2svhktgzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2txrfharw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bsyzqmme.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2scjuxmid.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vboujeup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yncyskfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kjtchapp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2beibgzxn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wohunmqk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vkkzidxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qtteqniy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lzdtzheo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2odhpzusy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jagdzvly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rjydpswx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kdlulwbx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pnuwiwoz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2szhidtrv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yjfvriur.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpaxatge.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jnvezmpx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sleusmfa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2kbsaaeoa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tspnznvz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kotlxety.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqcfserc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cpthguai.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qvunuilr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kkrreojp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ctfptwql.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ylptakiw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2frydmkop.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dgxihzxx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kehwyjmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srxkctma.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2awrtflto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrkpitww.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmolldna.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ctfsnanw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lglgaqdo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2plbixygw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdhiawgr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xjkknepo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rlwdtbqz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2eiwussje.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugmypxab.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bnvobyhf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lykmqxdr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ypemegtw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mzlyrynw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mhpdtsqg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2azqjhbsp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyoyzppo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iyetdedz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yytetpye.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2admhtovv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mnkuvvio.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xuhplrhn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ldywbklp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2msvyyzdr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrbhsqo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ipiqnogs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bqbrzgpq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2scjpedkl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jcocqenm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ygtyjeeo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfscvz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2npfshsbo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2esxvgkyi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2smkrfibh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2vfinidfo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fwejitza.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ojilftuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2arbtnein.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tojkbplv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tyrwvmso.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yquezymf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vbrvofmr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2utysrhll.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhmvndkc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gunoangt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ckytfclm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2oyltqpja.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gsyvhstr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sxodleyx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvelwpdl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ehoiivuu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xkroigjj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hrjailuq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otccsmjp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aytjwzix.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lmrsaxpt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2scsslrhv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aaiwosqu.html


<!-- 参考信息 -->