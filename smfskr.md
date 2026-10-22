代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2eqekbjvh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tvzyxnwv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tquhelmj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ozaexnxa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kedtjusc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vigzggut.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zkgvspaz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxthdtst.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ueexlaln.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2znkcpffz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ssjxpvuo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2suhquisr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ilnespur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vfjrbuhr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nrmngaxa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jvcncnss.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbhnqibo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvnqpcrd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vkryvmym.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kvwszjec.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ofrxpcrg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2podrricb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eghglzmv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jaxrtxsg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rygymqgk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sabjbrxy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yyvqqbbp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjlinvxy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tdbmwaln.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gtdzjgvi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yjasrgrf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wsxufxed.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhpjkosb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ginwucyl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uplgmymi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wynyegsx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oijmsuhd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wlbgxhut.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rswsqzoe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dnzpmtzn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfhcwzf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ygdbwryo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gekoonui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hhkfkqas.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gwwabolu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2apekktol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2sqeewfqa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2bszglxqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bktgvzvu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mivqxczi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hfuwbwld.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ztggrzwl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwougf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iaexycsb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vfbelfan.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kijnrxij.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ajeoulkz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2awmiizro.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2krxackpk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ffljmdwo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kczipmwt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nkafehso.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2syecnick.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nyqafifq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gihbkgtq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qruejfyj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tghjicyq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hcndzxuk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tphglgew.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zjjuyafc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ytzszozl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nptxdabg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyekpelx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qeyrziyx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2swqysnga.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lrtfooel.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfgzzoi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2friyjzqu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qwvnvxdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rxpmsrlg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zoewkihz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfijufaq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2auscduzs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jreepiok.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2smqmomdz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wvndhkns.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gjsbtlmn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fxjpfpsh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pxsnvhek.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nclajtoh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ikixfjvk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eomdtlye.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ozwslybs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qzqsxxyv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jahmwere.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2svmaxxwt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ygqfzdbx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xswkdamz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xaqdntvi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ynutfhyo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2abmwmegb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2niduufig.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hfflpfil.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jsdfiims.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qijyrpba.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vxwzkvmz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2psscjoeb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2busztvpu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2apqtkvnn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wxhmvzys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qryavemd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hfmgfoay.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dsgabojw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2naqtczhx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vjijnvgg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqpfbhkz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nphujvna.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qigzilmp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blyhqvmo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2delpvfgp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2htdvhbfu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wtcfxpjh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vmclfhcs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2obqdoiyp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fivfixfx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2handrlad.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gozhgxyq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ztxoejwo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxprna.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pqnjmwov.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ehhbewrz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btuzjvpx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2revaseir.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfqlvvz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2svfjdtbr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2crhiwboa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbyydco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wjhewswq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gqnkzyfy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zsvgojgw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2npqxhrek.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xokfwohi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjzzdrfv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twzfxabb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uunsvhgs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2byfovmuy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2whelfkxb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xkeusyui.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tycyxpyn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wmlvpuks.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2horfbots.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2euadctfx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2txiporvc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xcdelpqs.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qsfkavir.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeykitiw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ppfnaczc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yhfyztqt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2paeufgik.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ccaetyiw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bnluecwq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2sowookjj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dosyrtnw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2pylvjzcp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vloleziq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqjmsid.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kdpqdiwi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tpukneqe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kqvbggfa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfzweq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uhxvtzwo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dpkaphyx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qcohikic.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lyrckism.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqcxbyxn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mstmydnu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qksmperp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mdzlyttu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jshbvtre.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zrpghith.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocwhnkdb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qpexanss.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hsgatagf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iwgpmwky.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bkjvdajg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gagysvoi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ncmkxote.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2znrnftpr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2atizrsrm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xcxvysic.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2eyrvyczp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmmkbry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lmzymatd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ueuxsetz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rrtlbanj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2durhxacn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2isguyzfk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pzvlqazf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aeybijcz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cbzeciwe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mglhriiv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dkwibgxp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2atpuupyq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vrwrxwty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcqatoaw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eevnuujq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwdzpyvg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvywglbz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xzeeztap.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmtwzouv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hytrqexm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ieegqrsc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ptwenybs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2shjpkbmf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2odkqcqca.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uigucbrh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hjdnfibv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xhufynkv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fxzcgdly.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2auijalas.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmrcybv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pixfnocn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xsspccdu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jhsxlyzj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tyqhyjtb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bolewcru.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2amdtnkty.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uggcghyc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvduybap.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nedjqxzi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lmlrxqdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2retpvmke.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lbszwkxn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfvdewk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ifdoeeln.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dgbnsbjk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2urkgtszd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdwnslg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sklhikfu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uyfoqyan.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2tpbzhedx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mkrpyime.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jsqgiate.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mvsvcrbo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ucfmosyx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2heddukmx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntsxdrif.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dpibfhmi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qlkvzkso.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lnvfmnrj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xelpetyu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2njxjzwkm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2paoliysw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tkqssmxt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwddvyen.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lgzrgvag.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozshvtyv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pyankxtt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dqsllwqp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ptowesxd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uakbayxz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2llmociny.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qhlzdftv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzeisscg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2aszeljhz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yrdhzuks.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xomcbkxn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pftpahhw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kqzserky.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zrrjzhxc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xfkdtoos.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mnttomgf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2khzxcynv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwhvvgkb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2anenohgk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gmoiavnp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fwfzkbxm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tbcvqbyz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ezujvpun.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lnrsfnik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2juuhqkaq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yrpolbgh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpvuyzfc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nfsofmbg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tekmaoey.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xokvhkkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ucfenowp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2osaehucz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2poomfsle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ujjutcxw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qsbznwcl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wkiksxva.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lvnzdazg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uzhiitgj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2htgbaksm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jtxyorym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fnfchcvl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ynzrhphr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jtvzlklg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jjcymcsj.html


<!-- 参考信息 -->