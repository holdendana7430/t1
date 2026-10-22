代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rehioory.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvnukysm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kklsgnxy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jlaffdme.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fehjntdo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bhuzavch.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tvrufyqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nuztkpvu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xahmfonx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rfugsqkm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2twpugaxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhnznxya.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2uwaznshn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2yumqrxlx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tbhqkkmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztyywqgl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pkcwzbwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqcibkgz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eiozjcrm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2agynbrgw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dleqhseg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ivfjlnff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2impfyxwi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fvcdvlpw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cexiwatd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dnwtpzoq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gjbqfrlt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzcxko.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gbewuwol.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2foicxnqv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhfyihec.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcujahgw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2quzfnekr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nxczctku.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2noatbggm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ecmcgspa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pfleuzqe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2arnmtdun.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xmexusdi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ijtbsuxe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nspbulie.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nxjuyqou.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mdozfvah.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gkclodur.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtbxyoxu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aulezcot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uumlnxmd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdpzecjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2sgqbnzms.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqtbuwl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kdecucwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2idavlttx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjrpaykd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pifvlecp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzulykoj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ajbdpihg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nwssijxa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ftvcwrmf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2udnqgjnf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2nomzforh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uatyyxna.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qqhljwzm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vylbugrg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xwojrkom.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snrwonjx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngpuhbvi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mtgtqvox.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yxlnmhpa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mldwvajv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrzxnzp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hbqpwnxv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2luocnaub.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qnmcausr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ztyktahg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sfltlxrg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hofvlufj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2juxhngki.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjccopay.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nqxbcski.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iedezrgm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vwbmfchs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qiszbkfn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcfejnr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2aszrexzl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lazwypen.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qsfxxiwf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xvosvruj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pwqorouc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2livizxmc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bghhqrdj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmvkjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ypcoryqf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjnuvreh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ditzpwzy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mnfnmfki.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nutapmzf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zorilelu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbpgtt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pjleklux.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vulzwvnw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ysrfwsvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ezngslbv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wipwovvk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zzxofhir.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ldpmpoxz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gdovvnoh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2csfxxngq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mhzbcbcv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjtoqhdt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gvomuonu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfqdhvyv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yxamnwlv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bhbscpkw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ulhcesxp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ppitqelq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2euuoqagx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xvwzhdmm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zsavrkoe.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kncvzizc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2svlriqya.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wieqocdi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmwyfgl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yxtemvlo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bmrlswpy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2veibdjog.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wozzngmx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hmfxagqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2eieyhiqp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hrcjevnp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dujmdbin.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kbjnccmq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sldhursk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ucvhurjq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yelxcipb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ommyhwjj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fakhtdcs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fvncspua.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bcrwyymk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2levdnytl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cncqlkbi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mzirfges.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2efzloghc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pitkylph.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utxpdslx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nxkrhjkw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eifpfsuv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkvdetvx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ejuihbbl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wgckoffe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cedlbpiy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qnlqiwrs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2glghgdoh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kxczinxq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gqavbjxw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcmrhjce.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yhenixqd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovaocoxc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhklkseo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ymshlbke.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vbznulsc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gqonuldq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hlngwkbl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pwwcsvnb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvizaure.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2tuynetre.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2plrpanbd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rpptxdiu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gtafsrgt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpidfdmz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oaemsvfk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vsbrecem.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hlwrslwb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vkppcgml.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xirmtryg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lowmdree.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zssosfhs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dtezrywd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wuhxwkzr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yjdenqkx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fregbwpa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kkjtblxd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxhgxlw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fomsgvsc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ikyqxtty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2prsnpsuq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cehdksbn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ussbflgm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kwprfzfh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mjiwefom.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ydyjuepd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnnsapk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wvbiwwcb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xrxfbrmv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eosrchcl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lzbaxgcj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2coiyvcek.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ictrazgp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2piifrcfz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ieyoyjqe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gkewytro.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2spohxzms.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzamcwyx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rptqaprd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pfshxppk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zpfdiowr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vecyyqny.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ojqmghec.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hnkyhtlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pnrniojr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ydjkkmkz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qikemrgj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wgjtmvtd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kcbjblys.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nyricpsg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oazssqba.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2gfzzrhmw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ahwwqcbm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gswltjsw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2muafefxg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xngajfht.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zkpxyhpj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2atqyibwm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kpcyhnai.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2srkyrzwf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fypwadfg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nmlzfwqc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aetjyzpm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvlpzbrb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oijlmgbh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2atzihxyp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wddjaixi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yyawvilo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qkjqwsrq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fjoyouil.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ytvadzfb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ronopcob.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uyeqocms.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mkdpxxox.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ggzbguup.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ozplgqey.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2deqyvvbr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjjqgu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwzdqbl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwfauemk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rxjnllek.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nbhhhycd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qccevyxh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uoipmicm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lwfqciuw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2swlroojd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fpjkbipp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ijbfqsbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjumzdvi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qjmqqvuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suuvcxkr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2snyzzgcb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yyybgkws.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bxetnamj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cdsczsuj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fqmhxvrx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2emgfaczp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgnheih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2swcwtndq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xlhauobv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhdxkfir.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vkzcyjso.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pggxpnye.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wmvmhdpa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2coedkkyk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2estjadfa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2naklhrdk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ysagrkjr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vhllidsd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ubxctirf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qhygzvwh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jyienfdo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tebeflri.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wuccrbky.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lyzcxdbe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qxvysuuy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ieyvjyse.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ywvqqmmh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jdgdpdcg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xxvgxhes.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vgpuiurb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yuxzgebi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jvtrsimh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tiwhytkq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dctrmyzy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hrcxhgtv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eqgklyem.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gfltkdes.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wwgfflnm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lexmrtnx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qhipbbqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gxprcnez.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sssggpkg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vdrsvlpr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wecdsnpb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mjishzfn.html


<!-- 参考信息 -->