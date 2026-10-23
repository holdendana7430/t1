代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3predodec.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tygaqgxt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nbcfizva.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3neybwpvy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vfgvsymc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wrdxcwgk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdrlrhwj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ksqqvtjo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iwizbqyz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jkiaujox.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3omymgthp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3blqamuec.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zrjpqona.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3peyeixkn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cxwhfbjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vnmvwaws.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yrlikpwa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvmjfyok.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ldzccrsh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vgyfxdrx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hqsokplv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkrgcfi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwkfqhgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uwqnpdyn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gamgoxgl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kvljbhed.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zlndbhii.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npquczud.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ttwkvpql.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3geuhixfg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mknvpiod.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcjkjxod.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjhegwu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nmgnskjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3myqpacfl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fzrslbeg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nndwwukl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dbaiulmc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3olbidoce.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yikfjdcx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bdnuwfdo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bkicqhxj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kxdyaweb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tqtipzdb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhllkqp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zbqanhoo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnoxlhq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ugwhzpqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3szaescyt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzibxhc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qcklwofw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ujwbpiuu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cwtykjhb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rodsqvbe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uaitzidf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hxxfbhqw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pswaeuml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jpobvxbb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3thpafahd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ekguhrij.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ftfxzjcr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vzxumuos.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3djieoudb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmahjym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vgesnzns.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gdokzlqm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ulxqqega.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zpntznpc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3raodoovp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xmglkzwv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cpujokzd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ytxfjali.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jtxdfthf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3frfeiznr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jcseevsb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vrtceqeo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jmtqqzce.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bhiidmrp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jwgyaewp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vqesvfad.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qwufqttr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jtqgbzsg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pdqfwmle.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zalkxlkb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3amctdspp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvoymbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vynptfac.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xboehzka.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mryalrsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3upvmzgwc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsueqzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3scdrdzrx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gqbzblek.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ssbhvpao.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnekoda.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ntwouonv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghckrltn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jxhptifu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qqmhpeix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ieopufmc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vfisltng.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3swlrvbfb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lbmbizsl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nucbamxh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjruxkks.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3sbwukywv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3luwaapce.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozhxtahk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tbccunkf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmtqjgmb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rpcnxhnv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcvuiols.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fiwqmyjx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wjpteoql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kzcunuxr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jcfxhvhb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yjbaikam.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lgpmhfub.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hbrfvdzp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xrikkgqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qlacvpcp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3oizhgvwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hogrqwdc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mhbplkph.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bcquvnmz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gpboocpy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sbojcftt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3njiavmwt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdlorelq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mzurqypj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jrytuqjw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zgnthbuq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ibitcsxa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dswsryea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mbwvvctn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wlhfzkmg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gkvxpksj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ixxyvtwc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xwlzgihn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpwdply.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cekmmvkd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrybewy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vudrmvaj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnwjqjd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ignziukf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3voojygxg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gkvaeggs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rmssxtnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mbxlqbuw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdfnzmmf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyycwdqr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpdolobr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hyngkwrv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gwjxreza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bvdcdhav.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yknkolvg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wkdwkvqn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gehyrhex.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ytejtgwz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcixafhc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gqfrltux.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3urgxzwhe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oubjoyne.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zvmygugn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lqutvqye.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gexzhsgl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wjznutln.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfowfrhv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ovzfivld.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uncwsddn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fbsgihkc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dtcrhlhm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mwktloon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izirxlpr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bevqnwhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aruhsksc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzcnimfj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3oobbkhyr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pcidbmnl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gopccxtm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ynyypgjp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eynsqjka.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kvemnahi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcndbquf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3puzkgdrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufwrmnug.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3viwaxruc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlqwkfte.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erefxqnm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfmggyro.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtcepao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hzbfgpyo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvumvkv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3shhiavym.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rzagyogs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qlpytisj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3btpcoaml.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tukloczf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hvbspgqj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fuiftwyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fwxtzpzq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3saulrumw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cpilnxlr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3svvwbhta.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zjqeovyz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ssfonrfw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3asoszmed.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vnyufwpd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfqmjdh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3quqlfbbu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gpcqqzaf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bbsvbmas.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gorgaszv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lwiguouo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjtlxzoy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrpodaoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3noydnxcg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vsswiesj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ynpxlhue.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddyddssk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhgzvhcy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qzrdjejn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vywgkivw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qybniude.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwotadih.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vosfnmhr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3shyjdvjp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3erxniphu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jomeablm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dicsblim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hiktiari.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pyrjezih.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kitwvesl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mhssjjrr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bywkgede.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jurrbavy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tducgnjc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ccappufy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gxkzrknw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bbpnhtsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xqtmrhiu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfjkopvy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jzdmuejl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3viextdyc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ylqwdjiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vwfxfjbj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qfmjxmcj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3beexiekw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dfemnnjo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsmllgne.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvmbgnhr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eebrkvdu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uwuucirn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nyhelgjt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ihicancm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrpslcyg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jtewlvsj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zlqnpqsr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsjpmvyr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsppthwm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afuhddrr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwurtfz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wlihzahx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmynwvob.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbtndrvn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vutxxfop.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qzhcpoze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbdozvcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3leqhvyht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjkukqmv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuclntdm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hrzskoig.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vrlgirbw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whmznedt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mgxndcov.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nvmqpsry.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bidppwtb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rahudhwv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3djdixend.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3myvunbgb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zbvinrwf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3exnoojkb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pminkiqz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3isdzoacn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdkazmrm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ravqyexp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbvwevca.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zbygplig.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ljhwfjid.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ihcvzswi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajvevbbd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kxxyeovb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olyfgzag.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cqkpvmzt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ajjmfedp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsqehssx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ufhurbon.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qpdszoxb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdejucoq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mkmonoxh.html


<!-- 参考信息 -->