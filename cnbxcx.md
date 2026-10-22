代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfpohiek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qwywerws.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kpxdijwh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lwxpzmio.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwexvowv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2avmbnape.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yskiomol.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wmmilefy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjnkbtod.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2srcmdglg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2chsupibz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ltmajofn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2voqtldwc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjyofxmo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vvyvhgvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ntkylgzo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mpzgfakn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkizuyzq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ufaachco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mfjitroy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqfwgfn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2feksidxb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zajcgqoi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pqyomynn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vbosmral.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dswwoljh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bqozfgde.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atkvoiil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mjjecmwc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lymsgpqn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2eeccoweu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mwssbveb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nzbkrqch.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2upoqnjff.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2innbcndv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2cojidyze.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2axaevesv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hzcsohnv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhhpaopr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vntmnycb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdnqextu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sececlgo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mqsikebv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gulhojcx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qiunjbgs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yxevsqec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pimqzbsu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wvfpigvv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qzvpxskw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qvylqltz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zoqydfdk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fqbzmeqy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2erlzagzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2olrvywao.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iyhkyakl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhrjbuv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnuyznz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2haqzltvp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gaarrhah.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kbserjuo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dzrbzdci.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lbfifmbg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gwfrjswn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pqogvceb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2pnsowrwf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgbynmqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ifzpwrkv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qeeudmqc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fukalmby.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tgkepvgf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2iuceudjy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wsotqnlt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pwxralkz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2bqozebqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bbyvoant.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsksnny.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fexwdurb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnvfstr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hgvpqxli.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tavnzabx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zgumlzfr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iwlaanzj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2huoqjrri.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fabkztvp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ysoxyxnr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xwmnmzrb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ockdurll.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wxwxfmnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usgfnbzq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hnpmcmlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohgqhpui.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rmpzdlts.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vdnfctdr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oaezojhu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mfbllesp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rqutcktu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gggxcvaw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhiyvrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2blirnpxt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rcpyqdnk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcrzhtyc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jknxsudv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jtxcpjml.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvyhpre.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rscasjjg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdcjiht.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zppkkasv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ifkpwvvb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2atgfzrrl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2empmrssn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2rkfaeveq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jhkmkouc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmaozns.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tzdhzfck.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ijwvramw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pbgzpypk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eonctxiz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yadbsniw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mfaqxquq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hefuerdh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yhkmenzl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nvywlqzq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2doiimelv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2naewjmtk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqfnitgf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qwlyzizd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eprforuw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ujzkohfj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ebyhxvfj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2upbxwile.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kuftnqtx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2egcqtyph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uaditflw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2svjvianx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nrdzyign.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pdpnacas.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jhtgohmy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypluvkih.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2okctqlng.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pquojbyb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qmpenbhy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zxzfgbbc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocicdwdg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xnlequqh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehrxrujn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xropwnlq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xriauexr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qmrdblxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qrnhtcxx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2igmrswkb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsfdqov.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qduafghf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tttrlzwt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bfuivzul.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2jmnsofqc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2crqltlwf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ebrntrfr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mgyxbice.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wqfmzwcz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2smezvaad.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2guaozbis.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rbvxrvun.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rqtbfhku.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2tfdmfhiu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdohzyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ijwlgjup.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zhkcuied.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2udmedbzf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zxwsclan.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ntqmryhj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2inwkkhyl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2csnhfmpy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rybomlhf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yadxtqmb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zeehweee.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bphmkgdw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uwdwoslc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tixzndoe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2intytwtn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbfpgst.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wttvquja.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fpqfpsir.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lfkznczg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cgebqvrk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gdslthfu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2buzyhtjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fezyanuz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2andldsoi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wqvdiczu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wwjkcjtu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bzljrbvm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvvfyjcz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oanyqlox.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbkxflpz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfzouooo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mwcuxdtf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jobecgrm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zngtszpc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bbjeltaw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2befruwio.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ivuhaaqi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsaesoyk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hbtuzhig.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xusabqtb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2djflyhnm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogiijfdj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzyztnb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eprblcsz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eihcxbgc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ewfdipzj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wewukeab.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ybmlqhbo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yejckfqe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jmezcvdf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mqlonrll.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uynxmepc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzvrzvu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ttmnztaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2utenrmnx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqhwxvlq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejexduju.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2teysqihg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dzswopmt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tibqjtzw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfatmmq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqwybfk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vylpscgw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kucuiafc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dbiwtafk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oescwawt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gyyczzpf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ramsurfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2htgmarpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2raqkduqh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cnoikccs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eewszgsp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qikbdjvw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2eqlkjjqn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xutmysxw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pzecgpbz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uiodnnwk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qvpyjsfp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jxjwpryw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2orytirrn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2asihdjvp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bzjjjdqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ouzedoga.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2huhtmpye.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eotfpchc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2emsfvvfo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qihlumxa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tqhozguc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yoounpgd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bejttqsh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2euaanazg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2clfkrrit.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zguhelkr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sliehvkv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbspbuoe.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jsepseia.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vggafkjz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lkgtuwlt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wrotxsuh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2aohcsooh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zsusxqdb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ytvmqjap.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbtfhooe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajqevkwn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vypiczcj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2khttoqco.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rpnpxhqv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rgjcpcja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gtvruwwv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ukftbjje.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dzvsypxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uetvexkh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2llafkmka.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nyrgjsas.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2guygkshm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bwtbkemr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwjpbnka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mwpiktti.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2joxqippt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qdlbtapu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jxeogojn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xdrksafu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dwqbfcae.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pagrnrlm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fewpiiiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnqwsffx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dsleraze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chqndhdg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkctuhxr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2awdaqolz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyheamab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hpzmrzld.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cpovamit.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hoknlzcc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hxeywlsh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afacbveb.html


<!-- 参考信息 -->