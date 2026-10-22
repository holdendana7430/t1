代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ylswpfen.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yeylqcnw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wfqkutzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfysidin.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2npckunky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpkciyta.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vwvcegpf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2flspzcyx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hhfafcgl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mpqkijbs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jfqvwofj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xyljcxyo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cvpbluhp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2krawganl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mzdtwoec.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2myyjxsca.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jjtrnblx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pixutmja.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybvxzzlf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qflwnohr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nfszgarw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tqaaakam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2obzdrgtp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2relemglv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tesbjvna.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ajgjjedi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xmycwydx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xxasnsof.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzsrfgd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sgvwejlz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vqwbxdbm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ackawqtf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xswgelkb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2byngvusj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2paxqzqyv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwlufctv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2utuzehga.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qxkhycug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zgznndii.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jytzpavh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unkfygcf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xejvpuyo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2clqamqvp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tjwazxgi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mmzdoimp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fnhniolw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgpfrckb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gcleefxr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dozsmepk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nhiehoid.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2borljepu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jctitodc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwuanqt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vodunwsk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zpgrsrae.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tnnpucdn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2adhupdrr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2owlinymo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2augibocj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rlsxzado.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kbfvzxvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mwfwgjrt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hvgubjdb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yforzioh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rynslnga.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbtezdph.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fignekpi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uhgwlaai.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2crgobhiq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pmfgtrqp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnozcucb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2urcwuaxv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xmjqvgiq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ddbajheh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgruwkgz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2akuyzaev.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2odraporj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqkqafwz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ehhgqkym.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dscdfgka.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkwhjbqh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hyteiwid.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pdsrpham.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cpchucvo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qehdkvjm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2blwxyueo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lhcbapoy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2oyyihqwn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zuvkbcjs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2siovunpl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hnycekcs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lteydoik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrzgepys.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xsqsjvtr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2shnnxlxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ljxuwijx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fmyklgmp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqsstk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwobeg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qmrwevlh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dxxzlfpu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ugdoyxlg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utcmtbtn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lmljupwr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dqwrpnvm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dlgavxcj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2plxykvaj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hgdodstq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2juarzixz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zttqxllx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kqysjqsn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jinsgvvt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuyqrwe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xoinklwx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lhsabotu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dngzvswg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvuvxduc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2twxedysz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2odsazloj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvovlbic.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxercr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hihayipj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmnjpxho.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2esrqexfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bvrxdnin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rnockpoz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnxdyesq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmgdomto.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wizjyoll.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkpoxpij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mlvbkckw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqvqptrl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yfjfdakt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ytdweiyl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dkfbgvih.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ihavwrcu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rholulzc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uspvizqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2dwrhewbg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kpwtzfgt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvvbfrdo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mfttuzla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxckxadm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uelliefa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ysunjkxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgwditr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2apblscuu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mebkxvmr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ucxcobma.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wsjasdqy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fzyhtfgr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cpzcaqrb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fnjhouzw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgfivur.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tbafxefh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fcwnlbhi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxbkqzc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2eyclopzb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pmykorrd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vgrazxbe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zaibdnom.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xsgziqlo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jomsqdku.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vzfuclri.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qmdfdres.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iikxrofb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wtysttlj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmvkjdyg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2olgklnnp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ghbvbcip.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2aqivibno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jsgeinkp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdbwkfx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zjtwgwuu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ewbjjyph.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bwymlraj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yvwxeceu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gkjuohko.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xplnywyl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dykceeni.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kxlhtebx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ptsajqbd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dshyqxva.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kxaixpgz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lzvcrkwh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hdzoevfp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bjiurvaa.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sfsfaehg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jvekgqmv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ligmolwn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pgzgttow.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbwwebv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xxwqicgr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fppwvezz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuuiuzj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jxteaoeu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dyvyougx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bgbyjacp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2laeiaecq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kjzlvtkd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wkrkplqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bgbeiljj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ujeytriw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fnfrcyld.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iuzqcevh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rkpmnirq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mccfumlv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rztnfezf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vlmkaeea.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oivuuspr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rxpyujng.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ivuppnaw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2noxvewmu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jeovwkji.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ghhztwin.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vjkyzfca.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvatbbg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nfdfvffl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2yxpctjvq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uvjrfjzv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ptfqduxw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gyacpcix.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xrkxwupt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rnbtkgwk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jndjfhjn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lsyqtwri.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yfuodrui.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmuffjiz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mxtysnpt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qeibqufq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dghoqthl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2seoywjgd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2getvlqjf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlnebbah.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2trrmtoou.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2niqnhzfn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvqbxbm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cczncoie.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2linyxmfw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2niqqrxcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mucevpxd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zloaapxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwpytrlu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blidnhrk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gtnlpoti.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dipingob.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ayccuhdn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ilmysfys.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mccfhrrd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vatzibrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mgvvdred.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yokmzxmi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2khyhvidq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dfkbhplw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2beuwwpki.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2srntauvm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfynwyoy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2twgvdwnl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2szsfdhmr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wzxpyvto.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zswctfhx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hztfipsk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cftvjqpl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2opnvokqa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wzfbglms.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xptoczfn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cyxuboca.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2seljpant.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yqztuyvf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2luatefqs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vxqawtuk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2haijnuui.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ydfimnbw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lyexgrbb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sevcapfh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dzqxfion.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2eaglwjtw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hvgbyljy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dlwcksnd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lgdtxfus.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gaushypj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2asmbetla.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2urlcwqas.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zqpltxjm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dvimxscv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ufmmoggz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fvaslgyr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qrpbgvwu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ddgxmyqy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cfcmhlmp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2siefkzit.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fnwgbcli.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkgabxe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gownlrhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2altipbbg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2implsqhf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pojdvhkj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2accnvaxj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ubutkufg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cpfqfwav.html


<!-- 参考信息 -->