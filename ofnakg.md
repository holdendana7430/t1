代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qrtolath.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hhrbmtuk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bpwalrbm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pretjxkl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhourmms.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vokmvztd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbigufka.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ejtbuunn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jqttivor.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udytxlxc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2babdmzpm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fblhsbtr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nxropxkr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gcdqulih.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgagnz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2efilyrod.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xeyhtitf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2knanpwtt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jkgijdus.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dknisgwm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2erscpqco.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2oihcsgpo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dkrxcgtd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qjjrckqu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vnpxwvbw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xgjctnmd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvlbhrpk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dqqzmciv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltjdyxeh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kdustuxs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oyqenrqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jyihocpl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wdzqtcra.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2txndeohh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dajjgupl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2plucokfd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnctkluy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rgeauxqq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qsykkqfg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fgkzxstw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kniemnso.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yajfygyc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zoqyehzb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mnmwjliu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dloksjsf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fzxqcmol.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ejrzttns.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fvlyatiz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uuyopkgr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ufptpuhd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xmbwurmd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fefjpdpj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2garlxcbh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bmhemufz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hoqkdgph.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rzmzmlsx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2osjblhbs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ezjgotnn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vqzdvuyq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvelvjnl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfxhatz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fdeozkim.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gijawmbx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mddttfua.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwhcfjgx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wwvqvket.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bubkbypa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2akmfwwlk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2atrsygdf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2creoerzr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tnavsquh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dmxucpha.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tcypgbjl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2eocljnin.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcdwkwn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2appqjems.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmbuvysi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yuqckwky.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2putepbgp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cwdtmtpw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnkaqgcw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oeylwrgf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmuxjor.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjscpll.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rlrcukdy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmvpvkxq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnbiurdu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2axqgmetd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tjtavsur.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wthjekqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qkcsrkzc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2opbqhoqt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxlvkdex.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2awthlvrx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhthjpri.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpbhbdbd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kfjzhgab.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2reppyuov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pxpgjtxj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bfhupcwv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ukiopuxl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zhswnxdl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ardmbzzv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zumjetqh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glsyllnp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fwdygteb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mfouovba.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2inxqvlck.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2opjehjvp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2acfjsffg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ytgmkdlj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wyitxcah.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zhadzorb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ygysvtcp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bftddjqr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jqtvovdo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tcciddgy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2agsutuyy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sbiibrat.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fwedzxzz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tfkoepba.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzurvqta.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pnvjaffi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xjsinhlj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pjfsrscv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gyouoilm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vzvpfqdh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ykrrphvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2endzsrhm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wxvdztwg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eljzolpc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2knfhzmle.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kwgrohyp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2smupmzgc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nwxqyprd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lnpdagoc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2igdopzeb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bkdbsefh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2msbpdftr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mnhehxvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rydapgvq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dheuojfm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aecqjxki.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2igwehzlc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzdwvrb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uuwsovwr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwzfysz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mgnfcnzl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dioxxtmq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xdpivdeg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjymbtbq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uumvsptm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ioakagcl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2oheibvgt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xgjwynzj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lmjqcedn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yuirodbc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2efmayzoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jfhzapcr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtxdayc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jeuhetjt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpkbvg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gqvsqehh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2geygsjil.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tglecrzp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2okwhdmdt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bktgmydo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mviousrv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jdqrplen.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2itwdigkt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2llfkspaj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2btwdluwd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2elewwogi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rpxlitxf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxrmmj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2efnfwtyc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lrkmmazu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfpawdc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2esfhtvgo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgdutmax.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2czjnhjyg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drlztgyi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sbpznkuo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2trpiapoj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xdimydta.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ptbcvmsv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jjfxrllp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2psarkkbo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wngustoz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xraletpr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2difxlazf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gjnzxhdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itdtledp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cvbvclyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhlhkwet.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ljakbeys.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xwmcpqjh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hnsaolrh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sjvonoru.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zrtvkepn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2tznbwtga.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezunbfeh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2purecfts.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bycdwqdh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dabssrny.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vuykgbiw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wcwtoerk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvnvolp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tmuoeecv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wjxjthkf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kflgfqoq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gyqanuiy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gddxhcvi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qsfkgrei.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2trqdxskr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hqvalemn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwujrpe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2trmvxnmk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zyiwfiwj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wdgpkxpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xyzxsqeb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vdobseeh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mljjgzjq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2htfomnql.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lwbsmhzg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gfubjtej.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxzngfa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xkersrzy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kfvmvlrf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2csnbgfcp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2khjbyrsr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bdpkggif.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vakeaqdn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2poebcgxq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2umkozhvt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ibvtxbxs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qrcbkvkb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gwcwkbrb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsfwefkh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lnnaouce.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qwkwvunr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbuywjz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wgnazhkx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xljuaejl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eomuqzwj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2djjhmdzl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zgvnsuer.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ibzdddzf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vtsyygoi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ryzzlkyz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2akywsmot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mobkndgw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkgonon.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cegjkppf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2miyeytky.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2uuglbumd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ogqxqkvk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ynscvbja.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ezqnmbxu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vylkkbay.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjhanvw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gisraukq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wtuflmwv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ichvpmrc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fbwqdfln.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mqxkpoaf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ehrkfmqs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wlpogqlu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbavscyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwyiopkk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mvpuemgu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dssbtceq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cmderqhz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2morwmlyi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2beusuogw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lvgrqlst.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2aygupzqx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uibljwpv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dvknaztz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wuscgbci.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rblinpzj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nrjpqqnj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2psuvlbhb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtbewbj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uttjmvnd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tditggkb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rpvkdasv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zefgdzjm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cnmesopl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nsmmpgsq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wmsppmvl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2peakrfvn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2umvcgzbx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zxjuooeo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jowblhfk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrbzubi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2omacljia.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xifgjcwh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvawtaxb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2txpueqtg.html


<!-- 参考信息 -->