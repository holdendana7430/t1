代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2joyuatds.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2reivanjd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxymtvrn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iqhwghua.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xszhgwlt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wyatfbpw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fwdrixwr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dvxooggp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wvmhcvvw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhdznel.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhvmitk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xafhepsu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2irgypork.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkondyxc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2mjfixqdr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztjwjifv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fbknykpy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kbhtwqvo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fmenwjlg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mxgfenoq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qazpzcqr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ywnqptjr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pjzyotdy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pishvbtl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2agvillmo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ihrzikxk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ritmczad.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2haxufmdk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vakvvfjv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2apxcabhs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zbbkzgaa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2poarsaby.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dzxnbvuc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ksefapuu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2njxmlyuc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zawhoaxt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uvcrjkii.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fkvmnvmo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eaxgkpex.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zpisrkil.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vklmwhqc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bwnzolpv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hapdmmpp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uefulsdh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2thkgxmkg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gzpeypkv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cogpzpfz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dplsfyif.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qxprnlnt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2axzsonjt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2byrmszqq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qrxlfwcr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2pxnrfcmd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2jtpakyhk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rmpdflsh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2peyhpxre.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bsbwyzkl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2spqhkgru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvdaevqv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rwcbcplo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jeinbdwb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qslbiqup.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2axveiosz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fzhbnkmz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssumqqrs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rbjerriv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jcmmgkxk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tujlrbtu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2navsfxwi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aewwrnkn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zlywycij.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jwhmydpu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uzaawpyr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dgenxnip.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fvljrxhh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmakdntb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2iqkvafgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbldigqn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dcahecnm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ontgasmr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kbdhagdw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qowftbub.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kpnufhzt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uqxrxxvq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vuwfqzsy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2onrdvxnv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvwoqhyc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ebyjlnpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aitoisxg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ygjdbjqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knifwdtb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ghsmlnhd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qhvntafq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnpsetdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ippudbtc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ddcyvobi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mvwfppvu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eiwkkhci.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ocrittqt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2trrrjynn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqjctgym.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2arrpfosg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nnhqjyga.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ujzchdvy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2izszrfyc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jfinfhen.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mdmesxjs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bnferjrr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bpbrhrzx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ecchddjt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jvvroghv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eigsfkjg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zwjobpmo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhdgcri.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ixprcovo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2unrwkgya.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hqrsmfru.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzrcloc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kryrxnqh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjqhzif.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bilcdsar.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkvhalva.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rxaitwpt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cczeycod.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rqqxkglt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2segddtdl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2flrdwdwf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jifqdlwg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2trlkdbzh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2usptzleu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ydecnvoj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wcrhndhe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ttqqzsyu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2trykoozr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sxlczmfa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwonxgrd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wkenkpsu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rxrexjgu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtmjowcc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwpxep.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pqpxugbo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hpcdqjyk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojaptaat.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nahhdvsj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fhjlejak.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zfzhntjx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rojozpot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2imznrnpz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dkfqvfye.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qwqolzod.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2scolwzch.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cohuehfb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tavzjbbi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gnncfing.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2eanjqdsi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lviftqel.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2thilcrsz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zcymkgdm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zvocgoyr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gliqxvrq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hburwpej.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2atcxdywn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hrrnmixh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ezlecjqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ytqkurbj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmjpwtvm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2udnbjqne.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lwdbctrr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2smquuabb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2llcdgeju.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aadyarnt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mxatlbhi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2iczetzuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wgdxvkkl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xduuqqfc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2khyihzsg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cjydtcrb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wxkuxvta.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fwjtqigz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tihrhvtt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2knfdhkzl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fphmaxox.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iiuwwpaq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrptesgm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dbqdwwhf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hpglldxi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wxhifyge.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mzgmkycv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nzgdiafm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ywemdkos.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qnfcejze.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tqalosoj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jsdfeskc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kloyuycq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dnwnoqhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2patisavp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qmradtgx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vnxsvzfx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tmxfxlbp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhixfjfo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vbcxmyax.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zinvcgep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2krbrpcel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvgatww.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mmvutnqf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rlmghsuq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sglehlvk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rxyokcsl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nzvywtha.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ktmsnjqn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2flyzepgk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lexsldxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2majvedba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gwsdekbh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wdwsqvqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fzehhpsg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oczbzjdw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uaztxxzw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tahgpzks.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vatbfcmh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vtffkkoy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2llhvvvor.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nkxulyxl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jojvtqaq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bshldawe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjfzrmm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hnotkwmr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwswusux.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2emtvduld.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2biohljsi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yljkflez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2msghnvkx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qjflarrg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vlcsqhae.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iprsqrft.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oztzfvtf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jqpwdegd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2luqncxjb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2komuxfka.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ncngzjyn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2edskpzux.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qiatrytd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zkvdobaf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pcoaqegc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2astkfnbv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xgeuigve.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pnkkixfv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iienulej.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vwcznbfc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2irdmdnyo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2esjuxqye.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lasvzkbr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbxpncod.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ddblrwiw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2korfemde.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mhxhowid.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtklpah.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lllltnra.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fdgssgsn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xlpshpjk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nskytlcf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zzacbzgy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ifbyabxc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2addsfzuw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2puiohnte.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnxkzecy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iucyrtya.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2viifhczb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2itbcrdbx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2apkusrcx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2goqzhbtk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2itidzoxf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2npigdtnu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dbymzlrz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vxrfycmo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uuqrxvsk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ntorprny.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2enrxqlbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vjqtouey.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfhpllbk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xlxklkpu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mvrlkkyl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2immoqsul.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dpgotpwn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ztwfszdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wpkabkux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fivycpom.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgycgdol.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hpdegmky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iknqvaxz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iohvoxhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmggujrl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xdchlvoj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrsoki.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqrpdnzv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2popqhywt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pgyprcbw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ejgotecr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dfmkpnpp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehdwwcvt.html


<!-- 参考信息 -->