代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhiils.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dqxusmct.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3taumvcct.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xmgtjmsp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qyofsqrf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3imwqqddg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wsnqxbse.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3piembbzd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lymrhlgy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vohyapmw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eczlbpgc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ztinyuct.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cqoyxeum.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uteaaonx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3keftgrhx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bdqyopmv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pcutkrfj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3espfiiea.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3weeoucmk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oczkukhl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uppjebvk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwuooe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3csaekqwm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgyuhrjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ieccvcpd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zekigbwm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ivutazsy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vhjryxea.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkybcusr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3sylcsxyl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ctwpochy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wlbbtyft.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xtadonak.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vpldpqxe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bagiezjk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jugoscnf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ujrabdwg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tgekvmev.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tzjhvwgw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ievqehgk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhtarqtx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qphyskeo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rgruwcxd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jhaqttug.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kkmdvljl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zydzpwfk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iyrgmrnu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrtcsc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wbidcjby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bsoqxiim.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3waslxspz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ujsvjnjm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zhcnexmx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ccagddgv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3garqcgyj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wbbtjmia.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3boioltjx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zsklexge.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rcfhxorh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3boceyxll.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3evykxalw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fvdoplbl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3crikcete.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rcdcanoh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwkiuqnk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cxunjzab.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hrksqsew.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ncpxgdwk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3reokixun.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3isplovjw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3laofceqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xplhdtat.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvhebadq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3benalynv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tpjosges.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xjiibcfv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bblgdaim.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jyvdxxvs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcmgbwg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3winajfiq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3izsteaxw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mztuzpot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3sbjgbpqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3iciovlfl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ufwrzauc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3avmnznbb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqxanwut.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tcaevqcc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3oxesoogk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3icsbcmgp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yckupmkv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3aflawgqh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3twgzmsvo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3plqmzyru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qgqcdoek.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvjilcr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wdjxtxjj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ouvhmtxt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dbmzfbwq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3spjpfzpu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3obnnecqa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lazwbhah.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rlbgdhep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3doxgyrwp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kmrydbmu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wwmmimmh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hvwndcmu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjmfftac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gvvvpurr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ofailucg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhshlbki.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jeglkodq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3whtpskps.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ozsozmbn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuzvnep.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gabzmduo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lcwzhypj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ozrfjjee.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3toqttvuh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhfbmepg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3brlauffu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nfdjyroa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzznozkh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xxhyfkkc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cmlgygro.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dvpmgrra.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tyeokizd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ljgetrrz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwktml.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yplbfddl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3deddkmtn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kanxkpef.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jimgkxpx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3otylstha.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qrjszesj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ahjmaptp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ymfpbbmy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rltwayly.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tzqijhjq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hoqwlnvy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scantpub.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wmjdjujh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yufajcpy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3piifopvw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gbsfesyr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vyoarmhu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mnqbxrsp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kgpxufzo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xbkeiqox.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hpogvgvl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ukaclvfq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jwcdwirk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dpjfubvk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kusabzev.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3orwrwfmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yomlftkj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rurgbphi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ajbatgok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pogbosaw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3elymhdps.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hlzfcqzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3sfpctjyb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eapwrhna.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvthoyvq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cnpnayvy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3keevpqwt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgtpxzz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjswlzak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wgbbnycz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vysqmcvt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xipzkoyy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bcwvzbzl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gdgimwyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ptkbbvmu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jkepasfu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aseryvqh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xhcfrqjb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ielodyrr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3duxpdrol.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tbzlnhpt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lwzusedz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ehlqyrmu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bhrjebom.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cvehogrc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xgpimezg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ngaehbev.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qxgljdss.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ydvzxqyx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dqhycvbw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3trygjvft.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rvjjhkjz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nftklosh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xdiftwrf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fynnmjwf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3iobobrpr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3chwxyeyy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3apomjqrh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bncikmgr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jqldvmaq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jsczgvlu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jjxfovmt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jvrjhami.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ysenpkyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ovdrxenm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndeaxpln.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rirhozom.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ruhrsnou.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bgurrthp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yuuvjxvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3defninjn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bimnpprc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gblrokwj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cniskivi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owxakqdk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rlnkypic.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gybhddvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qnsxxjda.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmssqnlx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bksvsomq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ecojnrmy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wluvcowf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sszomtpz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3alobcokq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qgdkinrj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dnlbbtou.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3enovmbvf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lciqfzco.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhlgovt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glccmngp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eefqjsdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnhbwwcd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ncsdihkn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wwulnhmk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3euvekrpn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fslmeudo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgopusod.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hlynelqn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xpdgkhql.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ltgqsikb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zncckuzr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqrrhkgx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ghxmyhhw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3igprknej.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnkwyio.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3shearwck.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uiesyjjc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lnrhlgci.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dbdcytzg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vfyptrwf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3potrqwzw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tpazxdbd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kscpeeqx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3redszchu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3omugvzvc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wnwpdrcc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ztfenjlz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xgypqiyx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pnsubhfy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ohxivzep.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bskoxjxg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3scsnajjr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ywraelwq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhesajz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pbjvxydk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zcwdatqc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3icubizih.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3picarnuh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bibibcuh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjowlcnk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jdmjzsud.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tihnynzu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ixfxuvra.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gdeskcpv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3byytvpsi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kcdatnrb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nblofwjm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tbautwvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irmbnupg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gbdzuxul.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umhlinmw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gprdftfg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ighesfwg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3glddtkre.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3viovceaw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kvnlqeta.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rjpgzupy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cfqevgbc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwwjvscl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jlrgieoa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ehjopmus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qrpxmnxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pjimpuff.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mrrymvub.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdfjov.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iukopofw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vihodfbm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3njeufsyx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bdvrzdov.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kwkvxdnq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qzuywmxd.html


<!-- 参考信息 -->