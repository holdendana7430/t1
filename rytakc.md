代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3oforcuej.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdgnonr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjovuk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ffdzlxib.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3solaxrsk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ibyfwpba.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mtltrhxe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vdlkdfwh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nvdvhhsx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ppdnrjva.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hhzsgqve.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exubjgem.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3iytmzcbb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hytwpazj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ibgtmqpc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nlexusli.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yzupukeb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ocbgbovp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3nwbxsxes.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jtaykkbx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3deunxjme.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oegchdpu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tdkxxymx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bymtjmfv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wqxehwnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vffdreqi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zvchebtc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3etyntrra.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdvasclv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rsflpruj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xrjmoosj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggchtetp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hgzqvdye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zthcwgjx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hcxtrcya.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hslixeyv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3unuuxnwq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeizns.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xkeqwdun.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bzcesriv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qegflztd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hxetjmlf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3khceldtr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wmspglbr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kcgwpvtt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ejfocbtd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vefqkbhr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xwfqsmwk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lrahsdtc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ajovbths.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghwjsvdx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hdbhsnse.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3olwetacb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kghegpko.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ijmalvdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3exciecpu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibyackay.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lbxzpsan.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ubzztvyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3avynqnzz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrrdjuhl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eswcejfu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cbzvtjbq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3amgmcumn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xldwgvxm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vvzrfkqs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3khlazovg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwocrmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wggndpwo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ihoqmnfg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fygixjyn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fkboklgq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvjnas.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vjfctnnz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cradtdjr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tbbofmiu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pnaamsrl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3scuubjka.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3phbxkbbl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fhmfvcxg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uboetbta.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3iakdbcnh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mumcxfkv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pgsbojox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxtwykst.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3llqamneb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3snryviqn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjfwehb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uneebbni.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3twyawqss.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ziygngdv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ztxighng.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dqybtijo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zsutauxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gyrhvrbq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lsieypbu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lozjshkp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xiypfhgh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xryztsyz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bpwadcbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dyrtngbl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fanpncjz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrwapkbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ufuncwah.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqkxmhjx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ljbhzkkq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sqjunwhi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvaklptb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uygnlvnb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bhfysxsn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lglmsbds.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rtprfyzh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3prqwgees.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dpluinom.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rreclvmw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gsyeeafv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kmqwcdag.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jbxvpgtf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsbphoi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqbwmzl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxrlmls.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkorzwpw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xyjzqpuu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3trzinrrh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vpdaczyj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xfkdiafx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3buwiucuq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erfledao.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chwbftot.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dgidktqh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fcujuyql.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3frwtbzsp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aqejcnov.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vmsajyji.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ldmupjrl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3byfmchdl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cnqablsa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ljezwbsl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgyarlg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uvdhhmvv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvygwm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vhswkcqz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dxznixff.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hblkciah.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3exwknhmx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pfpdaeot.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3onauieoo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qkvvhjyg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nwagbgdg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pmdnlkds.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rgrupolc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3elvgmjcu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3nwoyzbrc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kepnrakp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jpsitisy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jbzoagsx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tcesrwnm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zwporkgd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qyxvqzog.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lskbzacz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nkhgohsm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zjxcqhyu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hrjvupvj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tohphidm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fjfjuonv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hveawcsg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzpdjhs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ntckyjgd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjihjphe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zweyyief.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fkbdgtmk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ajuzghet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axajanhh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rokdmzhc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpwwxez.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rxkicnij.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3leyuzkdv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzzskje.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fwvmjkma.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3echzoqsz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vuzqffwb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vpsgwjyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3leglhbap.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qhfahbtw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ygwrjccz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqkcwvm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zzxsqbky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wreuttxz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oogeaurr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bnvqjiww.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zsripzna.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nqfjumly.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cnevtulh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zdczggmp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tbkxypxg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zwqhkwga.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rfrxkquv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3evvvkugu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tinflqxb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gwkocwzs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xugkrthy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3mtyjvqkf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zrelwuij.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czqaxlro.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ybevgfub.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyvnsrp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujdkqljd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqfbbxoi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eimxdeit.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtjlqohu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xuepzgqe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xtihrack.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwzmdmn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qqrgqiwm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xyrndiil.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yusizhgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npjodthp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ceoqrjor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anurkotk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lacsvmvy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3irrzfnbv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezigjxdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pscdwvga.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rzjszggw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cunrqghz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3olahcivm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xxyfazuv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oewkdfip.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3giupupnv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pulsfcyg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljfrijkz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qrzsqvye.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3awswvjqu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3litadnfi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjcgmym.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ytkexjdu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ndmglwsv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mjjzplbk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pfzbhyts.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xafasufe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oututkqk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zcqoremd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bhvyhzyn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3haeojzlm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wsnvzlxk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tcxxmkto.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hvdaqmuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3emmphxbd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lemxbqgq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qmstdmyc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nkrvjliy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yktdynfh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvaodh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3srzyrkem.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yrrastji.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3akaxodaz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kthcdigw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3amstxwtp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkkxnel.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3atcbetrv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ygnldbyn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hdcnqpkc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwfzhch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gikoktsu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mhmudtlu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nisypjcw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3newniuri.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rfhgpxbo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3difqsxkv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjyewwjl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gloshukw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cvfywatg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3opnrbtnl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jqqpliug.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eqtzbqyf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dkugketl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zyvoiinw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mddnaxoc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hmgzspun.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3othhbbed.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3efkqpahc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zmysmsxp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uuczuzoy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zslznqbz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lidwnmsc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aevonxld.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3egcgmjcp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bawpxifr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsubuo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3flbetqnk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ahtbszwt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rhwtngyu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nybnduhy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvtedtsf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3joamvdbn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3okmdevip.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tlckodrh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uldebweb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3btgusnya.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iijtxubu.html


<!-- 参考信息 -->