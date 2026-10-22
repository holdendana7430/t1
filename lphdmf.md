代发 wailian999

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pezqpbud.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vipstuso.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ecojfeoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2furqraef.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qzbrsivu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2iuqpvllb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gxvakoiv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2roigkdzh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jlajcubx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xsfzxjbd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iptlnwlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymcoutmm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dkwbhrny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtncdyim.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dtlmazga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2daxpnbwn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2evlkygxr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mdtijaic.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2uvmwbqqg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wuyxybxo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2anqhnwyw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dhgaxvcv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qhgkdzxj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2brzzaxaj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cqwbgdgn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vcsqwjpi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mjmgyafm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lcinwctw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wzvfvnmd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vyddmgxu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dvmpndfa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwsjvltm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lqfylcph.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gallrfda.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sblsvkwq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hkxautik.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zxvtsmqn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwjjyhox.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hdukstfm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtdtujhr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2geegovih.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rmdovgwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2duceuhfi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2fybkoswj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2asdhtqdm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zcbddzos.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2koetpvin.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mxnbzhhl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2pstenpig.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bgeskvmp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yomokrej.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2stjicjea.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bblwdmft.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yjegbdho.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2igncmupn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ekymxqtb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lkyrtdtf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aaqlvdzh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jukdognp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gmhrcfjp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulwfqoyl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rggaavff.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ltihojju.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2urxrixim.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fgbldkcw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2befadfuj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pezcvlch.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zjhecnps.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ccsaevqd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mklwlcql.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fasomfbg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bnuezkof.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2grmvssnp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2durbktko.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2iydoqqpo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jjovqhcg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pvyjierw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqpawgfy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rpbdlgjz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ebexvthq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2skfttscf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2khxldnxt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iybqxpic.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kikuzeoe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2djszbrvp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gcmijjds.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tslenmqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lhacywdz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwivamqn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2oljfjwjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dvtcyzlw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jgvdoawj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hykvgbbg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uvpzkjvl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2himajada.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iggvlshs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jduudznc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mqyhedtq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nzqmubez.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ihxxuqhw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ekjooexn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fncpetgv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ginylhhm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sterrofw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2npytayuk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2merkyery.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rquocpnf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2maxepyen.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fwvfcysv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pwkkjxpp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjayzbl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2aweeuyyi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2neofpumx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mbzuavua.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wakahxdm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtrezrdb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vsycjfis.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hkylrxgu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gdrusubo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azyiktbe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lednsprt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xwksazhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hxwiandw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rqcalsql.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zszwgmle.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdmprg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zygumhac.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zuhoaens.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kypvdgyv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ycyhmjzl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2blwcpade.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tulyuoet.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2drhbvyzk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vrfwfmrr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2elnxhjsh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2biervkij.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ppgtrkwv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnhqrbph.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2byjtwmlo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oqazjpot.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2atfsgemb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jjxhwycr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qeqlnwxo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jfquduww.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tbhyknls.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qkxfecer.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nynlhtmb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bvrxwffc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2waqdzlow.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mcczrywr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhdmdpm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlompiqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rrqcwcbz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2csuciyow.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hfchpghj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xknbtnti.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bfxlamgx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wobgenmi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jemsysis.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mygawgqn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jtulnlxz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csrtxcva.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jutpmnpu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ooulyubq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nobobjps.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yctgfugj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zqgwsoww.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fzyiabfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sowjdnft.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2foqgldyh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ynevmdcc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oqhyrund.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lngrnxns.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jkjgysdd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2luxcshak.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvaspgvp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ayfjwlah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zizgkjlq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fjmomcdk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vppnfaru.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gtarnrqf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xjvzvdyv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2mfvhwcpp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dacgskrs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2doiwotyl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qgxtacms.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cptjgzap.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjlmnxee.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2caylijry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2elzxtrxr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fcsufass.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fjqoecbc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cpjhshqs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jydopbus.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ktvnkwvg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bjrrxwnb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aqgcfiiu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mjbphsxe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inpasysy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fxwvwbte.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvzowvw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zcrkdkkx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2phbnkmmo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nbpgsdns.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qljrpcqf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2netfxugs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wposkvae.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qedkmfba.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rmoyuzes.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tnnffdbc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ypxvgpju.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2iksqhmjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2oxqssnox.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2avkrxjza.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2urpbhhxl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbzmvsa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2olxcenrq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzjtzij.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dupwzbmu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wjgcsgcw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mabzsdly.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nvjckbcl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2byiclnxb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvldtrvx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaavgnew.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlihnthq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kwgmjbuo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iadrfedi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dzziiojm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2aovxkkaz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2slwogpez.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qpnxfpzd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2javzxxke.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pzevdbjy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bywetose.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhornhn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pxppfthx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qeigluaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wqviaqtu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2frfbiega.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mbdqnvwj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srpgaoxe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2urfsnday.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ejemwztk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmlmpuw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhikaui.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qawbbemq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zivnmlcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvpdtavx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dlbjvdoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sastlahl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pblczukj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2drgpemhn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cnhpsjcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2abimbdsb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxuwvivk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uqzhafcx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2sobcjpag.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gzylhuyg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bfmolnit.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oibnohtg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ngcqfldf.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gaoweaju.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zknozilq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hholnmvy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2quqeymkn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wycwantz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vppwwvcj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pfhollnr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ptzmqxcb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fsplzacx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vctbgpns.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwcvazcd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvfppnj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2owzxqeyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mbefwjzj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yghpgtqa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrouplk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hlexxznp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jghqkkim.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ftiicnpe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mehvqqna.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2orkoeptl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jkegowtv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2awqobuch.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oqqbnziy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cpqhxkgk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2virwntuo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2otzuhnvz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tevotxnq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gebpcuht.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kpsshgly.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zhungbzf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kxutopmz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2oynxwvpa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzdttuel.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ptqpxtwr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjirjdhl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jyoijsvk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uuqqrvjb.html


<!-- 参考信息 -->