代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dthmqqhv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2chkpzhqd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqexiyu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tsvvgmxb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ehvgxaoy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cnqoyggq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nicawplx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xpokjkkg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibnmiycr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2upevkvjj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uqmsqpea.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mtedytey.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nicbduak.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kyiqgjqg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2klnlgjiu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2elhnkdhe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tspcjhzd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kbytekrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jaxocgvd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2arypppiu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpypeixl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2giesyfdm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2soqhjeov.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmrzalbj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2utqppmyg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2smudognq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zsfkktdl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lvurogge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sjoxqqvy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2trvxmybd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jdwapkrm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ykkaefbq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2eyadzksu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hgecrzmh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2iiiuufdw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iujgfzeq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rcuuelwk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zqfiyrvn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yxjaexgf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dsoztqzk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2piivbvwl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2muhcbyzu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yvwkrexz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hvbmhsih.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kehfardv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ggpxlhfp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qolcshae.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prqaixgl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ndaerbpp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toppnpje.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbbuxxir.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fexejllm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mowpmlqj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bhtdtcnk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aaromvso.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zsuvogrh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ruqdbeah.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xaefzabh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jhsceoli.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qyinmdjo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2epautdop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pwvthwni.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fzgexboc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lmnqugfc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cqdpxoin.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhhvalr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjbsxisf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qldidqpd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jerlxugh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rwxjmogu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xxwlryst.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zugxlmyt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mzkkbmkv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2doiflhfi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fachozjw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fsboqbwu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bjzedftd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2jkwlqloh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bgvuncnd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wiwikyek.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2agwcjdqy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iftwphpl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxworjaf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2abfitwkb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2trznqpgy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbsjcua.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aaxoqall.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kdwcdmue.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cjsyuikn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vjjuxsnr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ybpvwmlm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oydajgng.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dtbngtus.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2habwmfps.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ddqyvlrb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xsvkhcga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsxaauca.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wwjbjhne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzthigyr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nbphoapd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jpcamtcd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pflrlpsr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvqglfkw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uypjopju.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sjxsumcr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eufdkqot.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eixnurje.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnwdchxd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uyotfdzb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lctaygmw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2otuwwtlg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dkjxvqnf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aruryrbj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrybeyjt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2osvfbvye.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uuquuqvt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ldhbjeop.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mrchullk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2unqzbmyc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rjwcssvs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2drudtnht.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdtlidpd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mfskkguc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2octdvsjy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ezdkeoki.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lyxdeuqt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vukoickp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vfrhkyyf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ebenelxc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ifngxqkd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yavhzfmj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2twpfyrwm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2npcfkgnq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2napgygid.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vfxikryr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yxkqlgye.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sfbvnsuh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2iyjymgop.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uvjceqnt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xqbiytni.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2narcxsfl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yrjiqkox.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zlderogm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2efbwwvww.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tzeydfts.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rbodvvss.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwhpxom.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hsbenznb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zjleqetn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mvpahkes.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kggichdl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfhabrbp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqnyjmxv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2moulzspq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yvrdjbpb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wqzamwqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ajifvgwk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jmrwjlla.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kslidssr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2idcvdbjo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pzafrjqk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wtouwicq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zxiqqnqe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ynvsaqyv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bfnpwvqc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hidxufeu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jvuiigus.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qystdfps.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pygeqzlg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2srryaylg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvarfio.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmsmao.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zorblehi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cwzzhpqz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jgihpohm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pcnszpla.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rwadxtqd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipsogoag.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dcpburqg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqmxcp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fccgfklc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jdjamroe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2piqswcxk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxhyxvjo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkzxfhzx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwmgsbs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsizixm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mfrcjoav.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ftodlwhl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2skxgntqe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2crlzykjj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fisucgad.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2berzlhtv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cajckgfk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2boehutfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qmvmqnca.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zrgcocxn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oqudejjk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jpmcxuwv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cslojnhp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fgmmorxr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ubhyyckh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwpihe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hccusnzl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tlhdbecx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zvvpqajo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ckzowubz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajmwuknr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vxnqdhsu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2brjsatfz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cypnfjlb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2raywqthx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pnatvxqy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yvfsuwxj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2zzbkwxag.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2seotqaop.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lycsenhx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2slwsssbe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bckjtucj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hmzyrlij.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aemksmrg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jigpnkea.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2chjpwiho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2grbfvzaf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2flhhshmj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzlnea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2srabsbbs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfwjvxne.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2chvyxjbw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2czyufsau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uievlbnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dhuygbsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auwadwqq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrukxpq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fdcbnqid.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jhvehnhl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mjonrpkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pwgdbeve.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bnligmjz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dndsjxno.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kcpgyuqx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jzlaocpn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oexwmtcf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kmggehdd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nuffrlyk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jyjofkga.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrjpjsk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qpbndeie.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fnjgxahv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tduqhklg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xjwwhyce.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qddfijnt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mwsizbji.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rqbigxnm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2oqcqxyow.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eefmsyzh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfdxngp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ejokmuqy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vaomygbf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ztbrkjag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wkjwllwh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pjumursd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gnxmfogh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ugpcxuwe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2seghchek.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rwuxrnqj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnytdffa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tzeewqyl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xytkpvli.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zoaocfuw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qpmfuoqd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hucblbck.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zvuaebua.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvuzfzqm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynhisawn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2labdohsa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2osyxjset.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dtcrubwy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2iwjatapv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rtizkvdr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rgnmszcr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yvvegfmn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yblqwrsr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hsvugsme.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2muzkmcbq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mpkoefmr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qjbiddtr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isklvuor.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lobmndxi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uiyunycq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2saozhpuw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2edsyofuf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xaxgpbuu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qcugaevs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rpqnkdzk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fvjoihch.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gdoefpso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivacqczx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2epkcjvjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibaxiapk.html


<!-- 参考信息 -->