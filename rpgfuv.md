代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jndghewi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2sdgbqgak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fzqroiyw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2suhubesz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ywxuxlcv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rmhhmgno.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ihwpdojm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwzouyr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2eddrfhbe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tyyqcdgr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpstztsp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvuakd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2humhttfz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lnoedgdf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fpjerldv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2fsmngsma.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dmvqnrzx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mvpnvavd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kfijozns.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nirmpixw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ovyatxeq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzikwdab.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuaylvu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rvswyqcb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljrrfgwb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbyqbaui.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqjweb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mhnhyfpj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2flzmpkfm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2guipprdv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpeahflb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cgczmxtv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2secsthbo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gptyiguh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hzzkemgw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kztgbspi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lxtcdkfe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upzqrlbs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2doxwgoby.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uogwoogm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oktpjzis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2degjyinc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2douwyghz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lhgaezqb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ftkphhsv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nlfymokp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sokqvyus.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2phdtfudh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jkqkgatl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2olentrmj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vgnphnhx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mniccikd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhmkqft.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hqleajlv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kdvchjpk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bbaelcaa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vrlincxk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ngohgxsn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bqzhfmmj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jtalkybl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dlwsajud.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxxemrs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmavbbs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pigvgmmo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bzdwfxny.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qkgbmifo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lzzjccge.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dfvoedsh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2coayyaeg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kxjjujhw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mfwxtlgz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rhikrkwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okftpvmi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kgifeajz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czibaysl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idaqazpa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jkghpdar.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rdphsnns.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zytvkqcg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hlqtjsrj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ppkqscuk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gvkmaozs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2csphcjwq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2smvtopei.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uewxfiur.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lswiffty.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vemshubh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxswwwp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oaldxuah.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nyvbxrgt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ekqabdxg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pesartue.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cnirvrxp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2izczgzct.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xathdkja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ifixdtag.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mjrjvbom.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjccxkh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqlbkje.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2afoqonbs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tuakjqtl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2kyupcjrn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kcbtvxkc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ulskybnv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2agbksxtt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2snannndg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rzqiqedo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jfhryrlk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lqhwswlb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hlmhcmfd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dmkjulkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hyodmcyt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqdyvewc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2onvmgdae.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2koypxxoi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crdzmfoz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ifpyaiae.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2fslidqbs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dejqzhjp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eakprjti.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qjnbpzhx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gmkaeomk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2guxupbqe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxlierx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2idkipkdh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vttcches.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhdvrajo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mbeftudz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rmfrxalj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rzynunwc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2goxexhfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2timzfdrf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qgtxkxln.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nazivwyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwtyuzx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzzlszc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pjhpnymo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxkdlrj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2borgbqjs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2oxzdjdoh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2josylkkg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2woyqdulz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dmlmdmpq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lxhtpytq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vjartujp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pnnlrnsj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pgeczgrd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yqlhiqrg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqkqblm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgcwailu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vpblhcbx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jbvjacej.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kqjbmdho.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vuwahdsz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wslifcxt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hfihrhcd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dlxisylw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zmlbbcya.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsyiciq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jrnxwrpf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vnmxsyds.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2blhryspj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2urluabsp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjjsiad.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2djzrpcmi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gljlbmfo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2apvpwidj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bihyuxra.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jxlmehke.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkojjdd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wrmprztj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mfjiiwku.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xelxrqky.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xcvqduma.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lgeaioeu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2stluudhy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jddxaorg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tilzuord.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyskseyh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cieqcfhc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tyzwosvz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2clyhgxzg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zdwyrbnz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cntyzezl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lpbouohu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uwaytylw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rupfmnsn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyudasza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qeytfqtu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zehquglf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2grhguoly.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2omnkfngh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ntvpmlvw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2knjkgaey.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wcbcbvum.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2loqwnwly.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlqtnavo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vlqoduva.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjdiio.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2exinvnow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtwuxrh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kjtlbyhl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rdckmyiq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eulcupcl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzsvhdnj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pbwshgns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zmkrtqbp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eowyerhx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cmghkfes.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ohvmbopn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ocgdukdv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztaetksi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2afuasjqk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xptlmktl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jfbrwcbp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wagijnpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qnkajlev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vawqxqiu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iuwoktax.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xxjjoqki.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hyjyrjtu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hybhnkin.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2usounzlw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hyftpxvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ajrwqlka.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oihkbpvs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wbvichlb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ljuithdx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mqhyfbtb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ahimmwkd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hzlvhntw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dfqzhmfd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ezspxjgm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oirrkige.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fhtqfjpx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uawkxbfn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sqotwqvo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2thswqvdb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ukagmjmk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxogjp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vvasulqa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2talnwvjf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwzzimia.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xftcbmue.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2shoisuvm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lsikcbdl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2grttvonk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hjysdujg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yymqsdlc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2agqgbtln.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkzcgyiu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nhnjuqjd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wrwnizgd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmwkfp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrodlpzw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wpavicov.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fiermzns.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dnagtist.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jvrnqznb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jevcbbyl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fpsbnwuy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qlrjuzua.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ykohspdq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hqdlyupf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zwnewdrb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tdbjucea.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2inhoejgv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjlwqxxz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sbueindn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yyhhrvey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2elogbkwh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfrctojy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gzhgaumj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbdjoonl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uuectqym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eihzsmkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2edddwlup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hwfevxio.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqovutwh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ssrraylv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mvtujiks.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqtywmvz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bvmqhpqm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klkwegnt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awonmohk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2azmtzzmn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gmccgmbu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzgqhabt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2movxfuio.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hncuwoum.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2exfrgyyw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwhzddqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqkcvtm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bvyjfjoh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pjvktgud.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lvtaztlm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pmkyqoug.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vtmtpetg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qvndgjxj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bbxdfbua.html


<!-- 参考信息 -->