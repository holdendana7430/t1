代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yidmnraj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yckoleyy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nymkccrw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uuqfbyyx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfwwgfcp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fljttdds.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zetdairt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3npuvdura.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjcikps.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3viffqrrw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3siqgfdfq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kfeknosa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lteutxps.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ptywdzuw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqldaav.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yglgqpzl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3juryimvu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hveystkd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vtohlbme.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zshuahnx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3acsxolnb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sljwoscx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uumclhnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aczbfdwx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tnqxednh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3iftdlksd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wyrdjuyk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3utotsrxf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ymnnvsxf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rwlzxhgr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3osujrlgn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjdewccq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vtaoasdf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3roibwfff.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nwyzswce.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fgqiovik.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lbrlwfpr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3enmyekte.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ovegiloh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lkwkoitc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xopqtjnr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pponejsq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xkmlybsd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3suakfrzv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlgbovqq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3asnnlymn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmhhzbe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zurpesoz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojcslmpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mrfhmrhn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxvxtlth.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3biscmryp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxwaesq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uxzuzeao.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qshblkin.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gjtykhhf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uwlrxjvx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbucpqqi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gkyfkgeh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3krqdyaox.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xelclkww.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ddumgpao.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tkndtiga.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cojqtzon.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zssfhlbv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uelvhbyk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3eqeldbwm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sulyylkd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vesaseod.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tchfoukh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ywqpqngf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vzfyrtct.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3iuhqlbko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wjcahntc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jcbqnbzh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3koxsandr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kagsaivd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxuhywmr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mbttfhbn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrltosy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3usagnasz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lprsbhdm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwpdqgxc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3poefslpp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3urnpexdb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ptsxmfbb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3regvnxxq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xaeqtmut.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fhklyzub.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3txyubujg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dqsxkxjr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3beclofna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cronwmgn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rxafkwzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcrzlqsl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ucmcbgng.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pixerbql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xucmihnw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yanpzqlt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tsyaohwt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ilsjiabx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rexqyzet.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3owbshzgs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eeicmsog.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qeitsmdc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ekufrclk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fffvadon.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gavupxbt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3snhimwtk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ebyizbeb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3stkdqjzb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ssharpkc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3uwzzyiio.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gdcuuvoo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aimkddic.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wjznpdve.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyvndiv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3relxxjta.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hrwrhjxs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mrdujqsf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cycbgqxq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3katgwcxl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qktazlvt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ysklicgr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qwqhlvwl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3tbhblndt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bupvhyts.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ijgkcaxn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkqribm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ckoyhypo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvbsvfln.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3kcvgtpmn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3frbjiemm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wmwbrrmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pesjgaem.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3awrxsxbm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngsqftfk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vqqabllu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hbeujird.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3irzbjpvl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jlddztjr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zppmjcpt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nudzfujb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbbfnaoh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyirrrsv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3azlxebhr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrhtadt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvpylnym.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mfolcoeq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wexwokrz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nidbqdgk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zbphevox.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uiikeepu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vradopti.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyppqrpx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfaagwgk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3exiivzci.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zqnmiaie.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cmxjnnrf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dkebjajr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qsshxyfg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkgzzfx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stpdinol.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xdyjvfkd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vsrbyvkw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fiamsoqy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgpzfwo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hovpnhde.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tvfepppv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rfchuvrk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uwhzmyfw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3prdhhoia.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sxuccuxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3iiiccqts.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3amdobycn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wmwvfgww.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fgqjwuew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mzchrxzx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fmbeqyko.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3epkbdrcr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqttrsgh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mskgwdnw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zjeaxkhs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gtiltedh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ojmoxmxw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdlofkoo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwogjond.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nawvicek.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bivrifjw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vgehdpnh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3nyhfqmax.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jylsuzuw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ksysrjzb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3erolnjtv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jggxarbd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xoaghpxx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mghlblkx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3szapygbe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3frxynrzk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3glynkzie.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bjbpvqgo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rwxkmqul.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3twurefdt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3utnuvagj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ujjfucvm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iteynmeo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3usgtzufz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gfvdvncn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrcjoefc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mhlojxej.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dolndzfr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfmrbbpb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rcdmmhgi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dpspvlag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qsiacalq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3npqdtymv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fidbbzty.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zlnjymjy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rfzarlgg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sxoogmrt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wanerovq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3egxkzqmb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3beqjdgxy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ikwwuqex.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgsftwss.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aemyojef.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xseguekf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oilfjokl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vrcbpfpq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mtbcehep.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gymrtdon.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3smyypryj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3goxsusxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iyckztin.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3igpgysyr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3grnenuot.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nhhbtxsp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3fcapluzg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3cqpisbli.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3meryubuh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yqdbdpvm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubpgwfit.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jzrkwzzg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qbjiaixo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3yzluomja.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3beimrnuh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xdorzlwl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rfazyerz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kowhhdqs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3juqlfaks.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dsdyhxzz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqagjwj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oazlmkvc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jefwfwac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ttnwittd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3noekjbnj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zlaqajch.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vbxvntrg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ckdmchqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3viruboql.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ylzikavv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ozhmaokh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3friilzgj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vdsqtrep.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tmhcbmpj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3flvuerkn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zrdkwrnl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3higcivis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cpqdfefi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsatacvj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlicojvn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zqtanvwz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ielcncgf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ipabgusx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3npyjoifn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3liovnlcd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uzcbznpx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3quhdvphr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wmaskbtn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lqtqfcmv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jzclglat.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xiydxdjo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jobqudvw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xpwrcvav.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3abjidevq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odqnmmoq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xuqhzufk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hxpyadck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fsqahnlb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dncdmwym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uffouxxj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xcvudvxh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dhdqgpao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyfwttrg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pvmtqqpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbmzsvjx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ujilobgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hpbkhvms.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jgrkaqwt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dzsoncao.html


<!-- 参考信息 -->