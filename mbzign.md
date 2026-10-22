代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2htvbqsxv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uyiuyqbl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ynzcdlwd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mdcqyzvs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cmhejolt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2whureugw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oevlsgsm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ddallxqe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mbmrwvsd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nifpduyk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zawrtawm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qkixlhbh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qgiurvqe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qrentwbo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lmxazuxb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nuqmgxcz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zofkxliy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wyxsrpvl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2elmrevum.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2otwpcmjn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2atwtaxzh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ioaidill.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2arbqrigf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lnlfdbfl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pubaqoup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rbxerjww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qjoghaxg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jheduozn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cpxzjkcy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xjpjrcul.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkoozsin.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2skpccvvw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrunivb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hkoubycg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gfrwimap.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xogpqkpw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ndcsuksl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2mhtmnfsi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vkewyguw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmlnymms.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2buyvummv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nsxtaamw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2dwtfgmtk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2avdqjcru.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gjkrrxkt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gunwiobz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oxuiobmg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2haxcuzrp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sdpwktav.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xmceihwu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dlzxbpqi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dbhxauyg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jrfbcfyn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fkagghwp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2llvoxfyf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kgthihii.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wylthbyb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfahxjcn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nyatirke.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvfeustl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjohitn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fsnghyyc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bgomsqqq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ksrfengj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rzealdoe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zsdicbce.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2daotounj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nmsoovjb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ilsuxbzn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ycqzrvdb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbzteolx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eptkgbhy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2okazvyyv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xbrindde.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oyrdmdtd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2erruxayl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cadaibqa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bvjwhnif.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2fwedkatp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pehelojs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fblyoazn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2grhhywby.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ybngtpvp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ledoyjao.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tofwqklm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2coxpvshb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vetvsijn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tpqrcqfh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hkzwwpdk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijcnozza.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lfizrxma.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gmuvvwsr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jxijfjgu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsmoldpx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qtzsuzns.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahckebvm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqhqhxsc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmyokaag.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nswdiisi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wmcsexwm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hrnfhobu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fqtzarry.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xdptxgpr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zxzardvg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2diidhbrw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmrdcpf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2srkzccdm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2imwkajhp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2badhygqk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kgjmlfha.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nxzapfnl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aohgmgha.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dolmdzkt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ufcjdzbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qcnoqtdm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyreqmaf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qmkjoyyu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2baemgwjm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ocpxcgzb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nahexzwb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lutlusee.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vnyeehfw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iigahzwa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nulnbcpg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2abbnxrpw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gfruzgzh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwfvkhm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wjwrqffk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mvdrcauy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kdfxaawd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mxjqbjem.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2unyejwck.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smkenkvt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2udggytvp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lyneqjzm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aoldcqfo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uohndvwg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qselnped.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fumnblxm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oteenhaf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vnxfajrq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uknikugj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vfphfksm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tdjzjyon.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rwhfrqno.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rtcktqye.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uppjrdkl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fjogouie.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzyzweoe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfusnhp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ixzrowtf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ibmvnawg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wstdrrqn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ddbitiop.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mzzmtcgc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2otbsmafh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aclhsgyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdzsaogh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmrzbesf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jalmwebc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mdjnqyxn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dzgfdmvm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlyaorxs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bqzgqrxk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2akxmuqjt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ahswfeyr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ahvetstm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wfwlcbev.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zkcamkct.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nmeuiyxw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ecpawcuy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ovuuktjs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xlabzjop.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfascwm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zgebnbis.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gllcqrwz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujvcjgbk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ejmomtod.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bnimexbh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cikarsqn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dqvwscmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euefpbfv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2innibhco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwrupiul.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqvzrqnv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2itfcrtjo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsebywgo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mbcofpik.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2phdqpwpp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2znhdklmx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qihbaolw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzqxcstx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nibrrwsx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqibgzwb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uzbhpphl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqlsxxk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quihfwkb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2krjhjpue.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pabudvst.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fsymukzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jnrnshki.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hotjeoqx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gtkceibj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tcfearfs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nvxxgluk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xyqlxlmi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2stgdlwci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tduhwlce.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jedkjlzq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2brwhzstc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nadeugnh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldmxufhg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uygtzwyp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2obgwnyyj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fujootrr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ajrkwdsx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2odtewufe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iumdqbud.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2meqazrxy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dllwycbv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ehxxvunh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2eqvnczis.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wixmauqs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqumhach.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uefjrqup.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vtjwfagk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yrhzkcie.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nxzcuaeo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feffjofk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ypwziioj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lymxquqz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qlmlkmqi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrkdnkm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aavrlfdn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfnstdmd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edombfiu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jocqkdgb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eculngzj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2trvcdaxn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iarwdvle.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yxphudwi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kirttzji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ojghpbdi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilgzrpuw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2osfojpkc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jswrufgk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ijolxdvn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2llrpgifb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hrsdmuqh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dyukqpun.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mhddpkcw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtilsfmp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjkbruj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mawvaopv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2byfgfoik.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xgbiubyd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rmezggzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkjlxjpw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vepddmhm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ahfzmavg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2brghjnzh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2edystsyh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2urgpqjex.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opslrqle.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2juozddee.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tgqavbhr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnbraaew.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hczbzmhi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmxsxlom.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcejqtvu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eostvcvo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjacavnt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hykrtlhx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtryugvt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dlgwvwpu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmpzaoca.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjrseafa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcbkclzd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sujscszz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2klvooece.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vyebrvfc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cipztfqa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yvahkkxp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zscsyyqc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ajlqupvv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oflcbify.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uptbxgqf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lusmuzvo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rmjxvpuy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2njsquffi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gvraelam.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qjyvlfpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlfagial.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dremfqwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzgvmurs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rxsozuce.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nngjlosj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgqvhaxt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2srqrvoos.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwnlpthz.html


<!-- 参考信息 -->