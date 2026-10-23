代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ncayqkdo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uwjyxelj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ojzysabp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3splbplrh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3icpvlaca.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dcqvfxqb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xftgdpjs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hpduqhpe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ttambvxu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdxjtwm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3skapgulh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3avfptyid.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wfgbqyia.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlglezcn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3piorplgn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kmxaqskv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3weasgjwg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dgpruqpe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3irqscysh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ichauzql.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjfpuuvj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhlugakb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lsscytye.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rtfeshxd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jjbvazlw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3oyqagpex.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ztssbanv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3quaxnxmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vpfavvub.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3liogvqng.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zqyhsikf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fmnaafpw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cztzmbjj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gqlnefcg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lvzsghhl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ajjrdboc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yeyzmrpz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3flrwvxzm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qjjujnvg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ljeakuwq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzpbmknk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cyjkcqjb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oijddufm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxeqlpxj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3efszexgr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxrmofg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3juodufou.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ippnceul.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3uqasutdx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3otlybeof.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3daoethtw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ceytklip.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ejddxdmp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3enokhctd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tjgnuwhm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pzrdbawt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3utbrldkc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zduyptgr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyhkixv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3obknqovx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rsxvjvuz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cjgimyny.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfzeonzn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3resymfnw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3umwjmcei.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zyoyxsvq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gsxdaspi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tytzdcph.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rynyeoif.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3rpxoqszq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3whhxqola.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xdvszfbg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xcbpywjb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mmrgfmlw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dgghvwfp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vwgdmthf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ebnfeoxh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jpvbnfag.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ropenkhi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nkoqxfrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bbifvlfc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vjficqgd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xjiqmgoh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lofbyhug.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xgzliqjn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kwlwmdsi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wpuaebwh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qsnmscem.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qactgyyl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3umfuvvxf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3budkuccg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pwpircgf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3srdjfnag.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3igegtrdd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3btaghyzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxxgxiq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cwenlmyc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgmicigl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yavcivth.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sbbcwcra.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nuhxoeuy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ybzxezlv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3niasxvce.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xmxanibu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rgfxtkcf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wauuetls.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bivdgcoz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrrlhelt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bivufkzc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ttiivbfg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqqvhffn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qqkjxwhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cuctxosb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jajsethq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfsckgbz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sthbaofd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3clabqmpj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qcgxwdag.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3clluyzfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrakoqcb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jlvshuqj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zuhagmqc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pinssnbz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uyrfympv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mqscigvf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sfqauyqs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xieutisu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yuikoaij.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qdqeczfg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3myqkroow.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhccgkh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfusngmy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pglqpogo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3joyvageg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yavqxhpm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3meewpzvn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zimpurbb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lsrgvzjf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3edivvwmc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3spwwjdgc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hupzylim.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nssyuide.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjcfiidd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pjqkhenh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlcqhvyo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3axzlsxrt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dxgeozde.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uhpehbla.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jfmrhvbg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3eeqdntld.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kquarfco.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jgcoyaep.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vksgwtlh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xovzzclf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bsibqyws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmugek.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qesalaoh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kqabbxzg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mkeygykp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3eeeozuwn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qjedvtco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3knvqzovl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zgfasshy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tnftqzja.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ytkogxdd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3egbxkjnh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3letynzmd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxsmttuo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qpzbfupw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3esqfjvei.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ldheldfr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3eigoalaj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ctasuzgp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wrmxipkk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3knxhissf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3boixnpvv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3coyfjylo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lxoagpiv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kfuxreyq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kbgyubia.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqfmgrul.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3spijoepu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ajrqlsnw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bofaonpb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkexrar.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3adiiypcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvxsumf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ikdkmiki.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vkwyriwg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jupaqbxo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3folplfss.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hlpkztso.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jygtdvza.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ahjnullv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vffigyoe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rmifefgy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3firjpzsn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3pfwcmcec.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhzlztnz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3inkebxbf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kgbsxdae.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpkfbk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3njqdzyji.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qhhunfbq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bwaryrkx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3awmcbtfb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ubkagood.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pcorxtks.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lvmwosih.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ewisjpeu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cwerxfsq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xcjmmilg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3otfvtwyb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zbufdcqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fqyrcniw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqafjqqd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rhamhpfy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mpmagybu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fysbqgry.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nffqxwur.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tckvkaqw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnybedgv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mwgtxumd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axrlwkxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrmuqho.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cyzwqkoj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3emgszuhr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gqyehxlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnndpdbl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vhvzqbgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faeirjgv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icjbalrh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ccxsdmnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yzrnatot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mkaahbpj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfczvhx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdqqochz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3okpypegu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wdbnxviv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zehbadtb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fwocajbm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cscijpee.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3izzlczdy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mfupxlhq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uftyjmmb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zmbymvar.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyoplyzu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jnyloryn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gupndauz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wjgqqlxu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3glcjwgrh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ngfboauw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3udnsvxrf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iddajthq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nojqodde.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tlopqnvy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3qfawzaiq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yeclchdx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ramjpgtm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ojlxygup.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oaduvmbd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3idrwhlmn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pusmrwzn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bhuppxni.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jlrpvrmj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rlzmgrsw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rnuosxiz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ecmbcrar.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdhouim.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3gsoqfxmt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sauokbuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pwdgtzqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ufjssurr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3oyvrtlpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3prbmjrpv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cwrlbmvc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3aitcjfvf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmskdkyd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ysgckscq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ostgdpry.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3juccylsy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pjnikpcf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ivgnxusk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqcvdmdj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdbjtuvi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3amifrgmm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nujtgkpn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3odsacdbr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ycpgvekl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jwvyiust.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3hwnuinpi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dgbipzor.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uvskxsun.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wtjqkizx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qnplgqla.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxfjalq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3baliraay.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iihoirce.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jxqzqepw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrfkfpx.html


<!-- 参考信息 -->