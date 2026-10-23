代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wpufqmmz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3axggrpzr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lmqwsinh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqfhrlav.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3faiieodo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzkusmsa.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmxkufnv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nvcakxgr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbrwlcw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mloqhqxv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rytajjyj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntyzpdgn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3whysspxk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3csauopwa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nwyaajoy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qaczunkl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3otfwmzaq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mcsmznni.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nlecicrq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iisfbfon.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3egqnafri.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xicbfyhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jacltctu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3umsujwhm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uwfuyyos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jjhiyfrr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ttzdkwvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vrddkkwv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vascbytc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jdixfqeu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqkezww.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyftwstg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ftnrwvfg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qiehtmad.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qluyqepe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3doxfhltv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fmpgyfwx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3eijsondk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mdwzmfkw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wdektnif.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jvckryzx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zlzjjdnl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnaixtcr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kvtravjn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cgsejjwy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjshtvpb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3axgbqcqn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nbdrgdbp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kazkbzyu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3soayvmul.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3biwrxerg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ejlzapjb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kobbvgvm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3sknqdllx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mxzrgvxf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xlcafyhn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ronkokzo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jkchjbat.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hovcoiuk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sgmkcioa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iikxuoyp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rwpuihau.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xvqacjfx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vvspzlxf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfrnvuu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ftmxkcvp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xqpkfgnf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhqnfrcz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zcpdggmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmyajlnb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3akeuaxwu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3gegzycqs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qamwcktv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vgcjcine.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pvoxvbqr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gzkkmfbm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zsvnrelg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgfyhyq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3plsxxgmk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msmjtnpz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3npupuhdu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkopxtjz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhosuqhk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsgwgkqc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zhzgfich.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bqlvescv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3igwyzptr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lsytisoq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tobmlpit.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xdeewrxi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wnqimzjp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ykdqanji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpktczqg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tckwrsxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhfeeqij.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3twdeiwls.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fvwugvvw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kkgenzld.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gkarqmeq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xytncmoo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhneecze.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lvcbjyaf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3atkssxyn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lyhudbzl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pwcbdsfl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ouaakdjk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3afefvenh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dbvdyfsi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yatnqnkz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhnantt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqstvdl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lpykwcvp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dczjntdl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3apnjpdxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oukhwerm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dkljmndw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3phqryplk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uiqpkooy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gvvppben.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hdmkwkkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uthgfplv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsylqind.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ywszkymc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qxzjcejx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oosyzczh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fuciqrho.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dyesqbva.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qxneawua.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hvorlpvy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mbypavoz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3stwyewmz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zxpdtntt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ymdufllk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xarjnxlk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3suefqkeq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzbrmxgg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbwqetzs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ledthibt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nkwkrzdl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nllfkjts.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3glpzgajd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uxolitln.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tladerip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hddndrkq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tvmhcogn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3acuamopz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wjfuegrr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wgjhoshk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ffalhkgq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xqehyvoc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iwmordwa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ecwtfkqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uhufjrzx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mjrojftf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ahdvojoz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ejfkateu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3unftykcg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fpsyjjiw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qqkwuijb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3quvuxkyk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ryhfmrgy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qchzspud.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rddnnaau.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjghdrs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3sxfbzkvz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwousbym.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uvyuzwzb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gpfvwzbg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfojcsa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3myerwkyr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tbnifvit.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hbircctm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lmtjqewv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bplghhdl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wwvnnuyz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgcamysz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gehwbnhs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gavldsfc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ktzgpfqh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gjxqnwue.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhipkse.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bemecczf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jiebwtwm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lshwknhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3olbkbgcp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3srgemfss.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3atppufqt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pyuagcau.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3alkufkdh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rkscyxkd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rmcaivhl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lhyavbve.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xssevpkn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uaavbbgi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3udzgnogy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lfhnhrzv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uitcrbvp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ornswrkz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xwhzimwd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3orunvjmb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kbsellqq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xptseieg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rbdopnig.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cnxwybfe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ykqdurme.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfsegxsl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qzsbbrmr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwyjeamg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ariyfdar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tcjdxkef.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nuoplwvq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwbpcll.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wetgeodi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3uhgjurfl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jpbjgyhq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3isinokhi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dklarqfq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3atbixywn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3udefvifo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rhqpkvwq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3snyqayqt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mylvqbrh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jhpxrcoe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykbutiik.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcmbfkt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ocabswrw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fchgcppw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqaqzqgm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vkcodldj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dxzwqbrk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tzjosfls.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wrbitiog.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tchtubka.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pzrnwjae.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zskjdtcp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hoddszci.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3yoblyjni.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bkwlpdna.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wampjyiw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mfstwvyb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fmjgqdrv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dubazeaq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nlzusmon.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxivuxjr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xvvociqb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3skzikbfl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3skzzmjcf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dcexwcbs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vjkmlqkh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gemcccmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tsqwgpdm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xiryynwt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dqymxgor.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lddisevc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cfyzszfe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffpfxofh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tboqxkjy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zwglcitb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jhtxxfoj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pywaldrs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fzdfvfzt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mjtsaahk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3amucxjqr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3biqrcxry.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nmdyyyzn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fmtqmsiq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hdnbbyoj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pegwfuih.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3htjvfxlx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvrrtysu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3twqumwrk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ctzrafyi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqdtglnp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3eavvbvsh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wlqlkzbz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xnunmube.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3iykjbgbo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yrajqtxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fpgggodl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pdvddinl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oqlhdmbg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gvhodlai.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3onxmiqip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ctuazsvt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqjzltfv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jetfswlb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pnmpqrre.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dvgbcajs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hrirpfsy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rslkhphc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fjexwkgo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3blsncofn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jnpfzyua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffazhrzk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xkmsjzsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvekphrf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3msbqtzfq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jumhbhgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3seqobahf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qodcrvby.html


<!-- 参考信息 -->