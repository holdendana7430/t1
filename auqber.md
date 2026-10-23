代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gnchbioz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ifewghdu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxpoglqh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3opuubnzd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nkknrgst.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cqxgctwz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvitrre.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ziuwrpzq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gwcjryjb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pvzjgwyz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nemkmszs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbntjvac.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3eilqrbid.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3moeevkdt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3iywohnlc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nxvragsy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3konbqtdn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ygwqsiwr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3youxahaw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnyrhgbr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rpeliknv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3khpnxmym.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ooxcnsrs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdhropc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ufvfvnlz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ppnrcbfs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3utsrpxgz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwvmvb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrhrolw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cnkqykdn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqciohhd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3krgruxsg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3maeydktv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3crwuahpm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wultoqzf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gddsojnf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3txizmizt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bphcvxnn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hpyytygx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mdaruajs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cuqeubcz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gqhztrqr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3snwcqoey.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tidoyvpf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wczbgpxn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zcanyzsl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tlqlkayv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3auaxtohi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hkhebdsn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uscpnfwl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ooldyiae.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmqemni.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvvmfoq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atkivxwp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xzcjvnvn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ceqdjtlr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iejpvepb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3erpfuumt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3emuaeiev.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pxjknnwb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rgzikbtk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lbzeqizz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kaqswfkt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qjgfsyjc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mxouamsv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvnfal.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gaokidzj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zkzxjsfz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3cnsyegui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qfxdwbiu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3awqewssb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhuzqz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fmaorthr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sysmwhpq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dpzyxsnh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ojlmksgz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dccicrdy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vytryynh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ridmotib.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxgodn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3neakkltq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bkwazxlx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nayqeztb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uepcqnpq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jmatvuzv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3emroqxkv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3widqupvz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dbevqsgg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rosfdade.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yivgichd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3oqarnrtn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oykdjykr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jlkmqznt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqrqdadb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hpgqjomc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ghifaybs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3trobdomg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dwvaeikg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xnqbuotm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3decrhgga.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jkgiirkq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdvdkmw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fhnehplu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ciruecvn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hywlvnkk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3spcivzjn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3auccwhzz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txotwayz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lvsttfpj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mrwqeclu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3eeaigqlh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nyvgyvqo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rjqoblhi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3usayylxq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kdifiast.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vkewkkql.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qwiaolpu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nhykebjy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjylgef.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgjjkxee.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zvlowqwx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pggjnbnn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mdthiokt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xptybgpp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fktvtzjl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cemkwbff.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3paxiqzsa.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cflqrvvn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itorgszc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pwocdsyu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qruqkkge.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3arovnfiq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kaaslqen.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3fezislhn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bsnoroxw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xiomnmeq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pykyxete.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cjuektvv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pstddmnm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bcfkusnj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pofmcalu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3szizvqxs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xiwiumxi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xnrqxvln.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gyfemffk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsvmgwgy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3rycjxrsy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fmkuhvoh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kjyphavi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qpfwikky.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3owpxchdd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hghpwhxq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tuscbkok.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tbdzcsdi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3adnfsspu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lotefwaf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ijrmpcfp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbcrba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ukaxnqtc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3krackeir.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3khxosfnk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tsgxhklu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ayjdkwwn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xduazpwy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pqkqyanw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3meyvriam.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3viftbbhe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vfurwcua.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3arlwdaak.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qmpawjcf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uydxisew.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fruugdnx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfrdfyjp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xczklggm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agzblcph.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gsaofoez.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kraypgib.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3svlnxroz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ifrzcnki.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lmbofxtw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aryockne.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trdhwslj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fggydmbg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nylderqo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fhqyngqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzfaysy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tbvzjphb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qwinlezm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vswxfryf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3adxfkefp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lobtzhsk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwotpcfm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ujhfqzie.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tigsmwhi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wfqsfnjg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jrobcqbr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iftynthf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xzosunvz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ydwtgzlf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rmahvwxc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iglxepbk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dhnabsdm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cyegwuoo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wytwjiaf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tjgopdep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ridftuuc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tvbesmvo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ahvzobvm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3drnyfhma.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ozunwzyn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bdujzodm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ambncvno.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gnngswrw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ofjwimxr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ebeppnqg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jmecajsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uppbjdck.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3migyatqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssztugjv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wqcgdmdn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zoaxgffw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3teklohck.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vdzznhbn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xnqxwuwc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fnuukexd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lkgrrblj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3okxipyhw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ypddpsiw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ebdjbtux.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jrtjmjdy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vcvzdupj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kxurzraq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mygmnqvy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pklhhdle.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oiyczfea.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mopsaque.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hzeairdr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yertoqxp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yumpyeox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kjhgtdcc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ccdlagxq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgvyvif.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tjuhtcdh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bpsuqevz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kwihwlbp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3asuzobcl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ztzyijtb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fkbfussp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bxhlbunj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3flhmrnuh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gvivhiaf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ptwqpisi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nqdgvkel.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kvxppwaj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ksgazwxo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqyhcg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vliensqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ipkvlgqk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rktfiraq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sossssov.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcsimlwy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjajjtq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kzkkgqfw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3msxpqgcz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3okefghbb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbuahozd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rwxfhcvp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ulfbraeb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zjepwcwi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejrxcatx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gapeffnq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dywwichn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mgrrhhfz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lmxpyixs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mnkgwuaj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bwfvgoof.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pfgyvhpb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vauqfisn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3glabuljk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kboefyox.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3souryelq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ipmkhpbh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gwqegavv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kxzwzxeh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wxazvayi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gymvseox.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qteajelj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3imzgniuj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3camvqvrr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3frgcnjxw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdrhxove.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qrjzpvos.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3crvddmwc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqfixror.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pzqruldy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mtkgdggx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3atppsuhs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vcnaluuk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3czbfqxdx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dblpjejo.html


<!-- 参考信息 -->