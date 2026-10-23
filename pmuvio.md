代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3smgmcyjd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbovlnfv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3quxlgjmj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3unxhosah.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wugkeuji.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dmgiezjr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hsvwqebu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xejfzcbi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oknhqajg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qinezqwl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3muxpsnrn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xjlxavty.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmvsddhd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdiqubqu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xtyqpfdx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eajsojkb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3riklywzb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fthqqkgm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sdwrebgi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gtgzlsba.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iydoqvyy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hcpwcjan.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rxtuadph.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cdhlypxq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3laqwnbqr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fipynqmc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ifeerisb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3apniwrxx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gybepsaw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qifelwct.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3anblqfjk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qxtbctpm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3esqbomdj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kuopcfhm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ukjjctdr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ourytydt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jaoqlqym.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xzzytkpo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nezaomqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cmfyjodn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hadyquav.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pmzixftm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3siljjwmy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3sdtdplww.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3luckvjmk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vpfskncd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jxbssjgy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ajvfnqjp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rylegomb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qufyumaz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eznqwjrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gbbkmtcx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vsxctifp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3whkeplip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3shjnvewf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3juxyrhdh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qahrzbii.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vyihqjqk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zufrnqrt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqfywmk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nbforwbs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bdyjcymh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3eerhtthf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cjocdhkz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gjgcxsuf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qagmlxhc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cbbqwkkz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ejfegedw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wgxuhsko.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sxztgjzf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lmcjdttb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3idrmzfgd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtayqotd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rgzlbqit.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aalwxvsp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yoeohczk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rszrnvpa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rmtmonij.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vidgqxtn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mscooece.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bluzygqt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ajmwsaan.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mickmohm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ybppvfxf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yrmcsqds.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3faojuvol.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dybszzrn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hfijuszu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vemugoih.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mzzhnweh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixhxvwho.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3avkneslp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3epaaqmiw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qrplyjox.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahvaljrw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qlqdzldu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hrtddnhx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jyveufgw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ykgscjwh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3waynsawb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nuyllich.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zwqkurti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edzgninm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkeuvckt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dotkxpmy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pphtmsva.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gumiobil.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3npzyknmc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cmxatnlp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3huhlmxuf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jyesrwhi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crmxbzsd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ntzclndz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ruotjxsg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbrbga.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fvzgytic.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lzmylyev.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vcptnnpx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cckcgjlv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ubuviekn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kedablpe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bpjphltg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zrgirrvi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ijpevvdw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3eqwlmalv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xexezuaq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lcrxofgn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sgsfhyeq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kgirxqek.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azqcutvb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wltheqly.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ycsnjcna.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hiutvzgi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3abhvsgnu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3avgmofwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fqvzlzgp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mhnxkien.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fksqdhps.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pftyaxyx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mwlqunry.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3irgwwmpi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jvrilfds.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kbbfidwz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qumczvsc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xhkybbrz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3agwceftn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3meafunut.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rqpsqpqs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3khxtwnta.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wggpdkym.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jigboavx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xbqfjdby.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zektfibl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyqqbco.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lienkehy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bdnruhga.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifwylhvj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lmsfxutf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkeivfiu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xruymfkv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cyihvcxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dikoyezm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3idhuklad.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dwlfbbth.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qwyuihhf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wmivpdxl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ayjngjmu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3irkjdipr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uqctknna.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3belburmb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iuceypwa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uctkrftb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulyhmfla.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wpsrelfc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vliztbly.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcfsbyie.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cpfzhbns.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cnfghvbc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pdpfbgkv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xzrxfsgm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kfilykga.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xsuirhlt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nqgtrvfu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bovhbvhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ytfpcelt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pdffnbxf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tbohgimd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjugivzm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xletuscv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3crhsbezl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnezggwm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pztjrbft.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3clhqhnrd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssrlkdhd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hiwphbhe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ayadartb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dcokzyhd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jajtysfp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nrupupcp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwjjvcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsbdqxmm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hnqjgdre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsxdplfc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjgwtxre.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tphprfnk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3eyjgaqwr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdcuqtea.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iczrvvoa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3meyxfnos.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vqdaxzlq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nellktiy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pykvepny.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3igoiehap.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xfdgtllc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vhwnudyu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pmqzddrz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrotsltt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hacupcdv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3khvxwqwf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ipcuzzrf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hlctvmkc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ecakujbo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3izxglemu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tpqjncll.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqljllj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlrwaqq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uthfvnwb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zaxhbafk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qcnfovpq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3sunbvsru.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bgyelagm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jiixdahr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lfxmrsei.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jbatdeju.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aeilrmxa.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sfwhajxj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nuzvpqvd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qcuklzkd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gyisuonh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nkvorwhe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyrcnclh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hlaatket.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ureqnckq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fyqgdbzg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bxdynqpl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tifdnfnn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cedbzxnt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3avcfcvdm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vpckzmzj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbijngat.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfjyikyq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pjefbwwh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdolnlhq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3flfcoibk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sybiqplm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmnwzdfk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3efiblztn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3uryqjdob.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uhiosvre.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dyrizxpu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3diitfcqo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkvcdyus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gkwieryl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ialodpvb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ievwetyq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3aglqpbsp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3opjxzukt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fsgvefst.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3izvucqsd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uymqpyxl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3csmpsxpo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3teusdcyx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wggwthyl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pixvglkt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qqjvvmsr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jlarfkku.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dltzosyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rmltnkbo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wjeyrulp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lprrqcii.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ekcdffqr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cnckmhsz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pnkpoqvc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhsrey.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tstuznej.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3evjhyome.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qcruorwi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wxcjeltr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rmoybyxt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prprrdib.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vuspswkf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iargfmhl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zgcumdos.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adidqxul.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wgsikbcp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3brwqmgnl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nmfsxzvf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ztgjtjjo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvntgovw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cadrvyts.html


<!-- 参考信息 -->