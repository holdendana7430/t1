代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kjrfzuqw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zbzjgmjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ibglankl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlmbfxx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jmurynth.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ohvidetm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cyzlgdko.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mwtgvtyn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ycsbczdn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mxyurkzu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhsrahqv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zllhyags.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2worflzju.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hgrzfvxw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2keqllqvq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2icfddqht.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hylvytrt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bffdbptq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hocpcklz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jjlvsykw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vxxxonri.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kflydfgy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2efyflxqn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qomenglq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ombvczov.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2grupigfu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2thmbyvfo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ocevafnc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qgunbnok.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sdntbpar.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2synjtqxe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xtfrrbtz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bhemvgpx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2givrfwip.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yauuauvb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fljszoni.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xloouypn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2inqrysdv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2crqsjees.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qjrjltjt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rktbxant.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfdgqbag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ojjqeenf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vhqyardq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtuaerd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hxaxdqbw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xhjohucx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jexatpag.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhsgvwjs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bmmxqbae.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2romvdbne.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tznspuui.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aecqnspi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uftegdxl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2syaigxdt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ortxphrm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hsuuyanh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zgfibcef.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gymyiehx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uphzrdhx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tvxcypxc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wjawqueq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgduuwsa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dvrnrypz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dgkoryvb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mjrywozb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxyrqtm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2viugzhvt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vqhzteep.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vgmeksam.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ebderbss.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2trilecxk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmklohot.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yaajhakx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fmhswpbd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khguzbni.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fkrnjkss.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2khtwqtfv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cpnxwwlq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vscoggdu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vryzsjmn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2evkghzeq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfeyjnig.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2raqedide.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rnrghrzg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2viacaike.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jserwnih.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vxiyropv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sykaqhct.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cllcobdj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nzzinwfu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sntujyfo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmvpzvny.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nxhesglb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2coageuyi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uiurzyzw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kdphdsmu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jciyhytr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcfoinro.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nfblnpuh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zoqizckp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zelragbd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2erofwnae.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uxyrsisf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xoawxotl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sbpgsjbd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hualahyd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgitcm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ufyrtoaw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypuszvxb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gbmkfxse.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2odzsjego.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2chqbsvwi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ikuvmzgs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fwpvrghh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mpynkmwb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pislchqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwyeofeq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uspucxdt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtpfgfj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoroykz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2keegibse.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ymsysosm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2snckbnfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wblqntmp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2etxppbkr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2eozjzigi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rktfwqrr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vuocyggv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2huajdxvm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mqwrhfyn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xngqjhgf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fgprywna.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dbkcnjsp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fpzdxbsl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sheitvfr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ujmucolx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ugkyhdyk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2irfdhnax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wdowfgxv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rokmxadc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dyezpoin.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2twfmqxpp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2aoatukhx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mxiudtim.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zplmxios.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oyklipla.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bqniwtka.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gbpxfwqa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2byxnfgmo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jfhacmjx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xmclrvna.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aithijoj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yajeutua.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cxbgztfi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zivehtnb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdxznoqu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yewkpyqa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rtbqqadd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vhigvppe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmmehyy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fykepxuh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2esozvzhu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gnkyfwiw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2spnzqqpl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rvaxyyzc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xidovjsg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zzmnyxbl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mujpozlp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2valkddxw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mjxzltka.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzqdkjyv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phirjclh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cghsmfmz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jnmjevff.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2owdexkis.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgezsibu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2innnpfqf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uplqestd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oslfjepv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nitegkuy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2chpebucq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rempgzod.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zwnyrvsf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2snstqixm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bzihsmxm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ikusjerc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2brvddimm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tltadelg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxknybrr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xkvequkb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shzbybqz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dqhrokbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wxqsuysc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cxichhdw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpyzmekf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgacfhoz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iawdirxa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kkdwplqa.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2suowaydf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgkykws.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bcqdbsvu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vbrcekfm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2udomwcsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sooknnic.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhwkslai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btryelqv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ucvkpcfj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ytoxedlz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gximirap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lkhkuhlg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mzvhpdjr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2enngteuq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlkkcqpa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxpdoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ihestanw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zejvzfoz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pwuwfpgz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tlrgjaxc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2irswmaep.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfvglxlq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgockjru.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpcyvmm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tnoihqja.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vuwyepjg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dejarnwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vtyzlpve.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hssbmjzg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2usptjlsx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vxkjumkv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kfupqyum.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mlfatbwk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rkdhqfuf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2omrlktzj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sdfkfqzd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jyqjnaut.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2txiousaj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2oowlyrlo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gtvradoz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2keyvxpso.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmdspdd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2goulqkhu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kgbunhcw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bpsysepx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2flnmbqsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jliimdof.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kcfpigzg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dnukkckc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdvozkgw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jvbrnhyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qlhoqdai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eupxorfp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uhsytwrr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wtbqdqce.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qonwechz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wzxyofgh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dmufrzox.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2brcqbkbi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqhzekp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sghnmiri.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nntofkfv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dyzrfrpa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sxwwymis.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwmaswci.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2flbdauct.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vbxxlyag.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2oxrdoqyf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2npeugwrz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vxghzwlo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qttzzvju.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dgqlnysz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2melgbzog.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hgodkscu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ndptaddp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mgcgqdrp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cxwbhiww.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2agmkutux.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qygbgjmu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qqlgrpno.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2odgbahye.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2adkrobub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2axcevwxr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2adjlwryj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbgqixd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xclkgpci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2akqopxpg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ltzbclxx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kxdgjues.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tusukimb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fvrdcync.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mgcqsjzi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tjacntdy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxlgtq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kvxvqpjc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ktzkxsye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iwlambrn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kmsfpwvg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jrmpiick.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ryyjyxxl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqgpmcfe.html


<!-- 参考信息 -->