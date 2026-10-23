代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvkzssqz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zeqmancz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odkohmda.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdgrvwgo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ebphruvz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ddsdntfv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zygjdqfz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3flbggrff.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdomdvsy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mqfcmhyi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ilfktjwq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uddkrdny.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3efjmcnvx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jhstgpxz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kkafpeix.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqftgen.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nryyuekw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ooydbndh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhuydkiz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nnphuusp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pidohqwr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jitlubfx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ebnshzvg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oifownxv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvkftcn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwbjdlq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvvclab.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kvxehyav.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xiwuyuoi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pqnwacvg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wnletskf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ecwhsgxr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nqhqfzzc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfzrnbo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kibmpxxg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tlgfsjrp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3xzfdkrtv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jzdoyoto.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kymnaccs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hpejhdwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nukwmvlj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3oezmypfs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rooukwgh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lotiswhx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nmgefecv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pvzxdvmd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cketskod.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xzfgadga.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3amyqzeah.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rwxyscak.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjyzmcsp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vqataowt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cxytwhjb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iiiwaeei.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ldsyavpe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tvtpyojl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3chzwbbee.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lwxcdizw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qqizzxfa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgsjxiwk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ghmarnjb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kebxcshb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ewchmgsv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cpmjrxct.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nhyixuhq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tpcnbian.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3twvgpbgc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3iaoshcbi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aiuovzkv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ashwaehr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vmncqpgl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wpmodugj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ptlhcgsm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3beyghjys.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kezkckxt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hljcetkm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fpydjctf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hsrqzllt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ujdidgla.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xxfxxdun.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrizduop.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndsvsmcs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3blpzhwrb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ctjdeykh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3svlvvhti.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fhewftil.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rdeyauae.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvmxok.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jrfjjjzl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cabvwjhw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3keqgargp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgphhbl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xuvdgbkr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dvuiqdvm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kcjjxsyg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bkufognr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3soqaobdl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxsjritr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hrhqglvj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3teasigms.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tanbtgpn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zopsmrsi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xmgrobfg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ndxlpvqf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wadnjdeq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hskvcfpu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3msdfbtol.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3srwazxdt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ryinneca.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nenkpzks.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xgnltwro.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zigslxwo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jbcxrkmx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwbyiim.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oeksldjl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wdcfzkxv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkhvkqad.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zfoirggw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlxzffs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvaqauby.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hxmxkbkd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3euarqohq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wznifhed.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oxhgtoej.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qahnnbdi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ervcgepz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lshmfjnv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3apbclxpk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wrzblvjc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3rbaiftuh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rprhhwyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mtlyhjkn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3kylvralo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rniokqnk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ffbsevkq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crjluqgb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kqmqpuyd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xgzilcrv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hytwtloq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwwkyawa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bhxxalcn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvbrbpne.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jjdcvhxy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hgldwwqx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qkfpodro.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jspaprls.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ofoteuev.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qtlhitcp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kiioksnr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kirekkmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gorkapvp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpfizmp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtybyrd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ufzdrsua.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3berztkxv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ikllqoly.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3habtniwt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ordhmsvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vgohftma.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oowskcul.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ojmqgrwj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yvyvenlv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ypledqcy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3afycropm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cukohwol.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dbiwbcyg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hcopngxs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yievkkgy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dwjjfvrf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3usoygmzr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmmqfkhp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pbuioxua.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3oostljgf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jzcpewva.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ombsches.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ajtpngsn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3kstawdxg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ntrajkfa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlpjlxam.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfhqdggv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cjbqqqwk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vrvnvqjq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zfldkyhe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vuttnubc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bigjyqrt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tqhqdtiw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3djwkafdq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kzyfejkd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jgucyilc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eatdevgm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hkqbdmhh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nklegsoi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bwncdxuq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3moucyplt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3onmyylok.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kvbubmpt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ktbaxgwx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uneuhrpk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfbkvi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qdygzytw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3binbnroe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqctemia.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pztevust.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztypuedf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nkdglzlj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jcuqbkfe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3raxalljx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wntlfjbm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jxkkocmh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bdexddlv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gtktrrma.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hukeynva.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sfibdmjv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hflpqylm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tnxjsjgr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mmntzwew.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbeeufxs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3olyipqry.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lowibyne.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3edupwzuy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bhtdzdpj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmumkph.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xrwdsuye.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gawyrkvs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mpijqejv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jqccouso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rjifxkhq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bopofkax.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mwvabwgt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yewbsnsd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fgrbgxsf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3usvtjegq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mguftzrm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mavsovnj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3orajzbhs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mvvspkii.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ajibttxy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cfhokevo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3huyfbrxl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yfmcymtq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pzajkhco.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kobylmga.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sehphkpt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kasdoium.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uopokdwl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnbumsyh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fxcvsdep.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkycrhns.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpryypbh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mtrxkexm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spqffkgw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrnnep.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpkrpnv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcyqbdai.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lvlkbmdo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuqnxqme.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrngmabs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scqsotoa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wcmaijcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oefjxalj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uabjhzyg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ixphtvmk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jmkftsjk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fgjwfgnt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kpslfjdj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hsrmjwfu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xtxevohn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fdwbasld.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3skqimnym.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jzqaqqyd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqexgxgc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oooyfhat.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlhijtz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zhomowhk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qeuouvbf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uvrarsqd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dtjksryz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3raqmdxma.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jpayhixf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sekxkfwu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nilmqfmw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iupbmdno.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fizwiqop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwlxgpzw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3quixoisy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3utwpjxkk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fapywyep.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rkqcjrdg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwdgcje.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrvrqmcq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qofxfvco.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asyhfidy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3raduxpuf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmnhvynq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3porjcsju.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjtgnqzz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3goqoxelk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfllucsf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvylhbip.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hxcbivme.html


<!-- 参考信息 -->