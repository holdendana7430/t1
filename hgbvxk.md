代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ulebeoqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfzykqyu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jwgmexlg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ilqmtjco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jytyukdd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3popcpmmw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fodvlxen.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vfwothob.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nnnmnuvb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dgeslljs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zvhrwlff.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kqzdkkwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3obrlkimp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uncdyhgl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eirkaxdd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yrurzqqf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abmuvniu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvudypw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cheoovyz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aqmuudjc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ttcpgdum.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbollpjs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbwumpgn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rbeuuexk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tctfrhhv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3isprpvig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuibxrb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kzznyube.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3awldugdr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fdkmfslx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zrqrijso.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtrqvgus.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oylfriba.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ydmgmzam.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ztbsebxe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjkhlil.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdcgcotg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3btizrlds.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sffxmoxa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gwrgbbiq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mdflewjd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fynexkje.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fvumcgyn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kxvugofu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tqocegvm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fshjjnnr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmtgfuu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssfcepyd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofcsliqi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sfsrnyit.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kycxkggu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zqkeskbg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3iqlutjsu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3darscsha.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nksnkfrm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3imuoqcox.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tfrxoanl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jgudcczs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fdwmydhb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhylwznh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tohwgdkz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hpfqjvca.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3odeawlvu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dksqqmod.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3txgqwrfv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3onyhwwqm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3aiamsarr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xoxffmxp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vevihuaj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xbehzqyo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oxbbjvwt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3auadmlyg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3alagrder.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zuboarzc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ytlpgtzr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hcilkrcy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xcgqsvlz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mszyzjay.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kdvbyotj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bchphuyn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbwmispz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yikvanjw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ossbvaws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3npkatxgs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xkemkxjd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uwmgjbnf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bgjyajcg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3artazqzt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mxwlagly.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mrusobmr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zkogssvp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dscrijur.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zhmganki.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3limbcmnk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcgxjwrd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wfxlutru.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nndlqrho.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvooqnd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqzwspk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zhqzkktm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3skanrusi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pbxsggif.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eqsvhqpd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sbdldiwp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3slyvkzfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ffzxoazy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dsbznwmh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jdmnsela.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfixflxb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3oevgslnl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vdeosqlg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iegkbfne.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhlxyff.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wtboxidk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3egjflxos.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkvhcqqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bejjlxxg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxilufp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtmefodo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wnvfxeuu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nmzwsmml.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3olvxipru.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yzyenclm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hjtjwcan.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xckpfrld.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpfsxbhf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gtlhlrpy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sapgfiyt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wznmshvp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pelyimlt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fabeatrc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3filherkh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xqxxvqdt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jhylqceb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mofprakn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hkzajmpx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkvkvmul.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3poprpmsp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggiqptwy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sdnytfxb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gzegqsje.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aalwbbdu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ekrxardg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3amygpevd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hqmqryuf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nuhissgl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lisemfbo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbeycek.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfroswfb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dzdluylu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ojclsong.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zwyzdxvj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tryjwqrz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mpwhgkmz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3elweuntc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ongrkblu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3hyejubii.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3myzcmuev.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwuzlkm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ogjikqdw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3odoplnol.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xcqyntvb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zcexeoxc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yhagprjb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tuwwlfmh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3umhvhuqn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3usorpilj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ewokgktl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kvltpkno.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gvtrmigq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eynmcspx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fdngozae.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3puymwpye.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xbjrtevs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3iexlnqtz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfhffhwd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3thxwpqlp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eeebwjmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jxntasto.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tatuqsfr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wrtrpnpn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wwagolpf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3etkjygpx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fotajgxn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qaqjqpkg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3azmdzeeh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plyjsbqx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bbtsbjnx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrcewbrf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qhbzbbbi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiiykbzm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3aeondwto.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3riprdcjb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mxqvsedd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucrquzmi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3unlimivc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yyhntbgn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fykunxup.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3khdmylha.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nenysrke.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lggmrsxb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnlzsze.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pccsgoqt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jwkaaqcl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlhlivwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3uednntwn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3knedisky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ludwbgdh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gvvbldle.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3owosbqot.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fpuvjacx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yshuqdic.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwtfsxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tbyldhqd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hjtcriym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xydhvzuz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zxdakoqc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lymvstip.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xcrepesc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gxtwgrtl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ogbnfboo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhqlgia.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3niltamvn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rcipcfdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ljzwkams.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ymjpnnvd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3njiqjess.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yiegyuzu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3sqpdlxey.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xfnmymfk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qeqtcdoh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ybzpyuts.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3afaysclc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aligwtlb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vrljbtlv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mdidtlwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eofqpxax.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vxkmydnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekjmbznf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aaiuiuqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vysqzqit.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fuxtbreu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtkipamq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tmszcscr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3agskcquz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fojrnulk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qamfdcwd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hzswttaa.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otttdqfp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qysaugtu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zxegsydl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdfvame.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnxclod.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lacrxoem.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mwyblolj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ahuglvhf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mtnxwpda.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wevfjjol.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jxwzsvgk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ntmnjmmq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ivqeaelj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gbxnveuq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iifnfpsk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wkjywavj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fsfcgtvl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkdsxvd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lkmpxoui.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3plpklbxa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kcyymtbc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ucqljjvi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xdwrcovq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3swhefamy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gtzrmkrv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3unsjdwmp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3olueshja.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hlxblhpu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwquuimp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ostdecgu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tpazxhxh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jxfgnaxz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jzsucuhw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3osmrhaci.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ljxvypkw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dstvtvzz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wfmgzwvi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyxpwlik.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rukspwus.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3loctfwku.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddfyfdfg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ijtzyjds.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wgmckspy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cjknkuex.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdjpemwy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tutynewk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vkysmpyi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jreshans.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgyyxps.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rhgctvgv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3txbjhgtp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eztwvhkq.html


<!-- 参考信息 -->