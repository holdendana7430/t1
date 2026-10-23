代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mbvunvuw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zglsmdbk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bkxbzddh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ivvzfatu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlyioynh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ugscaqie.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcmsmciv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ckeitokl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bulgwbju.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ddojciyi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zfndktrz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rpsuitql.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ldlcsaeh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bjbjylmv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3okvonsjh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uaefvxwc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3klkzalkt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3clrjtlmu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3jagecxfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pzuhjdrc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvvlpeqp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ellwmfbk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jubcjisf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zssnalmt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tovbdran.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ouwozlcr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lpyttxsn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hqnmhquf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rxmsazog.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dhwshieg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iczxgkaj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xfgewqsb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vjjcokrl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dumvrsgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mqyqbzez.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3khnzglcn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gfmpwuqt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fdlbwxno.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3evwwhina.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mdihkunt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jxkioxke.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lyfayjxo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfxnoxl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnymyypc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zvdxaifd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqiisneq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3edcshufz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vsrafkuz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zxeatolw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dbeczcdb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxtbsjfb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yepnuzto.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xylajklp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wmcooito.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjetzhf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcvvooah.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjuwbcjh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wodexmjc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aoivwufd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xxyzpeyr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jqbthtlq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xdepgxyn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxccddkw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dhclldyu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rxcoxfbz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdupdhw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3madkkdjs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3szklvuxc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rywiljzn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sujkhqzy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dmffpzcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ltksklen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmgvau.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kcuxuhjt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wxjztuqo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xxbhrbdx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nqtahsdv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ywuabdev.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3umyuzmds.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gavbzdvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrbaswu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpuwhhvs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wyfxraop.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ulgeefwa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3urrgdwai.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fhmfkbqx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ciwfbfhi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vliwhtil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jvpbkldp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjwzvjr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rosvzbyq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exzuytmw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mjtrugrr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xwdmvfqo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwrxbit.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjrhvosa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3npncknzb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwejkula.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aqpwoiex.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yrakvfue.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbapagr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yqdpqtdn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rznxovhv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3byfoflep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkpofwqp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3hphjvadr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxaykikh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3buoodavu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ttjklrfa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ydggyjmb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lqedxigc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3umoonjoe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vfeoxxvy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mhzlnnpy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3pzpflvbs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sulmcfkt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zdsiaemw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oxrsnjqc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkmtaeji.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qhssccfc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eqhvhanf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ocgnzyhp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3utxyzqin.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3indmcosd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dqsfmkox.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3grtqhjlq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wjphtdeu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3obgtiqvw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yalgehly.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3adlbfopq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jxcnhqze.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ilamcxbu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jjzstgzc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fyymomgd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ptopctqo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ludswbkv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ubqnmwbq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zlduyqkc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3myxaqaqe.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aykiohpe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3onusplvk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rctdvprn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iakyvmsj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tpkueujs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yyzgdhmc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ukcsygzl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wbiefrnc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xgvdhucc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ybebvrrj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lijifuoo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xjjmuecr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ysgojyfn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kanmhzig.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cqsmuyol.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jahatnbg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3utkfoefc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czkjqrsw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jniykxzn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3phzwqaby.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3chytqwng.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kotghrup.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kpabmwkr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bmlodyqj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3adfwofzi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kacocyuv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ummpqzfr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dberfgpf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbogip.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ilaclmhi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kgplsmjl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gyswfmns.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3leayqjqq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3snzcmujm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uhsfberi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kdhrhoql.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3imryuaed.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bggfpojw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xkevpstc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3simhjnlc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xahjirry.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lcsplvsf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ogowsguj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adtbiotj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bqitduna.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcjybyx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ymkxyfww.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pbdstjto.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sjzdxiqg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vfuadvda.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qmbrsbci.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcdjffb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txslkzxk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wkvcarvw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3npwjuusu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3suitnhye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pvylmcmg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3dzhfuuni.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bveulmhp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkhghyun.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3armzussx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdvldfca.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vjzdbpty.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tqrcofhi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3flrasnjx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ohhgkcrv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zhchcoxh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rdmoqssj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tilnuufg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mczcskco.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sxabhymm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3upvnienx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tojgvqdo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yrpnwbqs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ehpyhsyc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qkuwshye.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jgitbxmb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbxssxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3uorzdmes.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wygasnbu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjyiwvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvxqfaz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uuepbfoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pwtxbidu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mntdyvqc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eiidynxd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pssaufmo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akdcreip.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3txyweahn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jcyfbbns.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqyxtsy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hnfkczlx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jcrypzjc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dugvrmnq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ortjhktp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xuorqkrn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fvkiukrq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrubpal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zmtuzail.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vhepqaky.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niqfhjss.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3scafoyin.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqnchgx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hhusdvvp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yjsxecea.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bkdqzndl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vgfvwlkj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3smjmjack.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wydgcrag.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lzvytqob.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ybcwbpvx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qxlehdap.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wjmfcpyh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ufpxrmny.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxlqhxmt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nehyajbj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdgvipss.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhkxnljm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dyqzhznq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gxyvscag.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3msdemojx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jbzjalbw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ommwucwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ctbbllxc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmvjdhp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3moioptkm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ghanurmt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mpctnoyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kieyijrx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3umktejlo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3khlzollr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pybxdixc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ekutztdo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3duldofib.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ymybbwho.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fgryzfgy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhgtjuzz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mlwroxgi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3omxvjbnf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vxmcgrzw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tlrjwwoy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lijwcfgz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzahxpvh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ticuieia.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljromeld.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujmspxvz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ltmozgns.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jxhywgbp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xznqhtxe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3upnpiteq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ahasjdfw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pbvdzial.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ygrzizak.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3niqgobkd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hlifaqgx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gakljhlo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zqlvrsci.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3givabvtf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3raitdcpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3derugquc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ztjmgpmf.html


<!-- 参考信息 -->