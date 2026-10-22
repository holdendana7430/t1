代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2avkymgxk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ebisxetw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhnhdpx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gfynsbtu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dnnhdilh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zyfrywio.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2edfzklko.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yrciyecs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cuutkdow.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2grhxtcbp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kgnbdkbg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cbdiwgyl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yclwraxm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zkdhofcn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ezciulci.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vcfunkjs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ogtfidlv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gdnesvqk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tkxrakmx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xosgftqp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmdcawnd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbdwbtj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzgywq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yjdhvhsa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jcvgiabn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmpnclks.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2naboucyr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gonlovkv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dhkcnsws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tloijczc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qxilgzqo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sqsbdipu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wruqlsow.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zutinmxd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2verdkgsn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2aewrjkdb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mxnvefwi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uvjnzpfu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdsvont.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mvjntytu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lmganhqn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dfojxwzd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prblotlz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ravtfurx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zkidgcqm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pfsgjcss.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nxzlvwkz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ggckvzgo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyqtekkm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mowbvqxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qnukyvgp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iyscttqq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2osaqholh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mfpvcpin.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2baygeusv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2azsvbmev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nzsrpyen.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qobuwusm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyugerk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2evvjijfn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2emxvdesc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2knvoklok.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iiobxwmf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ovpitzas.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2oizarrsc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2juyncemf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zeulfycn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wprxnwvt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rbtgiqah.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xizaxsdp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcyzovdd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wufxycjh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xwacxuca.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2thuwcvje.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ndftktjm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ebpxjqxv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ioappqir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gnkslgak.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ddfjdhra.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fheaqvli.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdjyfpq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gxaqhwkw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qsinhpyv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uwccculr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdihelw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dnqlxojy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdvyrhu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ocmpoulm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dhcnzusv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhubiezj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmyywptz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mvleitkm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfzyejjg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilscpwip.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ikajxvzi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wnvsxqld.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2croyasmv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zmpgvuoc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ryhyvpqx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gmyzmcew.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tsxposqy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rdngyfeg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lxursyih.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2goqkfrtp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wwwfpezi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2oostpodi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sazagzyj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cowdmkiy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gytjtidk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gcfjreuj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqcsxlk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vqwptyyo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqjsghd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ahkumbso.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2aqoqjpsm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2oxdzguvd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uabbxciv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sepuimbm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xeocxsdd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mshbiyje.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmsepszj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbohvtbg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dpkpoirl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hyjyizld.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwakirhe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wkgwxhyy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jqdekhrh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2eedurhub.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mwivmjwp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ritlsfux.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zdynqvwq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aimuhayv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uapjlkhc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxgflqxd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jkogedgc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqqngttt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ssppinle.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2azkdigcj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lbaqretb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bzmvwvxe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uyzopqwl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jfdonizs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2eonsjabu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gsnrysoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dhmmture.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dlwfzenh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2brjfphwx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zisegzca.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zwgcbwzo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hczclorc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bckklfma.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vtaayovv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hxptddmw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lkdfahxr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zwgsdhgw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dxacztju.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tkhidurl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dengztrs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iljntsgs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuoikpmm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2scwgtpcr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kojcqajv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhdaicl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oqtdordy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjymjdil.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lqeynugv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2stphvxzf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ebvipksv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sfnfmugh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ldstkqjd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wtgommmt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pmnvopol.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2glncbdoz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qkjonxyp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2leppttmf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pvfoblzw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbgilhpj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jaillgoa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pcbczmdb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2darbwvup.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qomztafe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ewaoayuh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ijrliobz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ghlluqrb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zpkreafx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufikrjra.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ufalrtpd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sbfdpxzm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2imjdcypq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rbrofzor.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bcgqkizk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ugucszql.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ougycbzd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wopvrchf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygixowvy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uxxzyvjl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2manfdulo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udrbkefa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uhminxba.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xewhmrvr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ibobzxlm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlmuuuav.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltywwydd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2owhzxcjs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ihssfbom.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uqulxryv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vnqycdsf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uatlcdae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbhncbyd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2csjfaroq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aufqtlqv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owrxgeom.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oynrbwea.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pbuepyla.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2beqzvlqt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2errbwyii.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nenhexqg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wxeowpgr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lkkbbbcb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lmgicklk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rxmxybyv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pclfctwd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdevzzqy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2flhnrago.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ttptania.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2anqxdcdx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ytjfeyud.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qufzjymo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iavmnuzk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2igtjlaib.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zxfptwdp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aylybyhm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dxyrxble.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qopjfvar.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2axeflnbc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zxbpnxzd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dikddzue.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2whxednsb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ivqnfqsp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mzkdoxbz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2djljapyf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vpeqxvdy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxqegdkq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ijqwuhsr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cpbkhynd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cjvoslzh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oowtuxda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bflfjcuf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxmgcrh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gtxhdthb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dvllxvgq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mjyjcnju.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hskfinjv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tiaarsze.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2aiaqjhud.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tpdfsqtt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fvufnjqe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dotupawr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2temiyfnh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kafhwpew.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxewpkip.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xgblmwob.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2upriorri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghtcsrgf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jxeyjojh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2biikzhsg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qkllzbvu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dynklvik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2iimigtld.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wixpyiao.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ytncqrem.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eehamnda.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2edshavyt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qztvpcrg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pppsoxmp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mkdrudny.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yjggmmkq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cqmmvbrl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xcvirnbw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tzhhbxpb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xqywdnqk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jyxyutsc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wqalueuj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xkpdxqfw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hybkoehj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2foxduckg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lrlfmtfg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kzeimmen.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dwpxkiit.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2akpdxrzz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2redarnot.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tourzqxj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vfnimfkj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2slqfbthi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2awqbqjyl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2otecvvmm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2crcbzezm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhtiumq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dlnwsgmv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2putagnsp.html


<!-- 参考信息 -->