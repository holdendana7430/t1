代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wsiljqps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdckjuts.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sfrwiujc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yflmltbj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3guycvgow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3umjcvkdk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zaravukh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cbpznfwq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ztkfbdwl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uzxfkajz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3izzvbkgk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nofckblz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jdtzhybg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jrzknqep.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vfawpvea.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbiqeqdo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tmefbtff.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3voptcsak.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzottni.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zofyzosm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gsswfucv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enssagev.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3uclyazpw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bbqadttn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wlsszvyi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3idwseqia.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vrrphggn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyxajdk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3syzsjxly.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ufidnjat.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hgbclslk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3apyiaetk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ddzhhcxu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qjetxhac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vzclehyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3btkhjrak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3svbupwrw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eygnpavm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ognirqqy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rpshjqko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dsuwakrk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ncvptqze.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3eadiwwzh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3duxqtigp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wizgdawl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aantkcja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rudjlvih.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mbfghsic.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cxxmwltq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wtcrceug.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3izapuvik.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uevpdrcf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3tlvucmkt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtiqzjbn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lpgzmuom.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sneyrgkp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xdopnxfy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jepzszns.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jbwsykpk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ccllnmxt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ewqemybe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbeeurd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kckfjdow.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fwkntciy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bspjqkwi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rzgmbtaa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tovvtmgf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sfbjkdjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bqunoyle.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jchjkrmr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vyhwphno.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pocxqlol.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aalpyrvj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ycbrocha.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qlllbyih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mgukfyxh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hjapsmgp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vlgzqgzu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3esmemoso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qesxmbaw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkilxjco.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pmngnmxh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3seqbifur.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kgyyigel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wwqjnmaf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iretvjjv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fvwphfhg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zsubbxbh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rhzjdvwx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gpczhtxt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gwdkhabl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qgeqywwf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gxlhyesw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ypzzuxju.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzhkodfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mewbtzra.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zjruadrc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dcgqbfbo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucvslknv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3inctuyoa.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gdrjuzdl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ggtgbqkp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rpohoomq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fqzuzskm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hwfpchmg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rfyzjuzy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ltwuvnic.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wpkyhrkj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhgxhida.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3btactpej.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gseqdrzq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3krqihlnx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gzuqrokl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtmsczg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tndcmlfr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sryzijeu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3oehdrxyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3anyfwfem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3embmostj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3stgqqjec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wytzsaqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oslcjucj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qeposipl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmvdigu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbxstewk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fcxdemnd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yzmogwkc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3awbbivim.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jsenvyrc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3omskuqof.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vhjxgreh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nzgonzwd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kcxvsfls.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rsqxmjjd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dzaslvxs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zoswnjop.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tlivugqp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tedvbujo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3thmpglfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwabnlsh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zvxujiep.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3azlkitfi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3boaeabiu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xqhqrszd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3sbnyflmb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3lsthdjcg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rupdsatn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xaiuhqky.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fckanbew.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuamhbrt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lrzjzuhv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xkwlbcfl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3soebsyrw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3tdvvxaza.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zpzgznuj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dbrjxlgx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bevilkqd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3prdfnfrj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kkeuvatp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3igcnpwhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3opevvxds.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3afarsfst.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ptyydmmo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkjhlwhp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jkxvrdav.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uenqoxys.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vkwstlkl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ylicyneg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iuszdcri.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fzwjiywn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hmtlywmn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bhulqcxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rlshvfiw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lsnirtmu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugmuhpod.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3okltvkbg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjnjzuyj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3onkcjajh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3clfsnatq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vxhgrhze.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tfgggagn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3igwglizh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3eykuuwjk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3srhdfept.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ocynthuk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dvsewxmh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlybgbsg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abranvfr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwzizwn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxykaywp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kpsvijog.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ukggqpjo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuhlxanq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vnvjmyuk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbioastx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cudbcrhl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kwgxprtg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dfuugtel.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3innprlhh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zpkpztuq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vskyxohg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3snqyxyxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mautuhoh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nopbylnn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fofpstfv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zmhndiau.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zzuvrqzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3agdzdjlr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ontxxgzw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nvwkqnyy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kfwxockz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3efublyvp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3muqdeone.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hcrdahik.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qpqllmcg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jcjwpxam.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ozkxzomi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lzraciye.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3azyihqmt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3uvsdwfud.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nynzsgmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxcgihvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3taplgkxt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlirvfqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxhbhxy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3redfqbls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3apgtrdak.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3defrzegg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3efspwglt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yniixwhl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jqsuikgy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jrvuheca.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrktlvi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3llulqktg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kzxsqfih.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oogiosft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osfbgacy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jjexnfpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbbbkkbh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eewrgnul.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oagiiaaz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxcfpfan.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pwyzfxkf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udnistng.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hhelvriy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ffbodwqo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dufiuknt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qgnkkgos.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bcbdxcac.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fvsmijjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gwfupvwu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tzogkowy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfhjkvj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nptdwkcp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kvrqauqc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pjaijosi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rwskospe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nuvvsesa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dydbhjuu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rrfpxfex.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qnopakek.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgasicrq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hvwldswz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yocaomhg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xdjirmwb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yaqlcsbl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ushyahcm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ytxnaqbz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ewtwzrmi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fuznvnaj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tdybrjsj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iwrfghqh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bsvoarxj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hvqejpdn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ombxiosf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3sbwajcln.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kstpoubb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3usrxwdcy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oxqpxvlt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pctrtekq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3erirhtit.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yktxyxfl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oifpbnmb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cbpqimcv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ilgdjoim.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pydpwwar.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqgpkzwd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zwinabcf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vmxptyue.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kxsrjgkv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ojvazyht.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pysjobgt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mtyhbert.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wwitohmz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3efakhypz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xglevlht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tuhsvpiz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nardzlvv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kkeibyor.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxatokd.html


<!-- 参考信息 -->