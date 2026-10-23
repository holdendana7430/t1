代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zsacmerk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hefcpoap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ckemwpdq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zljipgsw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gmykwtuk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ewcwektg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3utxgmnel.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3awjanybm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3grjuomcy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubomauli.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dgqnsmiz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3evfadypd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3veqvberl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3knjrgdum.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qhqmyyxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ajukuhlq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ftbenjjy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iequsasa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3guarfbnp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mpnxvzru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kmaoalal.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3waevmesh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wgkdrlpv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfffvueh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3avvrrlwf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lqhacgab.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jgitrhrv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vosghudq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xqcgjjlp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3naaplpba.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fdphxkas.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3meldkvfp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rilqnrsp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsoginth.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzgxdtdz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3sjwqbfun.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3yzfmvhcc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xmslicpz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lemjquui.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eknmsotx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3twoajmcw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvnxxpi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hlqatkar.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kniikqmd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3witdxvrh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3juyrvhio.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ptvmsnlb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjeikbl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpluyxu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ubphgcsx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyclcdld.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fqaminos.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hnoilnnn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nhdlipmx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zlllwtdx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrumwvya.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvussoic.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3obzeonhr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jqltrswc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kxsfvpmp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3btuvsliy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nypbtort.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yjvrxsof.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rjjlmxfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3psxakjoj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ffxogjhv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cnybvigk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwgimub.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3oammxqtq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kpaenykr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sqhdgfqt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fgzskqri.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ugarjgfs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kdciodws.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uzkmuuqx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dzqygscb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3robwdekk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lxpfsjbp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sqsrsmcm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ahkcfzou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jywhkpdb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gzcaflcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayzzrlke.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqztxaov.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rppvvzcw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjehsizx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxpgzlhb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gbvwskaq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3upxlzkda.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ydldguzk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kyauetjr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3udohomhl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhsfnr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hfkhjwia.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqysrmr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iieejqbg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mfymfsko.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjcdfkaf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hmxpnbay.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xlrfjopv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cztgacwd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3anvuytmu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lysgjiov.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gememhak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mculwixw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nhlirrsi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vjqcaedq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xnmuzacn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylbbzkkx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3grbufeoq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gtqzqqpl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ezxjljmb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qwspslzh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mjacezei.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3osqepmxg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qydrzvnt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nqsjshkx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ffpyfdic.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hrxgxroo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vferchaw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zflchlle.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fovckeip.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dznnkrxf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jdjflqpj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ycaxhfmt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pioclfas.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ebbpxulc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zwcsewdi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qkjubxzv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bcehtdkp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hcycmqjn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mogvxlcp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lavlrjql.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ppuqlouy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hoibwyru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3owwvlxzu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nifkwljj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pqndhvbq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dlcozsqh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dbskftqg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnvdome.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3opjezuaq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bqcvvczs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3jskccyef.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xavoczfy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gtulldfm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ojehhmqq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rfqstcyw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3axibmgwq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mexyyeld.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qlismigr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3akfqapxd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nkmazmgz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oswabxwp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bluhbdxe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3clpekgnz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ccdzcwxc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sdcoejqu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nrkbkgck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3adlieapq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhnoukgz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ijrifanw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wzgktcsy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dnrzjjhh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3osmmwoqk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tfgtvnjm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iobmzexd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rfdvambx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vymtggpf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmbgpjx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yspegwpx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyyogvv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3gakcmdeq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxlyblbd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oiupxekj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uucdazla.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3phesutfy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pvoabsoa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pxvbsumy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ijescxhw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wotoucpq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fiezulwj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mofnlzwd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kmppnwcn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3htqgumbx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gmnfoljm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wmorskkv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vzwcvfhd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhaiyos.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3omrnvmhf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gozbldcj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvrxvgvw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hvmbrvif.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ggwavhcv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3buydocaz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvzyaort.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ehkiwtwv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmpswzel.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yjprflfk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pxfeyiuj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dbjlelbs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rnmlmaxo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fayuavzd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xrgycurb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vqmkfduh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kfasksjl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vsxrwyyg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3plisnayk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cwelyolw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xwjjekme.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btieqqkt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3abamjjch.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txkaeusq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnoascvu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xfgurklv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ifbudxui.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhymfrzz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asgjibim.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jjqlslbs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nphkxxro.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3chxgkign.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qhmvfgxa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3apkbnxye.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3krzapoud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ydtpxlce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3enxhgiun.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qrnbmcld.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gjntchhd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3edottsma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kbbquudc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rybwfoxx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ycxexaxd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ztdcoaca.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vdncgyjk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yfzyfmfg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rpnxvkev.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3maumcstp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gpameurd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zzazzmom.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xytqzqnv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vqldbanx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wdsbhigc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fgfvpsug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zfcdwfzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3owsnxcak.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qjhikcok.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vvlggvgj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlkxlanx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvqilbl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jdsouqlv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3thyhjkyf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rzfxqpqo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qgrzyluf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ovyizcax.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gwfmctkr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3axqsggko.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yygvmadk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auqgfzdh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fdaluxff.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkoazjtf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3niiglvnj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jymvkltq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odwrlwbc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cjwiivxq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ctfjtrme.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fwsanaqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qemahtxq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dcvcvfkk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qeauaaxo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gqqqfxyq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fyhanejy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wifhnust.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3agfwtmbj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3buzpfpbh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tvbojqun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gdlfgfnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mnlkwyon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3utlqorya.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gbrcmwpl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zuxsnybw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xbbqdmqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmsbljay.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bmsaukmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cusewbau.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jroownlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ficdcebe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qcnhhbqb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wnuwegop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rohphinq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bjtlmhtk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3abzykqzy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcthdwus.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vwomurlu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwchefuz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvftpxom.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uudiotih.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffvbqljy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqydqy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhngjmt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzscfyl.html


<!-- 参考信息 -->