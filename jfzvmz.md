代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3oscojxlg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3amvmqjcy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wqlvueqz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qjtpphvo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kqqwtcum.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3clovvlhd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ecjeilwl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jkpzjwnm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3otzkmuky.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3raehlqwj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3neyzyetc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nevggomu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3eovzeoyr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3udyabjbe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3etavpicz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zlebdulp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3sygkugho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ythbttob.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpqvlyzu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qimicskm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vkdpoehw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulinzsmk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mysexxnu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xqwbgtiv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwckegv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ykgqdhhg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rfxnggrm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3owpncayl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smxtxabq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tphejupi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqnqlzun.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3osurzfue.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dokcsbwb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ylsipcoy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3huvvtbwq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zotiulnk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zuytdrus.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pjfmtrjx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zjphmxlz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trnxpsut.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxgmzhae.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dvjdhzaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sixrjeey.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ftujevqp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qwaoruxr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwgnarv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tcffpzmk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fdoplwsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qlviozsz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ugeeaanb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qabcomzx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pkqmyvhc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrclath.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qomdhida.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3djtndapo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yfgrikhh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hqaqnjhx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gidqapbq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hbwbjuum.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3awkewptu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dsferkft.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3htpulqha.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzdrocq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eqzwvlsz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3evvwmwpm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qfohkscb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqucqct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fyvvhfph.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rjmbricc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qwhlbfst.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qnmdgtqz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qasbpucu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3detdhfgc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pltgllnk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mbdebwhu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cwlfcacf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vngbgrys.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlhtmyio.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhdvahno.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3byvwioyx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sutcwrhq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dydchzag.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tvfsfyun.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qcaaaita.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sckazbxf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3gkhkvxbj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3imkqnhnz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3debdcyyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fugodcfc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ajfdelzj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lmnaeaxi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymapywov.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vttbprcs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoxeuch.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3voonoyvc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fpzgbycm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pivkfbho.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3axpvuaml.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ctcnspki.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ezbbqczp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ubkrkhtq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wvensabe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ticsyeim.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ffwvosoq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dwxtygme.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxnvntic.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3asqvtzqy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3crhhutpc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pqrclbvp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rtzokltq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3omaomgne.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sidhbtbl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lnkhyebh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tkldozhq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rikgbikn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hsxiokzq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ysnyohjh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kbikgrat.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jhxpzebe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jijbpwae.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wdfvxuld.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3knuochkl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3shhdxvno.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxfmmsya.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zdtespda.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zkphrwad.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmanyey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3phoobbhi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gerotsph.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tzmjqvci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dzifjamj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3szadzdmq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kohrxsri.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztrbilol.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lzdpalox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xalapqck.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3krtfllzi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzenrkzi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bftkqemi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3msrxwcze.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sdadabtl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zwzsozea.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qeingbxw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxbsxped.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrntoad.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ntlvvaap.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bcitwhnv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kiinehqe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nuanypkc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xucbyslx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aecopezr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjhxbua.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3afwtbrfg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iddmhxkm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xefqlohy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3epkpxils.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3plfcqxpq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dmznhkhc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3umdzbuwr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ojiexjcl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3trijxvxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lxwnaelv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sigclsmv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3votjqfqq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sihndmdd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hrunfwkt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kootenlx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jotietiv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ovrfgaqh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gypiwzqf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mbcgbceq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3byclddin.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bptbnhpw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwwlwfpj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vndqxizl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zftrmgow.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3aiqtcskf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3madfkugp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aisyscrk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdqxmnis.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsaitnh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gvlvsrkl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xbgajftx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3loezwzon.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3akfyzacv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gbxizwlv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ceozyxot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zzilxyep.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kauwnprw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnrwafwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfyognp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqoagv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uovrabdw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sleyeclz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmanas.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kdolxziv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzmcbcxl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ekarneze.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oasqgnoh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hsakxrfy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yezmxaeb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sntjzpca.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jfznjvrj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vjzmsafj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3giggiutd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3keobanbn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hodlxbxt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdgwnltu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3grwsttfx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fklnhhiu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkjfztzw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jgwxzkjz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bkysauoc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvpcttrf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3athkikde.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yttrkwmz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hxqvjngr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wxwwsjut.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kcgokzjd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iczdzmnx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bawbdfjk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3saxdpfrm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmdijp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fawjfrov.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xfhlbmhb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3twubiran.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mzssfwye.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmzlxmgd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sbrcvorj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvakwtuq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sonneexb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxmhckqi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pbokccgb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3iqjhveey.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gemmwdvb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uvhyfmsi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uefvwymu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mbwiyzyw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mceujdxd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klwarsjy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hdgwfyfq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zklpdogi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vwklnygk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gblmeaqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xqvwzjey.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcbkidqa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcynrgb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvvtote.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3knnrdvse.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3agnwpord.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3scgqacji.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ayqniauo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hflgtrtv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ikfhyjev.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3npombubw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bivcpdqa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nmhsmkqf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dxrcyqpv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wurtihsg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3txezloet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3svtwlzwi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rgrttdpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kfgmtelq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yxxsbkwd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3anfapvab.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3izrhmpjd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yofywmgw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zaryewik.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3odjnwjji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3exgfpmro.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bgarhati.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oerclszz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfpijfim.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3psclaxds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dekwvjwg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oasztqpk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhhsqeyb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xmxbidxx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqacvhgz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxfvyurr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yibljmdl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdlrwaxy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfulfbmb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmaykhwj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfthxqhc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zdckbgvc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3trdswmmt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pjgvrlbf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3azvdbqic.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wyeugvfi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3finmvffn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3accfrqzu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrzcnoa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3chxbfkaq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pavzshyg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3weutjznx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uwfmpopf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qphzcyol.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vaybwwih.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zizhwsih.html


<!-- 参考信息 -->