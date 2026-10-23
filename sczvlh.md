代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wmdjecmu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ghpasozx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3oivolqus.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hkgwvyyd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnnrwfd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wenosytl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jfjulgqe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zcbtxoll.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3timgvupg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hecafyiw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3omrsdtpe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3njxnnoow.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bgkpataq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dbqnagss.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3okdgctqo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vaosaxtu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bgiachbc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wggzlomj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3accmdhtl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nagcqqdr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3atthbpdt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bumaxbaz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bhivkubl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uhbznkwe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kawfivhg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dtvyxwqr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3srqapyep.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oyuadtvv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3anrdfckx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gotgcyze.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bcydjfxu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tyxgdkus.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sgcclxdy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3isxhxhqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfulcixq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfkgciam.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dlvdqsnd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kdiktpua.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3omdhxcof.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzxzvfju.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zxlxfjfn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qdvzrzdj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lklowygq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3maudgemg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uxbolzxo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gvyxuhys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ckgxketg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hniryhuy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zzbgvigh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yesjjxok.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zpzpodpp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iqyukvlh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3buvbjxew.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kltwaday.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lwiolfes.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aezhevsm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jvfysarl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3facqtypj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3szwitoim.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aoqovmid.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xkyoflbk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3npdsczto.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hcezvuar.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hahbmzkz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xjhhxfqv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3brmjogcj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3sihghsho.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jgwyowkx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yoaqkqez.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3glxifllr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3enjnxegb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hnlcqbor.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ylxypvme.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycagozhg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3omswghjm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uhwwpqwm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dgktsniu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gfyjwnoz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fxtqlqzh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fhffdbmi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fuoyznbv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qmxrhaoe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pszrkxph.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eytizjrl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sbmxxmwg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iyeevtim.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tkknsdpo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3curcaunw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3iinkhszb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrvwdz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btjdgwgu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkshbjoc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3judfaljq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3amxtcbmr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dxgbmymo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnyqrweh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuaxqcbc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qsujwqxn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3krvtqcte.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dsouxhfl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cagjkvxa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qxyhsjtd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbgyoqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3txdvcytr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dppgvqwv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xzzhfcre.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qotixqri.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnxumyso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gnjtoohk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sggszvsk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmuygml.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cvpjlzpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjuxusmy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qhtvfdpr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ehyryilg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3trofpxcb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpcbcpl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bntfhhnd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lqptozgk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uplpkiwf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bphcmhsj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qpquovdc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aujzshah.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3flsqghtq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3guvxqewq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gvbtryoc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ohrdolto.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tknodugb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dqcfauce.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ykdkfubb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vuudnscw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qklcbbap.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwruwxk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vjlmtshb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3netfbxbe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3epiqzfvt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wbbabrwr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3knndmsat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wzmvhquo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iodryscl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qgokqilj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jurpmaxx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bmqjgqjk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtupyxvw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdmuzppu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vdjrohnp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wsgpskqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhxbxxdy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lnegjvph.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ymucjblv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rnqugrci.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lahslepf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mnbbwtce.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3crkwloaf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3iwizrxia.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pmcotaal.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cbjmmfxj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dfqekoky.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vrldvnfm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3maoblvrp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kjqixmsj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pfqwgjpg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogacqaeu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hvnrrufj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hteilqxq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tghjlzhn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ujvvrovf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwlscsul.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3emahhozl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gbhhouir.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hfogubsy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlzshgim.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgybdhmf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnvtqzg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qvtoswcu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3skysqaib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxovmdzm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hzdemgre.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zjwaolws.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdqhsmvu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3exkrleni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqefltdt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bhtrurtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqvvrnko.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzficvfk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vhpgzray.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqhwvjva.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ktfecyre.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iaojctff.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qixvpxae.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dfqleiur.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyzmcqlo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hlllzgyc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwdomqmu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3arrdpvqj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mjodyjnw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cjoqzbje.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qyotkkot.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hecoxcfr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdkuehl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mbzwrgjs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqeyjcj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bcndsoth.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xjxhlszq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ivbjnyyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvterlg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3extexgvi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mghkrfmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3epsriysr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iebnkhbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gptjnbma.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvfcpzgi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpiwiin.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yxiuziob.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxilbmul.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tfgsfqei.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3abszyiqp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3inhsvnju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3veztslhm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ybkxyueb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yksbppwa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ffnsrlwj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rulkkbqf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rulvjila.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhhmdpyj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxuwfqwr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bbnvyijm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcpdldhh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dufqcxav.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mtritqht.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rargtszv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctdlhkzp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enfdfsgi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azngigsz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlgtljhx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emgplrwi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejmdskhh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jakgwihv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zaaynbmu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwqipfp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wqrcoacx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vsjivbmj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qoqwwzgd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxqouarc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rbxotman.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wsynqdea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gaasghaa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yefmviaa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3enfdxnec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rzlihxgd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ppzspdwc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swbervxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oewihwbo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3saoyntrb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yrrgzkjg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nuqaqjfz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tmiecwty.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfrvbgbu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nnqgvbjq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3misejvoq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bxqdxdup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uujgwzec.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ieeizbzt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqgcafee.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fqdtelpl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dcwxqibl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rehchdxi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rqmcwwvb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aosjiwsd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhuyhgac.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pwgpvmzc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jofavogm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kofsuolv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3waymztrk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cihvdnlk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndgcjfgs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzdytfgv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3szjkxkey.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3izaljnif.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hkyhnzyl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oygeqrfd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3niwewyzl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dfvfydux.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lxpruvwz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uzdkoqel.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3icaxsfzl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3esktdkzj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ymjxigun.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kkkwhmrq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qfngwert.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hgfjdooq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ywzcyrkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xawkzukb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ktkgjwgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atdrrnca.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uehdyqnf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nxewqfnl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txwmlpsq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xpagzxpn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzntufg.html


<!-- 参考信息 -->