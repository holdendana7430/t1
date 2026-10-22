代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwhmsoa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqbwvco.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbaaljyf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dpgwkcuh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eapqatml.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hotxettj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjyedpic.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gcmajgdc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eliiyjhf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tezihrjj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2agtcpiey.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nwsqmcke.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kymkoamo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2clpkoxsl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2olwmrnsb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2neowwdlt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rffefzpw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sahggoij.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gleowctl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xrkuaybr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2aewprlkp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fszlfiwg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rutnsqyz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2onmfahhv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kismfxnx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oucncysw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2esbpuxty.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tnwnixaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2onrleqim.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2igqbegur.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fdumkydr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wasrfncx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kokvsxej.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vakczaum.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2stabyndz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2krxlkpfm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zzkwyvmf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqwiyqq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjcjca.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oojupckq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qrybqwbz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hghgtbtw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhigmqr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xjmbhrky.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbisegy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rczshhya.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xectpdjm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wawgozwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnammdqh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ewakybsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urqgffju.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bykcnelq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xofakdfc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2raukwcfk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttaovvjt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pbzwhzws.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hmjnkmls.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2shswvwmc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ezkxdcpo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2miypnxuu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2clmtzszu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kkejfqrx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uuskcsav.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2geoemczs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2erdtstla.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmtifsw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ldlwbojw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bnejugxp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qjfrakvw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ilqjzamq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dbxrgbjz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uabxitiu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjyisuu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwsjjbq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxncie.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hdyzwnjv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ehyhhpcf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mtxbgaml.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qhnbkjxj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wiroaoru.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wjxpwdhd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2oghfmmpl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wenbigld.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cacwxvjs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gamirfel.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mwktpzjn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mcickskq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rvfxonxd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jlwjovot.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zhuexjsg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2geueeupm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmqqgjzh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbobgoc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqcmdgg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mhjngibb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bmoiwaxp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ptdbcpoo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eflseftb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekilllcw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zybuasfc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tylfzjii.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ezwtlxcq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qipmknly.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnezeivc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqfentks.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xftunymx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2egirukvp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2najoqzrj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gkwtyhsj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2llajkezi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zhvjcnye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xkplkrpg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jqlfmfjy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pxedjknz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qqwvzgqr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ikcatnqh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qthniyil.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2grldgsfa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uayvjazi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fkfqcxnt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgjcbkf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2motraijj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vanihrbz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jxjzfrdb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zieluqsc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2blqzyjbx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xxhtscmw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uhfrzaqn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eeeitluq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mibslinv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2feemxbso.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2quewhrxf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mfuxqurx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cgynznnk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gvjrzppi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mdydvnqy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wqlrdrpu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xaavaypf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kakvrstu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nuxfbjiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iqhmwtci.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpxtgtjj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2abeczoqw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kmkxddgg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zawioton.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zscapmrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fremfvxp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2sfsnbrzr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2udfscdwa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qzvfefog.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pqwcucmw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fxwttypk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ladzakku.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kqjpexue.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2thwyvvex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iktrbwzn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wbzqwxvg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vecdfzhm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gxfhphwb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2utstrfpe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mibtsumb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tzmoibpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zaehftcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdeyyblr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlirfuix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ibmipkon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2htefzhzf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nznpzlln.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ruyzkvit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ripcrozk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxpejyim.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vnraqvtq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gllkklff.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ksbkldqs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ijpswesn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ndeaqjdo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ohmhifwx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mvumzlik.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nkwtbdgh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmwtyg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qbhyizub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xnulqbcr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yrwrtyup.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aumtznvc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gvaoxryk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pbdteocp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lifuyiib.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zrhhimip.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qfeqxcxe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dcgzatwz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xoakezbm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bflyknoe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2orztkimh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uvmizadw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yaghmjgd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sqwwqawl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mbzevxqj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wousgnda.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owaidwku.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erljrkof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yaeurtcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xatfrxru.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ropvtwtx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nvztmnqy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2oqlcdypa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ezhuhhgs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lbxykfci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ehpwpllj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ptnuwixd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ktngtgwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiindxv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lrdjovpg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zlzsgdmj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cclfpdoe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zsknkfkl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2btbkddtn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nywxrbnj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuovurr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kirrkwib.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cptfebmx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iimawlhw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2peotztaz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2shppjzdm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gjpyzhtn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cushcyfm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ihbhaltf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wlbycpmp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uxukirrg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yxzjshpn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2acbtugtz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpqlegrw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2chsosznf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2duhdcyud.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qqojaznv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aqokmvho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aipwteol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ljujikoi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2objaecli.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egclrmiz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2chbvzaqp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fkbwisld.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jhhpkmbk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qnlexlld.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lckpqmda.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2llglgisx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2engjlbqa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gkystjug.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kgezgahi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ubbszhqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfomkvjb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oztkhtms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izdchnlp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yttamavd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xwtapvsl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lqaodxrw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vfhzyiff.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uhphkzav.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2upzwacgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pzbepfyj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nehwtoqk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ydgtakuy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zdkehgff.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pffmvrbu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvrmclm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxzcwxtz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hanphtut.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gxdirbrx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2evcsfpgz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xugmrsnc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2eshexrqu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qvoaqhvt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qglsdeym.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uukzaukt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dvjbrnlz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ogfxvuzo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2elhhtvsn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eajttyiw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tgifukqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wmafzkni.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ycqqdcrb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iroxhkto.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zoduimmz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2czszrcay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qwwmqtsx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hmnkjinj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ciesxuni.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jujkqsrv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uuxgfcao.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zufwwqla.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ganodmnf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oixfrpia.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijpjjbxh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcrcdnfe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmfujsro.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xflevowp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlrekcmg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbaitlpa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbhbqvrj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znefkqgr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flldfxzr.html


<!-- 参考信息 -->