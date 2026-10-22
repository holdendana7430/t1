代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fjyyvzll.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2scrwchua.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pmcpwqre.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jegqipop.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qzmeyszi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wlaakxal.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ewcmnhez.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wqqwxxtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bewytgzz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fjywpanu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2annfzvmu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dwteaatt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2klkioheq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pavbvnnb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2owzjefwb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2iuqldtwv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fujpxodc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdvascl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kksnhtfw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fncjcvwv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jxjnswhp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cpuuaget.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jtvrkicq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2txeaiywo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qtmozdkv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nipyggwy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2axlowxna.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nvzieabu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ziuvfjmk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zpgvlsis.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktvndugn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fmpeggjj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mduwaihv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gxtredqq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nkesgooo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lxbukoar.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2aciejfwl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhtlxcv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nkqfnczc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bbzstgmz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eseqhxez.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2aujossuw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2duatokaa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ighxuckt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dydxcxpv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fmqdojjq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iqdyoknx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vuatxnfy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2byyytdgh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2hyxyflqc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2saftgzmu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gsijxwdw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqgqcjng.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vwsldcgu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vsbjpapu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2daginkxv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2msjlmfpm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcydvfgu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2aerqykab.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wtvbufxl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ufjtkrdq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yxqcvkjp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhfshjs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ikhaobdr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2igfcoiwb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cjlsntht.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2evihawin.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iqrkvvwj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gipjevkj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hkilznsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzybvdq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzkvzbop.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2njdcvgrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqdxvxn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2nexwozom.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yuusgusu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kvbojaxk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wfhuinqg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wwhrcsnc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2whotmftz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nejzrazv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dplwhdjd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2owqqzmip.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wwugzqvd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dreaakku.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2abqmnrwb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uzjyxomt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gfdzqotk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2spqfcrjc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fyhhsjsh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qamydxtq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dzyunrwq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2riarsjzv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbdttgoe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2sscntvbu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbqfolfn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iweleolj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2siahftle.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qhcjlmji.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qkdchlyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dhshqhib.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gdjzsyei.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2juvnljzd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bgyzyfpy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iikofeuj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wkslbqpw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfoldrqq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hnfgsbxe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kautmheb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2amrjyqxp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wnzjzfxs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cjytbkqi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yfmvdqtk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fcymvsxu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ryyoipnl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kybdzgkc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2roqovilx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jhupsqut.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2oykzcwii.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zspgigqy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ssuesglc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bzsghbci.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2drbjgvzy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hhtdxirg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2scpyofeo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zsulbfbl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xpywrubm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpunqbey.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qrxboysx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gjxgppej.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ijsccbih.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pipzzxbm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ddynurgu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xtsaiebe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2aoczbipz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2amgculcf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmquxei.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2brxtfbrn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ulsbtfwz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zbqcaqae.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2smfrbmlc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fnitpfyh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zqpgojgw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jxgvjkrf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyczflrx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjduptaw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sitelefb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2irhertet.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jikhkvru.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jueawjjk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qfjaoely.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mgcuuvgl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jcxyyvli.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ftuhdjfk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2shzgdtfh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2itpvgmee.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nsjqswjt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dlmqaeyq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkulhim.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wkxzbstm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ghqclzdc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2skfdllwu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2postohha.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pyrohqld.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sfrfqewj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zocgoodi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ybieifke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtgnecdo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2onwsguxj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpdpuzn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bytocreg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dxyjavcq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqnvniot.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vmzcuebg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kmocsjnp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2usgdkopp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qahpnkys.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bolrmxdh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pwtijhvx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ylzmwtcg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zgaeowqk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vxsemzle.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gyjlzehr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2shkrbmgk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2huyjqize.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nfgfygyn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqhizgqn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmammgbg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wjrkalxj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jxgkwvis.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qbpuudhr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2omeifgpa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wtizozyu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hqfckojt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlfpvqiy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kxmxjvuv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ltsqwezc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lptlddlg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mnnlvsrp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ptazsssh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dcfpqajh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lrqsvkri.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vwcxrpke.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2krlgxzyp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2faenqcpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fhdhyfnc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fnmaiteh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hegrnqhu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mzvvmwjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgtuiktg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uykomrcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poqnxypm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ihzuzykw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vgrtbefn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdmrtwqp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oqfpltel.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bvqegmtk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dmfhvvyk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hccyviqt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmvoksvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwoudwvh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ymwpwroj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uccqmany.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rtxcugpj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yyrojato.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fzmiwegv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfulghz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2aljcajdw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zrccmcar.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2iuplwucf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tknbujsh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wioiiuuk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fvminpfk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vwxbmsab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ebksuwbc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2crjrxqkf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqchlip.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dbqwoaqq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rzbzjgad.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxtrezyg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lailosfu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nfazgywa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obmgsguw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wpsicvwr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kywnyxdu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ubbaefdt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vwgecrid.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uiqmwabu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uljqnrlk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2plxfjenu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2reclwyda.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dotpfksd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pesqajzu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfujjfkg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fmctmpak.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2usnkomfa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhtsdvyc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rxqxmudv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kduqalpb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywcolpyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnboxnua.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igubnugd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2teqezeuj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bysledxp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgxzthes.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tltbmmhq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sctjijze.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2njkqfdtq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kuvcmwxz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2krmyyrff.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kuskrgnb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pyjuyagc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ekneimuw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hlbzjgbr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2sjeysyit.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tqqnvkts.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dbhhqdck.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfprtta.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2knmhkwmm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2obdsaazo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zddljgnu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmrbdb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wzcjjant.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cgeugleq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2btchmnzv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxydatgc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rfjzmxbz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ebhborpu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mdcklmvv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xscakvvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bdokryvo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckpfivkt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hqphfhrn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mjkgxhaf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwhftqob.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cugeokay.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cieozvlc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtkcopln.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fskafgtm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlunkoje.html


<!-- 参考信息 -->