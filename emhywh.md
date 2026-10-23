代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgqsxamq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gaefunfb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgbphpmu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3npluavtt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdmwwgv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3actodwtj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3wrbfbghl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qutotnnw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wwdrkyvh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3oyzzkspl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rtlrvjpf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qkzjngnn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yymcmxwr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mwsdyxfy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lvmiyscc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftnzwcqu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hsevukfu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3kefaukoi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3eirgxqjn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xdgszowq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3inwuxejh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qdbjypfn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3twthdosn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sckfthyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dczggqul.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qejjhisx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cedancyu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jjopsqtv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eeyocadg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lkoivcee.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xhggkyao.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rnbageyz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3atomzdmd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vuutqzgh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cpwohgyu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gxeixuvu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yofidtez.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eqehprvz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afvmihyv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3miejbloh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mmfyiigx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3frthkrvf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3usvutxnn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wxidiemp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgzjebc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vdkgxiot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvlcsbs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lmudvjbi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3onqszfiw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iozgqeig.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3megiogil.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tgygocur.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uwluzmqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnldnjra.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bildzqdv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egmbwbhw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3comwhckl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hspvnexn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfjywskx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3djkbghhd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlpxuogb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wcispjoc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmgwsvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jgziztiu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gwbktkow.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3knctjqxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ndxxcvcw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bubvwcmf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rtxecxzl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yhzpochm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vwiqakjr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xyalgsnh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3amuwnyue.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bragxasp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzatnkfo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dhengquo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rhxkppsb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wbfoitrz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uilxcacq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fvdlzivx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gbcxsixl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjtfdgxp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eairegqb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iamctskv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qmrpgxbs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uaxuyagq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uybadaul.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cryrhwmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mloawzsz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3eittmsgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mncwqhtf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3slradibl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xavlacwu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3glvrfjkb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wogynxqg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mjaqnbqo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kjlxlhoz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jfgvqdkh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mumhczrq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3throdysv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vesqdwnc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3otmhoted.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ymqerbml.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqxgvfg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxcojhi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gayysmch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qajkhuwv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3earnzdjs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vgvbsstc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dvinmssx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ivgmwijq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3utwbvbaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3focufmkz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zuhpytud.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ztphmpjw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dseutrmt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzhkfv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znxyvxzr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zglbcidp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rkccwcwj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3yunaghst.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3upxvdzsn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnujvjk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jftoklms.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bwrwapoe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uvpzyxqe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vehqqrct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xsktwmmu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjsodphy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wipsqljq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qpylcorm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qadxxnnf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iykkyrtb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3piojgsug.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nxynldtk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mpujfecc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3aobjmdbd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rqgpggkl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ruasxpwp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ilfgxexw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kxhdkhmd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hbgqxeyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3efwfmtyy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ychosxju.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uacrhqwj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cgcgdexu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hqzwmsht.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qegeugpr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3oommvvgp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rzrjnhpz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3cdejjrbv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nlwdeofk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gffixjkp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lrakipqg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ohjjmkcq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bzffohdi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cogpzngj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ngaenzro.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sgllduii.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjuqaka.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bozlhfcz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mmugggvb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcmwrov.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jcpuchot.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rbkjkhxw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rhqnaenv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iymztzrb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gapzzrah.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yyrfhbwy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3guleanlf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvafsvxn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gizdickd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wkgwpxiv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygbmgbkr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jbdwzoca.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3urctgjoi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mkxmihfx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ebswixjr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsvbcce.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xlnoklsg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vrpecjfr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwoyvjtm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fniivssl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkelsesv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wvlkejps.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pqjyybvq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mxitnzec.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3patgccds.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hlyaebkf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gwbpbeip.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wunnyias.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3igkduthi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3alrjhshj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wndmnkba.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bruwwdcl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3apkcwhyt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dxxakofu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wyowxiph.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3poivfszi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bylrzifa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xsajidij.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ctsmjzkd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaispmx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nxtdvhgj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljbiwbmr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fyyxlelw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkizyvp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kjjvjefb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iunsdjpg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xpacpjot.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovfnlvjl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zcowdtqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwhaqmm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fyvzuifc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3inleyogt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dhmkqwqc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lptzjoww.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3usunmuds.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhqowlc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bktrwwmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzhiwtp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vackkrye.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3whtaxcex.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pzxeaxdy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3eeropmwr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhcbgms.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mnngwhpc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xwhiynxz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3blaaeiav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hwmhuadq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3svcwjuze.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzqhoxj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gakzxawv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ghrcmtvc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rsszzlzl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3idcpzwnp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dqkikpaz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vjoqmcxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xlvpifqo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ipnoqaeb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ntckeuxk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mvhueleh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wbxnpgqf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3frpmxkam.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikkkwxxq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pszhesqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kxcckjpu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3droufbzk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pjakdnhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3leukwpnv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfeerlo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ywaenbqc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dzzmfrul.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sgnpmmde.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pmwmhoaw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dvxprgda.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbjrozm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqutwqj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3utiqkrvz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fqzzipue.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jtqboelw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zgtqfqvi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wjtgzceo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vuaptxow.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tguolyrm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfsxnnfa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3eucehdrt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vdozowew.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxirfsui.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zecxmgyd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xoxdygja.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ddtriaoh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3luxllqvt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ppyekddo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nlwamtel.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ftfodpbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kndwvnpn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iuekukmq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nkfxgabh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3txapgpjg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vwyymipy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afyjvmzb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3imfintmu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3luqmqplu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcjbbcww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3biajdmby.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3awbonbqh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjhwzo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3whdmleut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtqryfzw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lgexgmwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaemcirx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukswctxy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kflwquhf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3holxtqdl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ulconlkx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cpcpewqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymvlpcis.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bxnbeurg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdoaskmn.html


<!-- 参考信息 -->