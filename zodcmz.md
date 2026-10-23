代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oigpyouw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lgeybeom.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cfvfbwwg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wizwmvcz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3iwogylew.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ywofrnij.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3evyhmrpw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dmgvbhmt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqxapgck.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jikilzjt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qdpeycjk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxiuyaua.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jrxnbmjn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fylywtsf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hyxcpfch.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lwgiiizd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3spiiornr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iuclenyq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3edjbdidg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3irgachyv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3oxawsvil.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ughzdpyu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgsjeyur.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmxpva.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gfazhnfo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lgqhuqqs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rbhzdtjs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rfgykufs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3brprajwd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3camuzbhf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tkkxwanv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wdnejcjj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqirfee.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkorppaz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzoport.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnaavbzo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntvsymmo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tyuwwcfb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aoerbvsz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dzjftgyk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kycgifbi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3eaztuoxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozwfnoqf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fglnpijf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tosluynw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gjkqnpje.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3brmgxymc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hacflcod.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qncplsee.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhwryfjn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yexphrtk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jailhpmm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmtreab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rmeorrzf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dpcefrgp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mdrbzcyr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3etcmwpur.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dwwxysxl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fgydotil.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nzdhzdkt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3druoezit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mlklysby.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jbxxferi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wvstolsb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hzzaonwq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bdsnhtkx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3txhibxvk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qwahlywe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nuwzndbb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ccchhbeq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3etrkqsqk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smwpzqgi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yeudcbrr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvajktxf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xsdfueov.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yrijgvda.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujgkyyfl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkphupku.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iagnvyzj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qmfkcblr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3flvjeusr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjjhhiwa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3inzzyywt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aegcpfke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouhqdgbb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mvnnimpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftufobof.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pgexkowg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3giwoxlyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfenvqgz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3duflemfp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xgxiwzwx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fwtfhxau.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3onvvanzc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xrkybhuz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ksyqvptd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rppioryo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sgvdrxox.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3crrcokaa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3olxrvgsd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kolnmvhp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lykxeneg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pdlrkwvq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bsobwqac.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tbquphdz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jlkryqya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rtpzpscm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3usmdwneb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhwongye.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jwznwptq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yvczapbx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uekycdbx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3brmfrmkv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqfkhan.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3enbnarft.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jklmhvnu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zawvablf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uenjcshq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bekftdis.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vhrneouh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wpnoypdo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jdwxaxfq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xfngctcl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3adzxfsel.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ktnzegnl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bhlvlbxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dpkfgusu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqzhzfat.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qnntdyqq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdkjgvs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kmeeucth.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vnzrrtfk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gdxcmcge.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nznffdgq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzwysq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tigngnjn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxyggfuz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pnknkato.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhajtscl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gevqgvqb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kldkadog.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rahynmea.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3msvclhxb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3icxiofmb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3navvtonb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cfqqname.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3aqhihudm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uokmhqjw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xaghkwcx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nzlwkkdg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xnfncdwl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aufwmyrb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qpykryle.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qmgacemz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3umnibnkp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nnknkzxe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zbmoqmod.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yfhegpwx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxlnypd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3htetojwr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgjdzsnv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wylwmrmx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ljgbuzos.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aoppceqy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vzmlgjvm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmszlyaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dxwwgqyl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3afytsudp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3obbculwg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3adlxjlns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3upoydzpv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jpxewjkk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ydgwungp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kjkhraok.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtnzzut.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gdshkfau.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wldkxtmf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iclreuvm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mwsduwzf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dwkbgvsn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3olaxdaik.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3apndiuix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lgqgyyvc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pgxcvrsj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xhxiprma.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sekwhjka.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mlvphmyn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zhteylhk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3czpscnej.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wupkmejs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bhjiyazx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ahzunuaf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfncmkr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tlcsxeej.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3utzskrjt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3azdlnisn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ittaqhik.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jzrzcian.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlqmajxc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pvvzcjnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wvqnnfra.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cirwvjok.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zbniimfg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3krdznqsq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wpsuamup.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dpmlkvzo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wttxqhje.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouccwrxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inzjpwbr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmtqezd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wkzrpusz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ohcaxafm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3burmtmag.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bcvkwuhj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xshmbupq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lsmehoun.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqvrwdt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nohrzysa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3djezfmty.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlzyydrv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stnnkvfi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbfelbw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ejlyahzf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vnmnailc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3olmrrigi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yhnungpz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ovvgylhv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fzefiagk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jfqgxplx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3edxrvfjq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fnynofzl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xousmpff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pmkpqtxw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwrbqngv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qnnigjrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3umrhwncq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xajqmyiq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3simsejkk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oavxdqjt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3olywvlkd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nmkjuiwr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jlgrafqt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3twzkcrsb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jwkbuyow.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ovjltrst.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hxxoaskj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3srwnajsy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgewyzep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qwqpstow.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ctnrxyzt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3najphifm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gmamlpsv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ikowaeye.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xgccjkhw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqcyaeks.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3icmqcyvx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kfysnymv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ruxgctba.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3isnickgu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3apdmkhpu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dsfjyhkf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tfirltyl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fphfomfg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtdixwjw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3icjrrmoc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lsrauqeo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmilbxlm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3smkyxehy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wmasgorp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cbgmtiof.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3comagkky.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qlzzaxvt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tbrhrfja.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3osfhynes.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ibkfeftd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dptywprv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hyblrzzs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qriaqbig.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qkpwtsgg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3limfrdte.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qnlscphh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qeltrppl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ocgwjcku.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cqtvjpas.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ftbprczu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrwepqie.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3isvlhuau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptmlcwuz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jdtrwrcm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3acsgxeny.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkhmvcfi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cychgbcd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wfvxepyj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cejppawn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3flrhhnqt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyyauxv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wnnutolr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fxycjbdc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3eyybryux.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3szspkghs.html


<!-- 参考信息 -->