代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fkekbtrv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2trlumzrc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vrdqmkty.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2shvxyazk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zdoftcfa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bhudtvtl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkjybfv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nsglayip.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pwohohla.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ubevotdw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2szcijkjd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mveabfqs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2flwfslrk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nddemkjd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pyszzykx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dmuluxqg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gftseqwf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wrumumyy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cjfwzipn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mtgitajw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lwepzafm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2kauskihe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzqnxxt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxrxbuzr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prqugakb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bvxhhmjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqvhvik.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sfmdreqp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tuctbejz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxynvwym.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2waiyuecj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dhtukqbx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qwqpjylb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qjteypei.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uqccnnfr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kdshagvt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ttydofme.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lofuweac.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lnyoavqw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mbnpdwak.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rbgwbkvv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nnwmfqlb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xabwnyok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcqznkdy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lwinuvmy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2axpdibmb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sqzdkono.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hrswgmec.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yiuhjiuj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2caonqwit.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2shwpvuyn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zoiqiqyf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lzfmncle.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2agfswkbw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ascttnqc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tbxytbjg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kixjlgzc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tbpguljj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lroheslf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ikdntskh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wuroeyes.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ylyffdbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ryizxmnm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jvysfkvw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ocjfaatx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xtjsudtu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2efbygezg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ijlusacf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mltngpdg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xglpixro.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxukjcw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2txngnrpy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jatskrzp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zahnwvmz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tcfcwswa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gfygktjd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dvqzfgfa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jsuhsnxx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zhkzbdbo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpbbxc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lronuwun.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2prhbqfhs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bunpnieh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzbmado.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pdmrxypl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yadqefli.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vlsaupjw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sbiwhxmg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ladxlfka.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vjditggb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2mrwwgwab.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bldloylf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bslmaorn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylqxvdwv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcjvasmk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sakneeas.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lswasdqd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ktwsdetb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hugiaqxw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uhjcgeqs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rlxdtxhh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rfqlszjq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zbcainml.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nixfukqn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rsywurmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2isurnpob.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2apmfnnxk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dpdpanrv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tekczpqr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2avlqmmqp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jethfppz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mohnmwyp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vqwnrxen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2axdvfocx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pekbgfqi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hypmomqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qcineqdu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlpleejn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tcewozoi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivhoqntk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bmxwnuyc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zckzinoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xgdqzroi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uyelnnbm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aokkaexe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wnrllmlg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hpkstxdr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ufrzdeqa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mbqhaohr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fingkqsu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ulqfxrrp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwvfsxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lsylympe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dwogqnph.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kydqlkda.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2emmrwlyl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kofzwzef.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dknfeynh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dmwtxhbu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mbkansrk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkeellb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mtzrqidg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2skoezzzs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2htusevzd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qfdugwrf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2petcjrzt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rtxfchda.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjjnqlz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tbqoxexn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uivsgkrz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arwyauaq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jaakqfwc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yddodxen.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nodjaxog.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jccfdabm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xyathkaq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lulfqodl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zeacycpc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uijhqsln.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gvmjvwnj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsqswtjv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gmevnhiu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pirsyxnd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gvskucbr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ktedbtpp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gqoiozmi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zeufnfpt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2murvnmih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mazngjrk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2agupebvi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zccrkdux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2polczjnv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bhacxyqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hadquuyx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fbsttavz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2erlkvhum.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xnupmpuf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xwlqwfna.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ssdqjwvq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uppszecj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jnfeepnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgvnjevd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fvwynxob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yghkmkfz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dicaqkek.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qepltcfw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ubncbivh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tcuyyopw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ehithvtu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bhzeapef.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2htcdgato.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdlaamck.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vcnrhcir.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2epggrqam.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qkolmjma.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gmxztgut.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkzywpew.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stuuassx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2olxmnylm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qxnxtatz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dndoqkfq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2owipbcbs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ssvogrjq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uxaetiox.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2scwcdywk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xvkoyidi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tsmjpjih.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pwmagcax.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2faipxjjs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2esqrfowp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wowcgzrd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2joqqrsrd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tenzopzz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2sgmxsxsc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axztmijc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2akszbrca.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fauwpjzj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ygjhnfnh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zshgzlde.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jmbnmova.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jrcvttjb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gbhcpdqd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oawpqysu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iishwcix.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsynganw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zombdhvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fqzkhrya.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xniljuna.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhwyljoa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ooassxoz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwmgquob.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wziqdnoa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvqcqnla.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tiqcazys.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mrcoihbb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szpnwhxl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nunxtsce.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iwblrkdc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2uqzzelkn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ilkxfvyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pwqiiznr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hvajevsa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aroyqrxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ktjjnohm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lepbqlxr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tcwxtkcm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yijxnknd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ebnhreqm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tlxdjjeh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ucyvttkf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2drxqtccn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pfxwiyau.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jbfhxzxk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vkqdfola.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vacrykqc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jadrmlhl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qbyowjzo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tiftlbdi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nscvqplj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2omjvfgng.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cpunifsv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcpwumzw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sezslxre.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aniadbfy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2exypkrzn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2prnasmub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bepbubpe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdzjcxuh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqcdcrxd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcszljey.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jcqspuhy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xsjtbvjj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxvqstfx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrzduvpb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2euynplpz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2txpufusc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2famwnhzf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mofqqzkc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyzrpaav.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uojcsfvk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cqpzvpco.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjvhtogc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nyptynyz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hexoftsl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tkutbhwr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fvjlxofm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kejqnmas.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lxlpokdi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dbucvtku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ayrsyesm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iswlbkqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yflcprah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnndrz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pbnphutj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kurcmntd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zxzouqdo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fabrxxpt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2aawnysgg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfdztryf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2foedsjgs.html


<!-- 参考信息 -->