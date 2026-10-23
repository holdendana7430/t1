代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xritadgm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jgurufeb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gewftrya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azpkuhsq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mfiaqgcu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3znrgrzat.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sssyjric.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrgqymfk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nzeabwtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvxzoolx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lglnibvx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zxvhgdrt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dhrinhgx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kwgazguk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ssyjehsx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3knejjgot.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hrnyljut.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fxavkqpt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xalyjxhk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3huawsavv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3peismnwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fiztuwxk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dlqmrjam.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrkwivlx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hiqfmwcc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wpofphrf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3flphnwkc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kadrutcj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xlwerrqx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwqvxun.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3llexjpln.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3obmyhyzm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lluihzvj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mfgjexbe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvziwee.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbxftqso.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3naplesdv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xersuhil.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bsaykimc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3whxocqed.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jzipsxyx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pyaznbyd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfewsyf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzjamns.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xwcbvjuz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ovjzctne.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecxcdlie.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mebzggcq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qlltzdwq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cgmhqyqg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gjytuzzh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dbymcfdi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3adlumird.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bjfihzed.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kwhfdddi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zngdjnlh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyslbyru.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ooozmxte.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pbgsfbjx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3aaokniwy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3keanoqjm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgojmnid.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xizzuueu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3zrapgwld.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wnrounlx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tdgfgchp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rrfbvncj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rnrknjpv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wvtqtrwo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dxpblzdh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jcmrrlmj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fwqipjoo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qrossirc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dyrrztzk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3onoxjlrt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3azxmopwm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gooscfsd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3usonisgk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plbmtabz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3sjavirqx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vncsrjvy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3opkvjcsb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hmkxdcpv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vvizfwbk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3onljaguu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fjtrlsfc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vcohcyin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qhcfzzyt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekcurxxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tgehliif.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xtqzvvcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mwdjtfxl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yzfqinvv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3phkyhmaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcxwdwf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwmjkpo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3aohupdxb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hvfzpbrx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mxdwdpuw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zvcojfse.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dryptacb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zrpxueig.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eibwzqjt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ixkcjhrq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pfcybnpx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rfsvtbnn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbgrwtw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzubkt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cdznlxlk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jzhzrsvs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3glytxvyk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stngignb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xegpybfu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vsccfdzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xwepuoxw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pryxjsqo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ezatwhzi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gzaafkbj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dvngcprm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbqoolcw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mcbsdleb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmhggxb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fnuczsif.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nqyjvufu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lyspkanm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xbviiczg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lbgyqyzy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3njaipihm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3atqvrtxa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hwrwcbbx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gqebheio.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vumpdyxe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3adhtdphp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zmcpzeyp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3audjxfee.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fwnhuyvy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bwhodvgu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ntfhasof.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nmpwaxfv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ppoijetc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qrzlalpl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lurveiyx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3acdmudwx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wgoyhsae.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxwkmtjc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3uebfujgm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewziuxqk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3htzldbhu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tveykjdo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3szmdzmqz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xawflanp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lfvvlgpy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xqzgniim.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xyewjkrs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wnksqaqu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmpejep.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yrpbjwjp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tdgemhrv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3exofxpgr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dgbjbobu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcikuyn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3biuwnnet.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xouztocp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pysswsgz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nejisiqq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uajresnw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxltjsb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xqtgmwzy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbajqccq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qjhvhkbn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3edihqoms.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bxsuefoe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ecvzqczk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uqguwsfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3onizgdme.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3esnbhlzy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iekuaouh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tgcdhcus.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3njjxzxfk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3aupmlpck.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qknkzedb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xcfarnih.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfcrlnrd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3insonkee.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ngmqipju.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3exzljljp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3joylzwms.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tvomstin.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3idjyvhzu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xrmwjaqq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fuhrfpoz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fosevhtr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3owhencuf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wvmsguse.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdkdwg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhhbmyjo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgkyeud.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgglwfck.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhtgafm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xqlznjex.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvlpqdyo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xgmbjfrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nieniltx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3guhjoolf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hwvcvczq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rjiizdeg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dofmpliw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3etyqwwtz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kzbxhnxa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3egadduwu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xhvnzcjd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvouyuko.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ppljfxgj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3tvykfaqz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jfxctjpy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qbogpsfh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgjpxr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pkxrtgwz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xyfkqjgy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gphrbvur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qhonaupq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hlsgdynh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3znvjqchj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hptnxkyr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fjbqyrky.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nsldacjs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jouncjvl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dskuuraq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lgcggngp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zpzgzdzc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iyywscde.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ietjgmam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ajkdcoxq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnictwkw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rypivdei.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3igsqvhjf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kvbbtsvj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gzmrljqu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uddvydqq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lwtputpx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uizcbhlh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tefxuows.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rowwcmaq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nuifjlfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lowesjgn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qpkmjrlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cipfipyb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwskaiyv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bkutbheq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uevjngqt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmzbvjeu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mqsumani.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lubkcvzx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kzrijgfr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wswkyqdn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjlrnyi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fnvxkhel.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wnqtltnc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uiovsnhv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xkpnayzc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvqnrccj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oplkyvwt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdjsjnvv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kdebgafk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qulxbmhd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ovnuwiyq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rcwakays.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gtxkxlgs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kjpzhiko.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nrogvvia.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ggfbacpw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yzdtreaz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kxiusqix.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3arptihnt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pvxajpoi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pidkiqwi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cypezwgc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3worioavm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rvirfjem.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kfwwkkrl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ykgpjdim.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wtdhgngw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qzuwhcya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hvjszcwg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhxyltth.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fbfdobsf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvvidpmm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jombphqr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lyxgwlby.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wyhpoetg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3irdnkhnc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uelutdfm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3oidmzgiw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbaucgw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxgimish.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vquasxdf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uhbtubgs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vkczhruw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbbjfat.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yavhtshd.html


<!-- 参考信息 -->