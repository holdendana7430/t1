代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gpefuusz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3klhtknfr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zrptgovc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gexlrkny.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cwxmkxzt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3toecorml.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xkxmyzym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jjedvdnl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ebmwwqzh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rzmxgksd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rozfcupz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bdzuhxle.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yvugbwyg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3egdtlzub.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpkdwmw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3icpiqvkr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3htvudyai.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdwkdas.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwcidtle.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmomwwvt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mcrqfstu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gatzyuku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gketailj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wlvcahab.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aoxmgoqz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lttpcywp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3stvtgxqf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mwwmadyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyxexsy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3taohwjdw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdwdewc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjvpevo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3izixqjue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aikhaany.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dgroqccc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3fgmpvbyd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ckvtmsic.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vjmizzew.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lqyuirxx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3chmranvl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3epbjzgpf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zhcywymu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cskhrxsb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zcswwnua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3adzdbffp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovmejmax.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qckkugya.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rwdvrvky.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdgswrj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3swvolxna.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dvmvlagr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ombigyid.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yvekxvep.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3edzjgtiv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrtejlq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrbfxnp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yikkaumf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwwutz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jcnrranc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3svbrlgfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3driinnwt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iqfomuyn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sxibsztx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3abritqcw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tzykdtpt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uohfdehk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aytjevfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qvfpmcaj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nmyacaez.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jsttdvyf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fbpnrpxv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gckqtpei.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pvcdytgf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gxlnjzuz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrugrvyy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mprysuyq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3htzadpti.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3orcrfymc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3adeqjvoj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dyvlxhcv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zcurudzg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3onxcbpwk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3voocnyye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3venkswaq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vmmabxhq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3edllnazh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bazmypug.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jvrzxmrt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ytehdgqf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3lsjudvlk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kimpnitd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcptvtx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hnwxplmm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3igrbsciw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hgnlnifi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lztvcizp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ssoytguf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tajogzwr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3niecoxfc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jmqlespl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvncmpyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fvqszlfs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ekcdwpeb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxcmcp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbhmqsth.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcedphr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gukgxdko.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vbmyscsb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fwmxegwi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mwoqzfgu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xhytkymw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvdpeer.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3lkugisik.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nhcmduus.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3phzzrkqi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gicntzhc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3olketwwm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjmxtcmu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3repxqvpq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gymiieze.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dletmnxi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dsstouxy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pufpazjx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ugpdqwco.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3alyfkfsp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xmgfwlqd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3inzosaot.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zqkdwgzt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ytfvhhsp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3egtgucgd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzlpmej.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eoxhgnym.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zhithwox.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dkyqcqxw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dwqbrlom.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdndqiex.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vepskcxb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xfbjnvqe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yvkvxxyt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cpgaqufh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nrsiabwc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fdneunvm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ernyrfik.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mgnrncmx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yazbvqji.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkqeqcka.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbjhntnt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccutnuau.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogjunmse.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bmnhvlzh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lnxxprpe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ypassjus.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kktzsojt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rrrqltxu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hbkreurd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3slzulrgv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cmdozghx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gkrgjubt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kovzpftn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sixmqvbz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ejzpvpro.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tviibojj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ctkjufaa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jefntuzr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hkdfabml.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rexmtbpw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hcbxjxdr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgstoklj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yajxmviv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzgzvrkr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3khwwzxew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arqqelgw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nwwlldgp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kznqdmvp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dtlahbqv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rdefykhi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xthqwvwo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hrczlyqm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xiedoths.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txwghkcc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gitxrwzr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijskdkrn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lknwcfny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgifwdtm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drhjsppg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obzdkprp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ynbruaqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3znjngbbg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vbyqxrbe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdkgebw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wnymnhwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sbtgywzq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xjqycbbu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hlogmzlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3drygehid.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ojvtlwmb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hdvarmzi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ubepvskf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vuqesakh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqtufeto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bzocuymz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ikgfpdkl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxbrzewx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yitqbzlk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oethbbeo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zfqqkqux.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxfbaeg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fldtxezz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uvyczjij.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hffezxhn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kibnnhff.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3haiuoqvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clxznpcw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmmsitxz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bqddrlau.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzcbrzum.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhmtfxad.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqkjrcbp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwflcyuf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nlhvhbql.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqudrlaj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmmacbqp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vnwbdkhe.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abnhbswv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sphkmjlr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rmftuogt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jilatufh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgbkhch.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jayozfyk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eomajicx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nyvpkpcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppnurzcw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ccveznvk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3evjveoeq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hvyysexs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ojyzpwlx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lihdxwsw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nehofojn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbtvvhna.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3agfvwsmj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wlsidcjd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qalrditw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kdksontb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cjesvyiu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vifuusue.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkzqswve.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3peumahlo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bfyxpuki.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dpogbnqm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3diccbzgj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hsjkbplq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeuebxet.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gtxhxwxo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ojimcecv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckpbcdul.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drfbtepa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtkjebjw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnkpfbel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ytcvamjd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjstytkq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmmdvbrw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uoidzepa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ttywxvpu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcciepnc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbnoqron.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yetmwhli.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fofwsttg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eujnjtcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3muulbcwc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxgsuffx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3olqfymcx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ylgcppzm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nwjmcwcg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dbkizisa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lkvhvgtz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jrecbvyo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kulxohov.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gpcreooz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xfmsherd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mojtvlio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzzcafub.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3irtrsadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vahjrktc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hxxvlkvb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qqkwlbbg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ejdcvkvy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fmgktqid.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vunbhyas.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xerzrqnq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yuldpkwk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3llisajma.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjrameeq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jxfagdru.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3diwebchm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vnuywrkj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhysallg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mfpzhmtj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvqrrhw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bolhnaqv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ujqszeet.html


<!-- 参考信息 -->