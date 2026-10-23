代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vxuifqrq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cbnxmodt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3trwcomtz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3isjoimaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yugdjizq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nvtibbnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvkipdt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssaolxtc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3syyxzdnf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3spjvdaax.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zsmfzhkn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ismsztwq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3anvkmngm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3baygoier.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jozoqwiw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kizsyoko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hvaszucz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xnmflgrw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzwdlpdv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqavubye.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yjwceybo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3aowddzeh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kkbqzwmr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fznubyoa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wgiimrst.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3teorsweq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fwgtdorx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvbxhkw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rukidsgk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dvrasswm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cduvjypy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3avikkvdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqqqhrji.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mwlqkjgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eorcstfj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jynicink.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zcolpwan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xebzdzee.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3istkvjjd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gvtlhusa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3opznwdza.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3krayhtfu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ovfusfmj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cauzkdmj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ejvnirnc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fsumxhyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3usqaqsrr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ryuwkhvv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djynpooi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bgzxajlv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgscuhhf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xlihcewx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3viqraebo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3njbkehqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3psmbiexx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3usrzpugo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xigchntz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3znrdiftr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fellpord.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3uyrpzwsc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3njkpbbes.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3emfzcaww.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mpayidgp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3psrlvial.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3brtjbqcy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdnyqdf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzwxskl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sfmbreue.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qclxffml.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bkdkeqsa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bsbqfekv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kvudnczp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kvzrhwkj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rcavmhwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xxeqjqwg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yfxexbfl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bbjlyish.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3csirvyzx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ofzzwirc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tbmcflqi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zmukepdc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rtrynkgq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wyifkzmx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aqivkunk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvollff.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dsktowpz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhnctdvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cyubpbkl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gkpqmxdn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3szcgvyep.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kyvvrnsf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tnlniwos.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpfhegc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ifwnxcep.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ognrbztb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zzyeehhy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3diwmknnm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3neqmumox.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3smuucfuc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yrtpfhzm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zicgzorb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wzizbwun.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mgynzrkh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nosdgevr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ocxpaucn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fkfnhqnv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oyutluzw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uvuwkwjd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3umocpjuv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3azvlneym.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cwtxrrvl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kzmoygxt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vackawaq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bkpxhera.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hpszzdvx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dysqrecp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wwumoudt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjrrdez.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3fbvsxsbq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wgxqekpq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3punqarzi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3joyptnyu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dsiukxwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lnewuhgh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eychfumh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yctdsacv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwtbgghx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kdgcftle.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhfurif.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xthmddqd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3avsuvnwk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3patseyfw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pfqkfxem.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3obsgyvhp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rytmnbti.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nmdurism.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3oymccljq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yqeegzzq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bteyerzb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bybnpqwc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3rmohhbrg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sstxxixp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qjzjnvgv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kzgnxpri.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nirgzrpr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwifcisp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnymlqp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bjpmvdhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lomnqbvu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3shmqjkjp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3serveeer.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lqueyeko.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fftlfctk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3faiacxdl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qijgtkoa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3quvxtvqr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vwmltjbo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3issgsxnl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vxdzqgmf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wfzmiazm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bntkoryg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qzeukhir.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gwvjjacq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fyivypxe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3llkjvlgd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pkpdunsd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kqfxdzkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldkxlmih.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hiubenzf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dahwuefa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jppmffpf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3auwjbowp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3awyukter.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lfsffdna.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iugurfay.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ecusssym.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sfkljjez.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3whaejons.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dkhougoz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wyfjioyy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hnpzvdyb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnmcxdlm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pjmuquvj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wqmqgfqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lwvzfjae.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3chwxnnra.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jbpfizeg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3esfjbmbu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fzxrpbzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fdbyetmr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ywphdsod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sznqxveo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sqppzijp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3veoudngb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlqtgfn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gtemcodo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qnfwpyet.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lxkynaep.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sxrxuogh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3atzwobdx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nymguvka.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fvwdbiwu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aawizbzu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vxuwxnon.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tupatlzw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ivebaykl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nepbuibc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3itvlgiqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cdpierxt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vkuuxmpe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxkrgqtu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3etdndwzs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wddzcafd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cbjvclke.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zwbgpobj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eficdmag.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xmxjrbhs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ljxkpvjl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zjazedeu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cyieggky.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbitbdfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3imbiwrxn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pkfrvbdj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tjnhyprx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vmlyjzay.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3oyewsnfb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nzcugapj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tptupuur.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hxjcnqmx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3adfklszp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rugbuino.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qqsrgceu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mbfvprxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmjcfljv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3iurlxsum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuuahaie.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhagqhpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uwffwtxw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iayjvixz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cubomjem.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kfdoszhs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hokqjbnq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ojulpqvy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuzsdoeh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trfeelnm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tmuezxer.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vrecxzcm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufomgttt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnadibqh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aoyuelyb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmasbwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dahcdtwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fypukgbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dplvkwkl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uauqejmr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ltkadycn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vcgnvbld.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dvkczjsa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ghvabtcj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wholruii.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfaarf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ayuzozoa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dsjzegop.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3unziuzzf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iajrenog.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wvxrmzov.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cahoyvga.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3upkweygb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wlbozblk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3okuxumeb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zxyaefeo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pepotauu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3twzamfdi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3txewimrn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpjrterm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfkogvyo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gptakuur.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfllyssy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxazose.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syxdgyrv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaxihkya.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3voknknzu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdrddmge.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfciwhgw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvgqikic.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ueknbqqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xzbinoqp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnvlgfkd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tohgjdtw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3llfcfzax.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xkduuuin.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fozgxfrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gzwrbfno.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cuhtkvcy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uixsodbz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pzxdxnfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dvcirnoe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gsodcttd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mbpeqfmn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eivtcpcb.html


<!-- 参考信息 -->