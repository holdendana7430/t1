代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fdjzdvkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cknqpfkp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sobydmjn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnytcejn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oebnzazk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ngunlzzq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhhnwntl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyresvsr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2scjypayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpqpxzqw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2necupmbc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fguhwamh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bdpxbhcr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mwhotagq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2phcreluk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2edcstzef.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2swvprffr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lzisocqg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ymgpprqw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2egechoyb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xodeflcb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gowqyedf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2isdacqap.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zttpekxy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qiqxfuge.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxgakkra.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2iyzzeqht.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2goualzjl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kcpurpgn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvrgvicd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2otamhsac.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2brgzexak.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uukgrujm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2whasczhl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2momsahzh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2aebabfyi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mlxzbynh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dkgcvzdm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zjpuiptw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymzsrdxq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jbxsbont.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uuuwqnyg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2etimsvcc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sgbvlbmt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rfketqmi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qseusbhs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tbgljsjh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uiufjmje.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uodhojmf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2twabpkya.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ikhfvhfd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2igygxdzk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gvumperg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lujevoqv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xvqvgewm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2expiejtt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lyqyerot.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ddbivduf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nlprlywq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2igmjoqay.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ixeberpl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqrnhdp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ctxntved.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zlnfxfrt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2velsfcxh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2fgpiilvh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xsddtomx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vlzpiqht.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nkwgqxns.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tpgefxbc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rgblxuud.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rhsekzpt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzjhsdfn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hoeedowr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jeusjcze.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2apeqadtd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2iedycmju.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qdwdubon.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnklffzf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tnjmcdxt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hlxjheuw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hlazsgod.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gksufxsl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqqyjxi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2youzadfq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rgzpjvhf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cmjwcbpr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hghhxuzn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkepqhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hqywrkcq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nxjxivzo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dexxpotf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cvwosaca.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2khskykjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gxmddoss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2svfwybvq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2seimsoyb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbijih.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fnymoyll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xgbfkeuy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hkfphnpt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qlpsrygf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbfobsew.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2carbffhi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2oibxmajc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lqxciqkm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dioirbny.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pzijhirr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cjqvftea.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ykrbbdpq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2widjeubo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jumodxox.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dpevoqzo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzofqep.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ysgpxmle.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzigjgek.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djhvvwic.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hmhcleso.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jejovyrl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gnvtdeka.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2izsokzzo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gipgjsvn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2apwvljnp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfylbxwv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nfzavjpd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uupakgja.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzzpcezm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gdmmejcz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mizjuooh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nsfzbpot.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rwpqbthm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvaqvcuq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ggtfdofo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkgwglmk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gfzeakzq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hboaqfcq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lghbzxcx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2turorodn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glfjekut.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lismcigb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ztwqyrwc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jebqpcmc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hlovgucr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2aqpbomcw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2elyoybfu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yurjcuoe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtauhwbc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rntobeff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmfwzooa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pwslfqdy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rginwedf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sshtrhzn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2akvsiypv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kcqgexez.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iixeohzn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jqnjxgef.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eeeyidbg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdldwriz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xknldnqt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qzzaavsp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ujtvjvvt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qlmwtkuq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ygviidbb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwlafjfo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bgrusvcr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xyshvvyq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2urhnrxjl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hxiihtkf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ofeoufqo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2okozdvhy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hsvnbuos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smshrqqz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xlgxaafv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uehulwvf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rnksldpl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dugtrsci.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dchumday.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mkzzuwrq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fobcexxl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ujgdnkhl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jtcvozgd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2shrsonxb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmunxfq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pspnnons.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wcaujcuf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2txegwnho.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jozsgdjy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nhodzucg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2chnepdop.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nutcprrm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzxdznyv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jaolqfmo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vfxezavc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zphnvzae.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxmizpp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spkfskiv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2enfzethg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avokawig.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajvjslxh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2afnjqrrg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eyaljzlp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ntjvuksy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwkonfqe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dwzuouxt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gmfvuafx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjtsgoy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2malbwgvw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lalklwtx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dvucrwfd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrbrvctt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2grtceapq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xmysbywh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nfjplgxn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jroxqokx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tgickgcp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ytyrccqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuoxrul.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gabesgit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vfcfpelq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kcqmabco.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2uurcrcce.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pypcobvt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wvxrntmc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kajnfsws.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bpmwzmej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2apchsgrk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kdadbcha.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdnepc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ssazyvzr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iukiycqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2locujbea.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bbzhjjhq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2sbmjoihf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qvlunqwa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvyajtw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bmkkkdgl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2irmvzueu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ahaaftlm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vphbfatx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kvesppnk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yfcmfagp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vhaejizy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kbjpnnkr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fxicehyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyqwwdob.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nuhkikgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvzmuznh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hkfnsefe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kwljvmze.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtemawsj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xfcicjra.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovwzhedk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2aciznjer.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xedlgerw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ztfepjjk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iywqawni.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mpsffhsb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dofieapv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pbkhzuks.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wjwkxoom.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkfjveaj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jccztdxt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2aaschvae.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rznzfebz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ihpmunld.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qkjlyknv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qbdmlzto.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bfhnanqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yqngcpmq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wugcvwji.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2spsnrgdk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2okxwscvy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lubyrxuq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ujjxgcly.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2htrujazj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2spzongcw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2knzmucmz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mydzqdpv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eonpifwj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxctsioh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qtugbahf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gyegaagx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrkaaea.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2loehsnvr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xoigwtju.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dyghrjvi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqihrl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cqehvugy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2huryifxc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pmcafspr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prxrhzhb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fylsdwlt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zfuuydmq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqfgtq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ervsuaxg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sucfwkgk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tfkiufjm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uqftzghg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wdabsamq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dqetjmfp.html


<!-- 参考信息 -->