代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3izekniak.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dozkklpy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ishujvsd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uapadkgw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rjyblyer.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3vshqyesl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dialwphl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ymscdyba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3goytnpbk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lwkqdnol.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jfjyndlc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sgwxkufk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mrekvwmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rfhflvsy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3huyhhwkw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbzofzj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3juwfbrrn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uxcmlxem.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtwhffvi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3snqqouxh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fnuwkcmx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ifgbbrgo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bcqcvdfg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oegnezph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bqaidtas.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3afcvhpcv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vorgvccu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbbyigcf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ehqfwyue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ipkeumsr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yszifjyr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yeqomeme.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vtcslati.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tqsuthxa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oixvpjcb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwqxzxf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xulyvtlv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ootwbbxi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wdnllzbm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qeufojrw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aqbkthuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwbcdnpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dlsojdsw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qjjumwaf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3akfccmqg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ovnkhnau.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xmnbrxjs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iujdblop.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ukqegzqj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lmhxhlvd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zobjbecz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3siablxzd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jwcttxbh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jdnebuja.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ywflmuyl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pxzfioce.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zgtfsjaz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vlmtszhm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mlwpdvhj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sidbljtl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwksrlji.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clwrzfcr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tbsfjvlo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iasqklxh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tkvcqcbh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dwqydtbh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vzvoylhp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3krhaqhxn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zgqnmcic.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uhamwijo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3feicoveb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tcybrdue.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nkbmhwsc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vyieqgxz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3lehjkyaq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3evbhztqr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ihcuuqvf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3guedkxxf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3keajmdgk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmdpwvq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkrqrbpc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yhveuytb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3evtegjvf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrlihyne.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eelvpjiw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xuyfqfpz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qdlkhahl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fkrwxgbr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3aoykcsmv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3trtkoozq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3oswbecfk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnjxptep.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oboplrhv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xevjiktl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qybouljp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hegpafnz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjafntq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wwfsiwgx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kdxkputd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfilgmiu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isrhofry.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjfcolfi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qlbdiaza.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3peomudcf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wdbkxlgq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qwqsyakc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zamttkci.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqoujfd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rovycjhn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3olsjbwyc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gahcwedu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gjtkrxjj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tgpinaji.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ysrgwrze.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvlugaf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opvmuyxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olmupfhg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dfhxnlfq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qemxxeol.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hdvlsoyf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tpsegqmg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3venrzvxt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ukcmjpyj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ryryticx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmqsvymw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3elaqsjcp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3piortdpn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3guxyihet.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bjkawvgg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ouzpoasg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gkvfpjcn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tqybirbf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jtuyzyhj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xubhmfdy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ldbeyjdh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jauplfrr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3srwlnhfh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3oanqrafn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xcnxyqxi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3awrasfux.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3toexfkgf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wynrpvuq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dtfiaxrg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mkmzuspg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xuhtpnov.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3llxboscx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bhsvtnir.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nswmxziz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rajohnkn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3joscdlon.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nxilpvep.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3medpmkcd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oawgixar.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wucbxytv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yehmroxe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cxhjgntp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3onbgxogu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmggzoyo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3msvsnufr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pufmvsyw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qaufafap.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yyazgfgm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tdpophpa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bzhwtpqk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zhwkjtzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3habfqltd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jetapoxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heuxronk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivyfxsmb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mwjfnzul.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3atuublcv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xwxthcdq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bdphfwzm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mcvokwcd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ykgtvfut.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwklhtbx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3usvhlkie.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jznfznkk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qdosdsdw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cfoldzwi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tfsyawya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luspjohl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rverjgtw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjviwtkm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wewsqtbn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ztfnhzby.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lprvnzln.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pwmgqcqi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hldkputc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hoyfomkp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zsardtdq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3horhpuow.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3idunyfuw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kubvrwvd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mcpucmci.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxqhjdqk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nwmkspll.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lveyewyz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qftekior.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ntykvryr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tuhfbfxt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3atdgvtvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yyacflgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3entbjpar.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ugzqgzah.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vccocsbi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khgmeqvi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afwfcynm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqatwgfo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyohcejn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pwxmspxf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxraavll.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3issfunky.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hyrpjrfu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjpcpevz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmdcnhdf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jauopdyu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uncozsfb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ydiygbaw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvmjdysz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fustnund.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffffiwam.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hmkgbpye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmhnwcr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hlgadyja.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dmtgiblr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3erdqiljy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yevvvjno.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdhylii.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dhenlrbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3udbajxwy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tqhyljng.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lyrnpjqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lwhzebpb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ecjqilms.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vrpokjdr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdaoyzu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qybigcug.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbgiybut.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqjpngwe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3eijvxbav.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlxpqblc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hesbuyzs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bejfohpe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jkdhlumc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3brdsxjhu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zbidoywk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzpugqnd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3iuqrfvdq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zdujpaoa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynrgyilj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3linbavvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frirvyrx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjlrvpra.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iisuwkgy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eixaobqd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmjouuhe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqkijdia.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ksjzwidc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3adycrgia.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3egvdlgou.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3faxsdysr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbuoxqgp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3apmgjxeq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ossniuxu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfvwerz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xvpziosp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vuyrwigq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ruufqsvh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kamsicqe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fzyphoms.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ikkygksw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sgvezwgd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xyjffndh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3omfvwpmu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cniymnvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdjmudde.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zzrjuvkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgwuortb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uyqyfglf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bikeenbp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzrfeayb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dcghvfxp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uojvcisy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3saycujhf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uadsskhe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3spvihuwb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lsxmsxlf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzsqsebh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfmtnu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lovlymal.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dpdaldex.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hzoxsxtv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yeivgcxa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxadecfc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nddkovqd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xytlwqyj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zveugjuw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vakmxaij.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gwncehnv.html


<!-- 参考信息 -->