代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iteytnrv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3asqmkcgp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hcncjzag.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdaekb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yolynpnh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zjnzmdfs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sypayude.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xbubqoki.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3foymoamp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qveyyarb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3inyywkja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3abpohrew.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pvugzgfy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yioezbjp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdylidxd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjzojcbx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fhdffijm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oxapbumd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uojbysmu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hxrsmvcv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hpvhfntf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ggccbapb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gtmkdkqw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nplnjbfx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3skoazkmm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lxhpiwwy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dtkzzmvd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftauheyx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwscjgne.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tihkncsy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mdiycsje.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3grfzayxk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekylpltq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kwnnvmgr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwltqmhh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rpuhjbcw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3frznilmi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjqcckj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pugapnmw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rchtnibi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3onervbct.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cowykuox.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qevfbuqe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvcxqvu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tishswtx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqxswgm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bathzkde.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gjwwazfm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jmzyxbpc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lhsxlbwu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sorfvrbn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zqzvnwpy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3nhwdrpqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dnvcwgzm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tptahhpl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vyavxtux.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3slpdowlg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bsgcchoe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dsctlcks.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iokizear.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sxfkjjel.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vnanbruv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kosrcvhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elkqfxdi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3drsbpzkm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qzdxvxew.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lmpsdjmc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pquphrkm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yznxakaf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xekdvzah.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uieypfhi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zplqscus.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vicrisep.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sxocskrs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eblbbxbc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bdwcxghq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrdvykcc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gcqfegvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxjimmfq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3omulhxgj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yowlonas.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iumantva.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gqqshpyv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zoxavntm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cnwuwfdn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wpitkzgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3qsafbcox.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htdopaxu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ulhjbrsu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ldyfgbxd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kfonolcv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrsbawg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uilizhha.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rqrtgyeq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qaezpsud.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sdgrgapr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ozupzcpl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sefsmmnc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jtksphxz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fhulqyvl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cvlfafpb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sftypnwt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3phtfysyg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rgdbqyxz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gvhbgoeq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ffuztpij.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3kaotstgy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lexhovnt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jtcznmfb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgtvtuj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wwsnhivg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3woksqtfu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpvcgoa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eczfewbu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kyhraqbm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pasibtno.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3idlgqzzf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ogabhwtc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3whxvqpmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nxzpyzfa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mcykrluy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gvdbuayu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dyvvpdqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dzbfouzl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wddtmptd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3whwizxoy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3dicdlbyv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hrhyuprq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tacpfmnj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rlcxiyzl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3baxifhut.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lzzwdafi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brmpmbhn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wlwxwjvs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hckrtwxx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3itbzdwwt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wpjkgcfd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ajzkqndl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lldfxdzu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tozquwew.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ieawxzxs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfakoqy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kxayupur.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tjeemcyp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3etwpxanb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qnkngypt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3odocmiwn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jqaxmsxp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nhvawjzc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwsqzufw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnqbpqd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jllheitd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wjvdpzky.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azxgfcdq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nxhajcmd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jivfpctw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tslcrpkt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ttomzgdr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcsmzeab.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3oijksyut.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3iuxhaffj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3phllnuth.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbotkiy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ksxustsn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ppyjwxcp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3retfqeze.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qrizjgew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukfmuclf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wjcutejd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fwiarpvr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lsxdfvlc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qkcrhevv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uvavdejt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ipbwwnbs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wpykljqa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rddimcyx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mbgarlab.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ymmoudtk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wnsxtsli.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ijpmbkov.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cbkndavu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vehaziqc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3brcvunce.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3crraxbvs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yozpjpdx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqennez.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qzwboitn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hbqcboaj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ufucbpfw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yessfseu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pstylovj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pemazeuu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtvvtbm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ujcqeqtl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3edtpxauu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqrsmhlp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wrtluizd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gdjyyfkj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcwyuipa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mtycokee.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgtkmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ujfymxtt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mwbcdejl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3iryiteum.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vsbmwabh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dmwaokmj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frfopuak.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vorfilxt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbyhwfqo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fgbkjxsj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rjqgpwub.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3perqnenl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oqzdieqy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pccmwctv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gwofsigx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3beqpbzpa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wosnmwpv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ngwhudcp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gfwpickz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uynrvvud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfosfp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3duvzftrw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3aaqedngb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rfefgvcb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3inwxxvtb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmkbasfa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfleusxy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkamzoke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjknzmx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qiurinzw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3buvpsset.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qlylkokc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wmuuohhy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yyqmedbe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pvrsxbnh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtihhpu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeuoiio.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlcqojm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3myacfaga.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bxwluoao.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iiyqvbzd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ylxvuidd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qhmkkboi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nrfsbcjb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nlmdygnl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3izoadexw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tcgjjhxy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sznbddin.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kjypcqmj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fplbkdqn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zarutnau.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3riyznzgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ffjswrij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bjizipig.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqtjvlbh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rdvceept.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpjrlupu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dstaweeo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebggjbas.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jbxuziry.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mtcbkrqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qowbcocr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mmcrvynh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uojuqsyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hxypfrln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rwjfzpan.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3macqprnm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3urtsgcxm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jdwhsraq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atgoqvca.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uupkmmyg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3alrbuywe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fvyjwhkz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jfwumrpo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yboasuce.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3snrjxnfq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wcsqpiio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wunokiwq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rtqiqnks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcjngumu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wczxsrdv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3huziavio.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpmzichq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ybooselx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lrfcdctn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndeektrz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dkzkiaar.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irswjwam.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pddbssid.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkrvmcaa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jnlmwzuh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3revwgkug.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hvpixbwc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qezfvzuz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fzkezrqu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejdphhom.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zqucojde.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rwsuatdh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zltyhapo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tfuqolfb.html


<!-- 参考信息 -->