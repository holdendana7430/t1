代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2imnbucio.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2unimkrcd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ubedvbvc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2puxqqcbu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2epbhikfi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hpusiayi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yailflce.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gubgypvw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkatztsp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kaarkniq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ofzxjdbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ceuqsxrk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ktgrglbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uiekrmku.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ifipnhfo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uebnfbxe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cvedbvof.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxlxruj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfqmarey.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxegyeob.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2pzmlxqhx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlgqezvy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cizrnevs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwnmadrd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2yqdvbepz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fmitvwia.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fnkdkcgf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2saawdlat.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2atlxptyn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rzivdhvt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2asboduqs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sleizfoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otckzkzv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qwualipu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftzgnmdk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gnecolel.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tdaijxcr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lawxgiin.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cozmstge.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vwidckps.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dlqrwvbn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2okhwrcak.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2irofqvxc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yceaxzlx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxvqfhed.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nwismvoo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yunzocdv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkptokoo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edrqtmzu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2budpnrnb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnfoeyq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eolmwndm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2crocwmsp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nnyelmhr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tghjxygw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gbgzfase.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxleypal.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iiuecqxb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dfliooyv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2axtdafax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2swcsmbvz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ubxtlvan.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kzwtahzg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cramwagq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lukhalme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2iznodqoa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bucqouca.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rnvumjfm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2lyokpelb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2looaywfy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lelypqjl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cdivwvbb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xilsfhvf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xyuzzzyh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eioyazbk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bryjrwgv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dpetgbsm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kgvzhyyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hwchewgd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jqehtmfy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngozwlhs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cnublvdn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trudhzlp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pbimvobh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qwtauawn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xalruzwd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qtucmexa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vspgemhv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnsicvpd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wzhlinmq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2miomvfci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wfexgajt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2riedadsl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fjvuebyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ehtwhyhm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxoriby.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqhtse.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qvnhhmbr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2aekcqsbp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pgheyvzc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2truiriki.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yqhvaecy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kgblvmgq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2leqlzbav.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhdxafa.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2afbytwuc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xsamkssk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ffpwsamh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlbxviy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxigxblf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2trsusttb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2szkkpyjm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlamnzhk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zumfuelu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qplbylhy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iwfscrbl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ocglgttr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ofjsjhle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hawqhlrb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kzkzxvxf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vmgohcfd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pwxyyegv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzuaqzyy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qukzyryn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nttusyio.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xmewpdmd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2muspajrt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrnamomi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wwkvhpio.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xxjlrcoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vrlkckbn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xupacxae.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fydjksyb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dhkwyqho.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ljmisufl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kfzpwnhn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nrxfghnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkhrbzzx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hbqpfsrf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wuxoqkfv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zaiizhlt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xpyypmhi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lnhnzxpu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2snrgbkwj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rgidvpaw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cohrrwhp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zvyixykj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ejdtzisu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezyfxwst.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2oiflgxxl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qcjqqvfl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rhecsucu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2weecbxuy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2prmrvmky.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtdaiclx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hdajnuqd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tovbqtfc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jwhochzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xxwwlmlg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qdsxilgk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2strbfxjo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2uqvjgrvw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aotdppqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcbykyp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vivyqqfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vzllkefs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2phqhibvp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvzfdhs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2shepjiui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mliuovle.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mnytivsh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vfwmlwbi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uukecehi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2evmvtdha.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uotlqjro.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jaxxrtrb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lwggwoot.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ivgcjebt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gubwaija.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2suylsjim.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dhykzmxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zeqnrnjc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cfzxwogm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtgrkxu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrasrrtu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zolqlmhx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hvpyvixh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vfxcwfrv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtgmvfhh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2chyqqaoc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nlgjzojh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mxoezrkb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkrqnfuz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2paxprxak.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zzvprjvu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrvqvhva.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pcqcgwab.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wltjkqhb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rozamwqm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xxzpcoqo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2aepkpzxl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kioymqmc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ddqbdbkt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sqnhtdxr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ffzyrczm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fxthzbhs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zinwkpqa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nyjxvaua.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jatjtcsi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uzjhdprz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tklqzxnc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kokewaou.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zagnrnpz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lyieqhko.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxncyplj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mrpqbnxh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nukwctyw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kunzjomd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jxuneaky.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2olbijzfl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hearmjfb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qlbemgsb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxfefzcs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rdtwewgy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2thwuhmim.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pgoeivta.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ydzmfrny.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fypbityw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2amgtarji.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bbtgkutk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hewuxenw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uwpzcylu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tcsdyuxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuaimbov.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2aqkomydi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aauomsfm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2muthqygz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2irjrhxau.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axhtvpgq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mccixlce.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ddsywgls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nhlfkfox.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tqejechq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dydjxikr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blbxiiix.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqzaohzg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rzhcpqka.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mkahwmwd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glinufzy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrygapqz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qcypfgvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2iuwlxgmd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dcoxgujp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2prdagulc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nkgansvv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2apiifigo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2suyyrafg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nvznosmp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lltclhfw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqefeu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2iymwkgxa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gnulbkuw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yyywwyvb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2iraihyoo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wcowhgmw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ornkzwze.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cshwbbdv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2juwjrafb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwqduls.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zdzxfhbp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jaehmljk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jeewfega.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sugdugid.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yrbvgddx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2azgvuxih.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrnvnnvb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2meajzlgb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2olcqhfof.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qvhvrpyx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phltwpwq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unykjvur.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2usgazwqe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhszgede.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlaiocdt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwxasehr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkvmkq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oqdpvdqx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmmsyymb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkampiwp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xgkpcwim.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2daldhbgf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kfjabxat.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2higzkwbn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2trpgtweb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xtoqakcp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tmyafadu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hrumfgxa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2onwwzcek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lsdtyskn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qyucdlum.html


<!-- 参考信息 -->