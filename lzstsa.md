代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zemlzbcg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2roucgcdl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lxdycfmq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rpyrypns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fzvbxkbe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pamiqdwz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jxohnyyt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dixqgoiq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsyeowz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lxhtmkuk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ovqhjnjh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nzyepnhq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hiimpptp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fhtzexde.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hcxozunq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xumoprcm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2deqlrqin.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rjjopcxb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smidsmha.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sdaiyssj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpluztux.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmljkuvy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tilqahcc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lsydpald.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2hjdauuuc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bogmbfgp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hxmmfosr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gppnkdmq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ggywoeqv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ojpljiqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sjqdhzeo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tanrnuhw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jmvgnyih.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nrlermqq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mfjzydrh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rkpannpr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2llkzlnxo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qfnvyuih.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xvpmxead.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2awtzreba.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hcxsybvd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jjxcvwvi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yljfqyfg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vtwtiamv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbadtwde.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oearbssc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xscobuqj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vrgilwgu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hogebsxa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xptzqtsf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uospywzs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fwqsdxgw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2huhmroem.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2izezbmxn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vcjpesze.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nbevnmwv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usguvooo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mwihfmib.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dpifppum.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yhqypxuu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ithvrrhn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tlbwnahm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wwpxugfz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2btdmegzh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wvgswgza.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2orrbfhyp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwuvtnar.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2drgibtzq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pxvkmnra.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tbvhuptf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xubkszlw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzphiixx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kxvwyvsv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2psthddub.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2cyaqxvlg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymkgvtxi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2botknfcx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wcmcazft.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ogngqpkn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eynnasji.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rfeqraby.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eazxdbnz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2adwvqeki.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bacuxxkd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lteximqi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ciomkplg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2klxwihup.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rjshczzl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cyoqzoph.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhoawba.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jehfsqgk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2anbuwott.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wzmqfnda.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dhdgmjdt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jhhhabia.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pgpadsud.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jnwkqvfc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dbmeufvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cgffornb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jaxuedqm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nayqxzyi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vjhfsrgc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2otcasrqv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2skdjpokv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2omqdfiho.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hpbxsdbg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ajxwffik.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lbwcyfcg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtixfsnh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cgqiibwk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2itmrvpiz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcpsxlry.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nkrslout.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gzcddkeb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zskvcwhx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lzhoonlu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2owkjtlem.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2njaupryv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mujrafqj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csmladsv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yuavktrw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gxpyprmm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dxgizsvq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2umfuqace.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obsmxfhc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rhtnlxaa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pxxorkur.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dfhtatlo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2klfmlosr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gvipwphb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2evprnmmb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rhibyjhh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2scfivcwj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgooyljt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bhztqauv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aecfgrya.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pmbbotfo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hibdlree.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xxcakcnm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lgheqzev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xwiuudom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rfafphac.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zcfgygti.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2quldwtpl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mriyqjjb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bnucconk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpeytpth.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xwyqeqbn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tezrkqtk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ikguchhb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mivnxbsd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2otocljux.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fqdzcmlm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uvbiqjub.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cbznqkze.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cagqbrzp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2eqfdevqt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2slrpbitg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jonfguxv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsdxvip.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwencsx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsltxriw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hglxftnx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2aspkwlfl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkivpdvc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2obkmzihv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2scldjknl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2srvrkrwe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gybzcegl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2daofnxvp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vpoguynw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqmzybtu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mtqmwmdj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkijlltx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qkelvatz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gaanlqct.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvkoqmft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yntdzgku.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lmcpupcj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tppskaat.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gohohtzq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vsphntfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2agnthjcc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2goywhpve.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yravjbhw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2znrovfwx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rtrvwelb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ckkvqoju.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tpwegejg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dgkcsoej.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vmuoniai.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ookmaxvw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vwxwatyz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsytgdzz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2csgtfyrx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcrysvb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sknwwglg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bpjjdlky.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2scaqztnv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2sbqvmvmd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cykezajb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gktmfegu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tpqbvifn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sgvlwkmu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bkbvwkcf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wxlcvdgo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2duwrndyc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bvjieezz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyqmvsgb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2igjmqzjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwvpehip.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xhjngthp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2axrpsbao.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zglmawii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jjhywtlv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2glyihjzz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2agrordhr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2znogqnte.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yylzqdre.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dbcahunn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2athflmgz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qhsjytar.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2txwcfmhj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dukwzubx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gcfmbmga.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjajxpq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqmxgqi.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ngtqbbix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nyicqbyp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tplwiwmm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uwacchht.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oareuyzv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oyurrlzy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dsqahnln.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmgglxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rfmfhysj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eklxsivv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjbqolkn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2szkbvcia.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhnqxold.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jdlpqkok.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yhmfzzfb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wwxkkyld.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbdzuif.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pqbsyvhr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rhffwcbd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ewhhozbt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fzfnvhok.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ortcinad.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kjqeypul.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hsdxdsuj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2reduigol.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yvzktbrw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qmstcqvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ujakxffs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gfylvghe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mchfcmwa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uquplial.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgkzawvk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2szzuilja.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qrexblmd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xgdtxitz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sfmpnpsm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xtpcrwhz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jvohnrku.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xuljkkqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sckebxpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vlqulvjr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqbsvce.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wpjamrqb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rkrjnrds.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wtmkxrqf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iisijnzs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jfclzdeu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fvlmwwip.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xfoepykr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xghiapgd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nlrgyzmb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2munqsvvy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xilvjmcl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xlidjgtu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zindraup.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2owppkdjs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cytuvivc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjhpknsu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lfipjlzw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cnpcrbzq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zprstdsa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rkeedrwz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lalqixje.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ujvebrag.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkkkvxwc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2avnkyoxh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ahbfnwng.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fqunoxyi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ppduqhoa.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2swqmviom.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tadjqddh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zxnqwvdw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jddruymz.html


<!-- 参考信息 -->