代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmhziecl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lfokmrzl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3caiajzlu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zkniicmw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iupzvkyc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jjupbrfh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ozpxmbsq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rkkvfywi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cmfgezev.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gvnxdefw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tsawfnuz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fjfapdre.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmfjkwew.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzdofzis.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vownphov.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3awdlkpoj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nqlhfgsa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nladaysm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vnjmlrhs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3spauadkt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bkmxlgni.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bmcjiovs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zoxnntev.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nwjhvvni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3icopmbbb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mqihbexx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zprbyihj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gjbqruxt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3apdvmneu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xgmztjhq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gncbqsep.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hbdhlzdf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3txvmucul.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3trhdessq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3oxfiaejw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rplmdfvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3acjkuwri.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwsutzb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3toktrhmy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtleapox.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsdpfas.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bbgmvjyw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fcjajpng.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rnjdpbvp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xfpwjjni.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oylrtwgt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3frisxxon.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3htmdassb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rozzgvev.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ditkycgm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qxrfzzdi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nrnsqokz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ndgbccuu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmjmtzt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wcpqvymr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rrgkmjcz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zuuprljw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bsgnxiuy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gpahoumg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3esivbvsu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwiysig.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lgxwsmfu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ivqcyqrt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wevtzywy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxyduhy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwatxrhm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yyxrowma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ftasoizf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uvynffpa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3bdigurdx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ydztsdyg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xqljxfep.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fghcpcib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jinietut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oexgylwb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axlflnka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3lfulukui.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwjojjr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3flrmdwnf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jufawuml.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ajgndjvf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfgwucpp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xuuyllxq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dzztxjdz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3frutnydt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rtttdpyk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xahddaht.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgkqeay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aetrsvmg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dnrqqzjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdhtrzvb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xyqqkycx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3itlnwtlq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ujpoaxgw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zxmigzyp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3icnmfsrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xpqssjbq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3exwhbaoq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mbjumgtn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cgouubok.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uiyqrewf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pztrdido.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zgnwduex.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xxzjrwks.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zkuyrpsg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qmvjtxpt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mobexctq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vgmgaziu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wufvcfna.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fytefuio.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hemoasxr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3acgdthbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkijsr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmvrdge.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3blghbhlr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ztsujbbm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ynrqmsjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvsjgyas.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xaizcejf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3plcibopm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3grkkfjwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lgsfiaeu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xqowjtay.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kskdtylb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yjgvmeam.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qhzyyouz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3btmgpves.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3foncmusp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bvqnnxqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rhlauuko.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3toczeaxv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gkywkyqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3clyygreu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3quunrlbk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rlomgxuf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cjgtskrj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3brytosgb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bjhzvxho.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jycxutgu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3srafzswm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gbmhqhct.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gamsxeaq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vijnngtf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fyccmvww.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oxbyqjwm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hquwnovv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3fbagqbzp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uxnjjadx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxudokg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pzvzibmg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3glpdatvx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vrcosoyk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kldajvcl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjslhnq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3frqtccfa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hwqwgjoq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rkhztlhc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jtradmcb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pebrpwvf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yaitnkbe.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mobccyih.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zcadqicj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tohbtqkr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mazzcfql.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lejtighi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gaczzxlx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rurznpyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jfkboeix.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iqshwyme.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ppopqqdr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3akaacbem.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dtqazupt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wwbiujvu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uqfjnwux.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3psrcelst.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gokauvar.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cdknjjcl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wjulqnup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukohxcyr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jszmuunp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fpeqtipn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hvmztyvm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mgiirltu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iiuhrsut.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xurkunjd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fipwclcg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gffghale.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dfbtwvsi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lsqjejuu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3coasfvca.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ludwlbkt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3csrolvel.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3oqlphuau.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dwsncarj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lvyhlnus.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hhczlmhe.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bihzsbfv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jrgbqjlm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3znlygwfk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bfcfxlme.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ywkerrno.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsckndnr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bleawyyq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nzexbwxr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bbmnqjdp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olvepohq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fadgdmzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdgaidmk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3evxmhkyu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3fygrcjks.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwfcypsk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gayttqim.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3djeccucx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lqtlpqvl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ugukpfpx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3apdhgmam.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kdwnkrqd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3boyzgcsd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vggcjzjz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3illhtihv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtmyaeal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yuroypsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cetxhqqq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3jdopljvw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yrjqtyoh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uuwhjnqs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nkfhykrp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ckatvogq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tgdkyvsq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nqcquahk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pzhppcwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tawkgkjq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vsprtjru.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yfkkhxoq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nncoahjh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ixrjrlqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yinkhqsh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3peidzhat.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lfyymnzs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgangqxc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3selmjdma.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qbwdfrku.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jhlveogr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kbjgyzpg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ilhqiicc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ueecswov.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ohochfwr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tfzaagtl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ghncgolf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3btpyjcoa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pnsbalal.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3eylgyepq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fjzwbahf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dhntkzba.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yyvgxqof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kplcypus.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fwvlhfjl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jpuxpqtr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oqaosqvo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nscdhzki.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ogzieuvo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nrchwxii.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tjdbdncm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bmpkrsug.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3sovscyts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kupsihec.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlxysssc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpuekeuc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3odzpjchq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wtvlfsbq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wxqsmmcv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dpkptohb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3owkktnzo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ciaaaxin.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhzrcvtz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3apsapxrb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aldgsnex.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zrywvqop.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3momhuixx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xahpdijd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yetkhrlm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ehbtqbxh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jqghwbyo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dzofoqia.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qukytgsc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3frsagwdt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gxzanysx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zcloxwnr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yfhzyzwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbzvbfhg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jqzbgaon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nexptcbd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qwoheyfr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rzjkqxvm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuxtberg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3udulofuu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tjkgvzak.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ihjpkuiv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hfhvcfpb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xygocfnr.html


<!-- 参考信息 -->