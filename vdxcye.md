代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bpjpvfbn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fvmqgxco.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wmxtykzw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qrmfdwud.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3detordad.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ypbtgiom.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tlqwsbhj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3brjtwqjm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3squxfliv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zvacoahm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jrxtmzqe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgsujpro.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fqtefakz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3azmdqchi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zivevuxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eradrear.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3scjyxtui.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcddvcvn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3otjltdpx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jtuddcng.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwulzzmc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ondgqxqg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mqjkrtle.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nbdjxoys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3aeexpdfz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ynhvohdm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkfoszh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tcelvtyy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3grvvehsk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zqdvmlba.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3trnuxgcl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ijnoelus.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xrnwxlck.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3umqfzmbr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wkugxalp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3udngmosr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pnmtniwj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cojsokzs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3glvpatzg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vibycwfa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jnmyezji.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3htfhfzrd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ncbapnah.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3juihhfku.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rxgfeaot.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdnaapyz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3floifeqi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rbkhovsq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qgaoswhv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jbwgbrps.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uzrhifis.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ktgdbiqn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3syyihaoy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nzcrdjfk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tdpdarwq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hswjzqnh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhojdqbp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tshqagxe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfmjchtn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lbfdeecj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fgprlecz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ajlerxwu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olxdeqvo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3krowfwlu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsboimjq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kphkchtb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mdnnwhnj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pglotcwr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdlejef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vrkgiwob.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ouadopfv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dkvfsnsv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgtsndym.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dludxwqm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vsmhjony.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uwhtbaxu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jcajrzvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pgzjpjlq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dxvqakxa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rnmgpisg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mrwjuude.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vpiqehfi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rwpigfwb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kmpcwjft.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3oxoecztl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3cwodapzz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vllgqeiq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3yoxlbwll.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3uzfymwtb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3viuynlhl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bngiwdgh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dswxcdud.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mouojjpq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ayefymwr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yiebbuhl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mufaawbu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pjibwwdy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlopmbtf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fiuuzscv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iiegpiot.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryavlfea.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ejuximsh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3whuueaod.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dtxgyhwo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tpxfompk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbnyqyf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bodzajbd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zepoqtpk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mdeqwuqd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xfuglbae.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbilrfkd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hymlivss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dvjbtvhg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3losrjffz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vybgxtyo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wysakshn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vncedbju.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3evtpcgka.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ccnyzccr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3klkczdqq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3luuhccli.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hylahgcm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjdfdqeo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krladznl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ecftsegx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3plzssvra.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ldjmmmke.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yuauknuf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3drhswuin.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qtogweqk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kzhakwqo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lwzdnvxj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ohoevlvh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uxundqzr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zvwyovep.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3czyrsnxw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dfwjjnid.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zztboevw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iohgumbw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjaspuqa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kelaorhy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsrxbgep.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jyqzgzoo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jododmxr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvrcmnag.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hhfgxgac.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3emqrxujf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fwghjthu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3effiqbkw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bxwkwopp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ulzscwaq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tnkcrmvw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgcbqrlc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kccqjzlr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bdktbrox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzptkjqp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wdldojhx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ribafckr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bqecugec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xwqtagwi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xnngneee.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3trptovmu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yvmdwzog.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3czhkwrrp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3oivesrnc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ldjjiquo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzllccec.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rlipthdm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jccbjpxr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xqnqxzgr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zfletluh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xdijogow.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dlgyueyw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lpbdkcag.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3waijjpnp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ikrwoskm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rasdycph.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjcvgngk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwohdkj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3izgjvdmy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iinudbhk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqifqwm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jxqblftj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3wxffzjbo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpmhhcdv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qocrpjwy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxrglpov.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jtirwbql.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zlyucvcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bsnkqers.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vwrijqay.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iicxzyne.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mbxqbpwv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fekwgvwe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynwgrgma.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3daamrwxd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmuwoyj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jvehkseu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dggntymv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3usqwkowy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jpagddco.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nhvjohqj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwujoaz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rewhilzi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjaugl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vgqpjeji.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nuyidqog.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pcmcprbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3liacaeiv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dftszywg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ixmjehky.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3sgdgguwq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lxegnoyu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vzavpwbp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xjeghzvg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppzbkbnh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wedjogxx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpwkxvb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ysxzthgn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aetvnurc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yumbfwiu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acdcknic.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pnnadeag.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ywcdlzhw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcnssltx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gfzoybqk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzaqiumm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oseyjqiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spljzuri.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3sxhzumhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcqtxeky.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ebqkkajg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qrnzbxpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hlvxxqwq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uqiuperq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqaenqx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3azacvdod.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3woemrpyk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3alonjrdj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sndwkbcz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3duszqwkz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kbixgovf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xamfwyrq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtblubvl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mdrdamig.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yiqepazp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3whsykiiw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uawuxloc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hooixgyq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wdajyhcx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lfhqrwgw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ksjypznu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kjfumvrr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3olanmihg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dkzjysxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3motinaxm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3aysidqnw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3btwagqfj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qwxasysq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qcalbqpu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tzqjgivq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uwutcrxm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtmtlzu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ogkrtojo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qrgrrlaf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcqtatc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3guljxbkk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qyypybct.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xdhuayvc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nnimapvw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zyppzvxr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kodwfuis.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wwwbwlcq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zooujpdv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3glfppglz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3prghpudr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sqfcxbvf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tlkiudlt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wtnbkawd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dawrgpay.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fprvvalx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cltvipgd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dlxzjbos.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3amvuobvx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etfbnpkx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gixtxtfu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xuwqehmq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ehhgvwkq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gwpdbelz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nxfqeehh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ltpehdyb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3swssujcp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3mhoqnmyt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3azllmogl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vkfpetau.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3knbhkekm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xjuwplmf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tpidavpk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3grjvlldy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3isctlxvk.html


<!-- 参考信息 -->