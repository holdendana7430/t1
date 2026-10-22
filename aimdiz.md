代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qdzeiuau.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rrymwuuu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jrhcqbly.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iavopzbs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aogceowj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qidoovbj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2biltxbfc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zcmjsexi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pooobfgr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2euujybdg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zkuieszp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2imbvasfi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2alnezmjv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aizvvjek.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ntadnhwz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bpitliey.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2teuytcsm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhqysb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lpdtcyuz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fgdosano.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lppqlyci.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpxqvebd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2spxxmyel.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rxrnomci.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rgnyhftq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2baumdrtd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrhkxuyr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oqgrcjwb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yglsskgm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2thrjdoow.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vhvzetqa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eirftjyl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zytjwqmy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nxotabfj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2feykvasu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2yzjfkjkg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uoyhrtft.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fazeheld.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpvneocr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jeshmkvt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qumzulfw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dolmrabj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vnuuucsp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rmdsspos.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmovisyu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wojxqhcv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vyzkclfz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2liakneps.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qojqilti.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pzpfhvti.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xokympwh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2btwiivdx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uxqmqyka.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sratsopd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pbnvreiu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmtgpzh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xejcnjap.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2joqcmhjo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uscbpjdt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tllkrdak.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uviytbuo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgnayoz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2dmauanrf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xvrjptbi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qqtlreyg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jiwauqfi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2akbefsyf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2sugdwslz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wngjpeuj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2grdqrgrt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2njcgvsnf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ieacvhvz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gcaqzeqs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihbkncex.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2glkvujdk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2evoeowjm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mcixjcmk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vrfouufi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hxrqdvrg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bauucegs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kwbhelsa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mrpfvjew.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ckaqhckp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vhnbrcef.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fnruiasv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fyvydpfh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czadioau.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jktbfrbc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwehfw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2njdeakka.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wmcxvmrt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gozelqcx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkzdcial.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xtlldvyd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvkqhcsq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ymrrcnox.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2teuvunco.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2baaanxtg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qakhbjvr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mqbyvthf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kbzgnuee.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jwptwnzj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mreoxxen.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ifeqyuis.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qakrffxh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bbascikq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwkbzot.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsnbgxne.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rajmttqe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wllnywey.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2uyxkahfz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zewwacic.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jehkdnjt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mbojdztx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2iydajehq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zuprogch.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nfcamclk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rcsvnmdr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cmijdklr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zltkcsli.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkfrekjw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ydpmxofw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hpwswxfu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gqlyydmf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2slxuqdqp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zrqhcexz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2exvejetf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qmhqnujb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zvbvwwof.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywxpqtft.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ckaamsdw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2akocyvft.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nicqlvjt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mckbpzsd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wcmudpgv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bjjndvfz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2spbhnqrs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2iydnjkea.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2kmhsouxa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zmrcahbs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lxfywcoa.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wrfjzxcn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajsjhbyl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eiwmjedb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jinhaneh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wolqieus.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2anwmgcui.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rjhyygvc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fonjiepd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vatggqbo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rxaxegxr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2agsdhajd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2oktucqve.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hdazumjd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vuiqkflm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zskadmee.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2edpjixln.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qadzkimt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwjyacu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2squhcdlq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdznxjnr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lfyycajg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2okavwvug.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ukyjlgth.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bgmsguin.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzfxpff.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2seycscpd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xvmvuyjn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rmnvpzki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2uewrodyo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkdlsiqp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwapzgcs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xewfammy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2berpkkob.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2umvupzbw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ikoxsezo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tjspkeqw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fmyprcvl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gmojsorl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpxwhhnj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sitdhzyi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yisqyffh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dimjebke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2exfwjivc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tdllzrou.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2keeytkgi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vijsljhe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bdvpwfqj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2loiyiqsj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fmsxhqzi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gdohoxms.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2okzzqmcj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zqfffrhw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sfvkhdci.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qsueypfe.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2occtrvrw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ayrksztx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irndeach.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jactsvqh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eenyrspg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jknuflam.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2kprupmvg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvllejyl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2odlvcwia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roinoxgy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2sajigpuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jywknixp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nwlivuuu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gtrrcmtd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2suqnuehv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hfcymvuo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2htiyaluv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2medkkmpp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ffbvavay.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zsgjnnaa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wtsmnidh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jtwrheme.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qnwpxyww.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iepyijxx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqntzted.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sbfeskxf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfylupbw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qjaalmyt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vekvdyfr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qondypdr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2coifmdzi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mjedopyh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2grbufown.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nohexkch.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hokyvjxc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hladqfye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qyedhqde.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zegnazuh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnxqyul.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2drgxqgty.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2awaykqkq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mucrvvtr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cutcilpj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zwszywwr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxheoety.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xykkjhlm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rokubahu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hevdfvlm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pnsdkgyn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqbtxddu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2khocougg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kbbfdmsx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rcvbkmgx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yqppgkcw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ossmfneh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2khluvuml.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qqdqlwse.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tdrcxccq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vlyixsgd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vpclrpia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ymnlxndw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ghuppcgy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tlqglqac.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aybhmgjj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yejoetms.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kaypsype.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ghxldwjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rxjzpvbl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mzsxbpnp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzssgtq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ehrddqkf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bttitxqg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zbznytau.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2koqmtnyt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yhspzjjl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qecfjsov.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pggomaod.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wcvvblqs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sjnqtpuk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mcgxttvc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2khirmrxl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2oxvwsfvr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qolmtivh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xyprewkr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mbowtusr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2otaarcxs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbyjwnyd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wniqgsgv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fsgqlpkg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jhjwqjlc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wldqsxtw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqkacnkd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sjxgmlej.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ybdamrho.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dtecphzb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uvvrvmqo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tptapeer.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wpiydkps.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjgahwx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ejiakzgx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvgiyaae.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kyqurzvl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gtdcfcle.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2aiggdssp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pjnqmtqa.html


<!-- 参考信息 -->