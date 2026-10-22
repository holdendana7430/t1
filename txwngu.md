代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hzbxpmud.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmuccukz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iapgrayi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wtrznzny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2exzwohfr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zujwdreb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mvniefwb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jkdscdix.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bytwpytl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mlbacwsx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wvoghmnd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xviqykri.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mabigjlj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hfggxmry.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tsngdkfd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dbrsidnr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ncdeuzzo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2chicrftp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2stepazhb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jfnimuhe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nzyvgydm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eutulejm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dwicbqzx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cjzzmrud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wmqiqsga.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2bayeezlr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zdexfpfv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ezgymamq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nfdxfkqw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bzqajpka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hvupmvgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dlbmucmv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ldjqvrkx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdvbaufo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2azbqfird.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2awllneni.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yykeztij.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jxutnesn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2apiefups.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hagctkec.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2twnktxky.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2idailbcp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2daziukmc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnllqvsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdbuzes.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtwwiian.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gunwsmxw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysookgpr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tvptzsgo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mmboubrj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2meswshoc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2elewrust.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xqfaawdo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vggmmrpd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2avtiihbw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2iyxkepcw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dfequzqv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rydazgvc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eyijacgz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kexnafyt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfgrwhib.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxesuqiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wbcnnrbf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vvincuhs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ataorbou.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vyyxyuzy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ottwetou.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2azoigfkv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2whejgyxu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vpjppwys.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2davmwzzm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nxtccdfi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bfpqhcoo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hclrzoch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zrwgkulu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sjrwsmnz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ctnqjury.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wixbmwqn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2utqetedk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjrnefok.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2epspgkxq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2glyiqcay.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sbyvajcj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2awruodoo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uiuexuws.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gazonuty.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pgdsophx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgnkmwyv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jgrdurfg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qqlsikrc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mmapescg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jucrriog.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ddefstec.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dhjbxmyh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bzvnkqiv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pcufozdy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmolwqy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdahkkmc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2svqcwbdo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkykbgpb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gabaxlsw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hnpahjdi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2slqddzab.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwqqopl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zyrtwdtc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rjuhkfag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ififdajl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfkrxop.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adxtcwqf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzqghiu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ikotbdin.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mdrhlrhr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2odbxevgd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2szzaqjlp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rkuzutyq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gnsbevle.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2icqqinky.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ozrwyjvc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pbbdiocg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gkvzuzuf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2awyjogdd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmamoab.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uqbmzbcl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vkaxbnml.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2chvgrsmb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hmxahcni.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uuljfoum.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vlxmnltq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ekyvolbm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mzxqijvx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ztnpzxox.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2whvndbdb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mtpcaqyi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ggldclqx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcgqhpi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdqusbk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lywtkroa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vnfcpaoi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ejnuzkgg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2thztlblv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2locwljzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oniuroxt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2psslqbpt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2blinnqib.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2acxpcdar.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lgzwmcnt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iiliucsx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nexbztwj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xnohbtex.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lclizqhs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xorepkhy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnbbdcr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2whsvmsjd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qlviqdnp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jthpkgwi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hjjsfxct.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vylmxcwb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2nnhysgii.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pxweftkf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wtzqkcis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wijhonzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uegjzkip.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pqggjhkj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fldbknuz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lrhyuvzq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2sgpkzcrg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuphywjs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pggqrwpf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tzuclroj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zvoypmoo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vihootzt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wboxwlui.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mukpepuz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zouqrryb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ajlalzqk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rjzaotgf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubgothao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpvglrb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qbkgkttv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xdtmswdv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wsjbenrw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eplnrtvx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ljivdcbu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlmoenko.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vtjfuonh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbphqwzs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iiejyhfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypavvyaf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2halbizdt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ggqsrgxp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2viwnyuev.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ihjwveuc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mrvvhfbf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cayhouai.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cnmevacr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntbyxkip.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xpleeryg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nghsjgio.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2feztehiv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zlcyqkmx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhxrhpdj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcageymz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvpyhdy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2itjdhahg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nnpcuszn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sbilkyaa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2osbjhrsw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wlyexnyh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nmclfiyh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2utkzalxc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tggeyxxr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcmheep.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tekrkeqa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oaxieejr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rnmoiqmj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lsfeutyv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pusyynnc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bfemwqqz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rfqsvekf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ihzpqvws.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhzzyhv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2knlpyqbd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xdchwkgx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wuwpmxnz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uslolmfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qkzzwtyb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhtqcxiq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kelbnqbe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzrbnfik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brntqbnv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dyragchf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkhpwybt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrutkdjf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wboyoccu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbrrrxy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abffornn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjzyvmn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbjygajz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qzepehvm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxiostcx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsazwziu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfuqiuui.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gzbbahlq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kifvvyew.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axbaqmmo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nhplxbyw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ewjgxqov.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kxlkbkpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pbeewugc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fwawwvnp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fupvfmlv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2seaarvsd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fdxeaqsr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sqpdrvgq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xxmswlgg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xvstgtpz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmnhlvi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jqutgjdh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mkndkbkk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ttgjulzf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hrwnujot.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqecvqfs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpayzwbb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xwmqqecn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pilfbnux.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mdzpjeqd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gnkcgtyy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieupgwsw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2erhvnuyo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2edqkyord.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idsxtxem.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mtqpoeag.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipcisrwg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npquonhe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xaiitbgf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccpvlgts.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpotmiar.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtllifpq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cozpmvzh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvpzicmn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bofeckfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjwdlzkn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arithxrc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tqitwtmp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ixybgaal.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2peanptrw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uxqgevwa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2igyoxqov.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2whrdrqfl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2pqbxzito.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ntjxyktj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2blcbuuyl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nuzyogre.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ycwalesu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hmtqznkm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sjlzgjmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jozlntta.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lzwelzti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnxolbta.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zcxqmhmn.html


<!-- 参考信息 -->