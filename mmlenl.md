代发 wailian999

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uhetlqrr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2biigydka.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ztdauwuq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2icbrcrxg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2trylbwxq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2prtenbah.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnmpaxwc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rgpnsimq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2helfknjb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ivnmwnxb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wvpclkwz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnmrsopd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2inhwqyqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dffntzzn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nwfwhxfo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mktwdkxz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2utshnycj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dpbmvuoq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2csjbuxhh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hemtivrj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jkbintpz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ssfhlgjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyzxfear.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2acpdtkit.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2exrinzun.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tektwgyk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2spzozmiv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zclrltoa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pwuyuhtm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2owlrdwfr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gwkznqvm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbyfyavj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jledsykr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lmbfgvyy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpjranhc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ulukoevc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zobfjhhr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kspjyhna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccuatwin.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2auwjthut.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sttxnntj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lhhashhd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kewaqjcx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awlomlzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kgocagkl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhogsxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hafmlfms.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrkgffpf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pdmeyyhz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hbjvwvlr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsaqmsu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovndcaew.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2puszacro.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2izkcdezv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2htqbpzza.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2afwojnjt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2aevjzyeq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wsxhwtxq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ltebpdse.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mspfxrcp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gkwuaxpu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bukkyuey.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pplkpygt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rxjhtjxi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uqlroivz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tvbhkano.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fgvpcreh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kjsbsfew.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pejhweuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnaiurz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mfanhqjq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fyttlqsa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hqdbilzd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2osxbhtff.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqsfcell.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2aetuoreh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2iesflrxo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ggflhfnh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bmujahqc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uijqkgut.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2evgwnsrm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sruxpvjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sgxdadse.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ewiievre.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2srzcwjxh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zumctuyr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yvajtouq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wopncirh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vhykcxvc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jrcbfmiu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2atyuxdrl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rgpqkyga.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ghshzjyc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bajvroca.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ovyofkzg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sggdilyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cygrgzdb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hhqsonuo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hslaxngc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mgpqhjab.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2szjdjabr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ijnybqos.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xnjtgscr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vtknbyjf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hmcbcerd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jelygwlg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nzzkxrhe.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wcgeoqjy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jmtawqez.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cawfbhck.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lkbqsxiy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ixwkyhag.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2acsxnaed.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zefpxzly.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2olkmjgep.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iagparez.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cqlpiigl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2eforefzk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2utoezrpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2frbocvky.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gdldptra.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dwbgtbdf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ynxqyqul.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xrydqrqq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bdnhsekq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tqridgvg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ueiziefa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkjfnxw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jikfqtfs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vuneqrld.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2navsoxvz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kgbgeavn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjeydzz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hypyhjbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgombuwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hkdzjcia.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lnpaprqz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fibhgavt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qzeizhcr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hcldhzqu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fvycfbmy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rnsrpnpb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wvpvtked.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mjaugfip.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kpzxkhui.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rshsrpwa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dymcbkgv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2txlsnwxc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xcqccesp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2smptzvzn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kkzpyrhu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ujmxcvni.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2krelojpb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xzurqrmx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cydspzxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2glumgffn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wlyfrzmu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2whdutgcm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nflolyyu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tsscookx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnekuliw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gqxaymvt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hoitiqkv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vaqyrwyg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zybfqcaz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kygynqcw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzlaygdt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mubtkcon.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nqbqhvrn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ljmjvtlr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2iwtydnoq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwifjahq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nbbrfkjx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmouxhsn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cjjrqejm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kiznpels.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bgjrewzw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2paoyyxdm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwycfvl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fxznwvgo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hynrspsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2avkdjeub.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mqvqzuhb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qfiqhqlx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xhsftavz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bclqfonp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrnmivwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iriwfkxn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grgtwozl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jxxdrtax.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2shydzbmf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lswwkhwi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ynnikjjv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cwatvuil.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfrmycy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2afkfvkye.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rojpbaog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pefovhge.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rctepxpn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2feziiviu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqeslkby.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rqpjyyar.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yffgxfxp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcxvscmb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvdbuwb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pkkfouyd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wrgaquyx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ufzwntso.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vzrpumom.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2utugfqec.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qyijqoak.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cvriapsn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vmbivqha.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rpmyysjo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxnogjdk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpvsdhto.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hrndyhky.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dghgaaex.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jidteaei.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jizlvfbv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2idihngcp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2buprxopn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wnhcavlh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ucxgarma.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vmghzref.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fayliiwc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vlultybk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqeehvsw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2blcwidnz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hqgrtbnu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2okqcoanw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgqefvzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mawqrfbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pgcfybzi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gfqxygtv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eaqjfqsj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2olrifncy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyhjdshq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wsjacast.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aokemwce.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ojrfhdny.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yjonrguf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlqzatln.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gecuxdkb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aallcrue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgdonolw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2laxolziz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2beqbhrnm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vurkwjws.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufxegunw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jvteurvh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ppvpdaxm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fgvtwzit.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlvdilne.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zshigyej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hadsyuia.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xpcmbgej.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tyntvqjv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2muqpjhwt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2asveqmvs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2misyuaxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2saosqpjf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kjyuwcub.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2abovnztt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rfjsfykx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ohpnvaly.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hjxecmxy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkarcnga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ggrrbtqs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvrgoy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdnuht.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ukyaxqmb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ajnexgwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqvtrvlr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mydxsuas.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jnfbqgqj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2arwnihof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kymqblys.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wlqsfzij.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfxamkia.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vitinjmx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uopvyrvg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2unwpepcu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjoinquy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyvzybrz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhiuacbd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhbnfpku.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbcnhwgk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vluxpprq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwwjsr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sdlmbwwb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnllfkp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozwjmbdl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jyefumje.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vdlhqqkf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wszzxton.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nferreim.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cigayzdd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nwycqscu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ywcgsofc.html


<!-- 参考信息 -->