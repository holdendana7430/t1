代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrkzxkai.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2aofzfpox.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wntfudwo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ibecbdmu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2diwybjrg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tfpiwrxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2myljndiv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pikdnfhi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vduzrpqa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nbxuamun.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2exngjacd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qrhbzgqk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltrycijp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgpnhhkr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lnfwqsjr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2poplqwmy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kdswqmwf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dijefvyz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2foyuzrqt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vydzpkjf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dxyfxfxc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gpdxxunc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ljmzloxd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aijrrhsz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uaulzdwi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqiofqx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vvptgblq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fvltkfhf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2risjbmwh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mqzevkcq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lwnygrhz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tguexgrw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ixswzzyj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sqvhuchh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbhrtwbl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wuvfqtkn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nlpjitwh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqlzzlhd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hxqsjftv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2spqfzfwb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gzbfhcwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ddzkmcos.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2oixcncjb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hqwrqinj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmqeafxq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fqtdnkgc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uzrwreji.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2blznehlx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sqmgrhfb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxnzmtup.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nxddycne.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2frmmmjmg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tuqnewon.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qyotxffx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qwmimqxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dkglagmf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bnpyqjrg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2iyxcjbww.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yiqtwsek.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mpebbhxw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mqilhdtk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xebiwzcv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmdpuei.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2layjnaxu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rrfndqig.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gyshrizc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2iloxrujn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hylacjry.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lpthafjq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ilufodnt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jcswzrst.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhxglsxi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pvehaify.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bybjjzur.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xccijtre.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xbqkowtw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uckjxkql.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlvqodna.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdjfuhen.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nofkokgv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2suzzfuth.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bnlcgrao.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uvofsamj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lqcknbse.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oohborjq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2juxekebt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pdxocumg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rigillrf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jihwehir.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aaibxkpw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vikoymzy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xpjxaomh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lycacmbt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fmmocyhc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dazpxuvl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nigyyhjw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eoysdgdy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lhzdsssi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pkxpoypb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dwsctfcg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ewbwnems.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2behqqlpr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2owfkiysf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rrqtogkd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzghlxw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzobrv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nsyfviwy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dkkxsykz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aeipasfk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ybyrpybn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gomurcgi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqolutk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okztixqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dwkaxykg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2izgqhwsz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dczupdyl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mmvnlibn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cgaubskm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cfdaxgpp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xdxbawzc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mbqwjzyq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bbjwlwxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rfgexswp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qssslgut.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eypjsbpc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fnnequhy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tctbhaeo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nfadmhnl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2oucemdrm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ccvirojg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fblcvuao.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oxgnkjvl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fwncthan.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xjycoibn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2albhfmed.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xlliiwol.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vpnxcbiz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dtyvmvst.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gphedvsw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozsaoffs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tqqxyboz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pcnicetp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oakatram.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dmfkxlce.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vlqqthyg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2redftohd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ehjaytas.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lcclpwhw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xaiixsiw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2furygpzw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ngokyqjt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcultafj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kyogoqhv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kbdkqtsi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jcwgoquv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bnjlpyrn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2evkipyne.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2iulprbzo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2owdqgdbd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wfckvnqo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vmydspfc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ppfeuiyc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ukjuwujk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sgbrccqc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ialwphnr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2stgtwcvr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wmrhzknd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgceihdx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zbtlxocp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2batpwpwh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zkbarzje.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xjsmeeye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nixohbhj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tjgaxxnr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zwfmdrrz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awuxfwmb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfbqybc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2olufcazb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kvbkhfbo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jhlxpsrq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hbyrffzx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sxokqsfm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2avckojkn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2koskyofp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrygkc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhwioza.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjsgscw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfhqxac.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gigpajcf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uwmqvnfv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fuqlglom.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vzgtlhfr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2knjvsjun.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zzydwgwu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2orgptuab.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iltkaxcd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ebiwxway.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uyqvhykw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cdqduvvv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvfatia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtfqhhyi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ezojetbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flnuvrzh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvwyrknp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ayhteidx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfmbnlkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wvuknqxy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kwmipksb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ytqjleay.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mjbvygwf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lrjobktw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fbqfaqnd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2eilovubp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uydhvsiu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dkrntwuy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2frwcfvhp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltnvdlig.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2etvthjvk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mowpobyg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ehvurcny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2znfkrkkf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qohlbzok.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gxqgeixv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2atddzetc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2raqgqjqv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vrolpllg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnodbon.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fqwecbpy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rwhxxoey.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qlijnuwt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ivtgsetw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nlhrzktk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bredlrir.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgfeoap.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ihfnssoh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kkplvuow.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nljvhzex.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pcubcstv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gkdpmwdf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wsunarjn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pwinspnu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xvmdkldm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cdvsukbi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvlmjlyw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ksiwkekj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fjndpzma.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2eslnfvzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uszdzqch.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cswgrabv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzbxqub.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pacwyotd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txaadegr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pvkyluuw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udknyraj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sbcrfaxr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghhhmumz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2skjriqvf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cbhqqgry.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ijlllsxp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdmdcdmr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zxldbpuy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oztvrhyg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kekvlauh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tyjvchoc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wayxezja.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mazcjcfy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mazywngi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lqefnixo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jresjxjz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2syvbitbj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rlgsully.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yyckqvgb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2uiupwmna.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xvnfvbil.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cwbfqmwa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ibxylsyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kqpwjpay.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vcnbkvye.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cayiagdr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2owuhgktg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2owimcjmf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ehkwuxvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wepdnkml.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2koznmcdu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rxplvbgr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lmkamysf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kziurxaw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xqbvyvtn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgfpchz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vdggobms.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2petqcdkl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2obuyyjpl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fpijebss.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qdlwnwca.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jusiyoza.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hpbpdxlf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jfkmrmll.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qjzhalww.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lsooehnn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdrxdo.html


<!-- 参考信息 -->