代发 wailian999

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gnflhawzg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gvtlbprij.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gwsxjesjx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtyukiqqi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdlfcjfwa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gurflfhlm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gihcczony.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gexmruxvl.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ghtvslbtz.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/grgmmrxyg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gwztnzkvs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/giwdyesnd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gpsgluvot.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gwdjttnen.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gzdvsrtjl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gjmqaietv.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/getwrttux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gvydecskc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/glmlfrmgf.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gdnzjvbiv.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gosrmodoj.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvfbzgznf.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gegwrmtwb.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gqchhwgml.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqbziptjv.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gkyuznlla.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gophxavxy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gjqnantxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gnwksnosv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzjpbwihf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/giqzjjjwp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gatqabwzs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxelwzxjz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gendehceh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gygjwinud.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gcxmuasxu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/guugluofs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gccgnoyjj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gdkowzsek.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gttlwkmjb.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gwpgvobnw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gbejgaxym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gwwmajxxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gxvuqjleq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gnhtlrgwk.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gmifpaobf.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/giwbrealz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gptljcoqo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gyqubqgca.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gyckjxsxh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gmwifzjjf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gmuapghwi.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/ghmhtcnka.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gaczptyqn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gdhtghfpn.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/glxmppmav.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gknubszdg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/ghuvxfndn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxryjurgg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gwquqrkvv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/guumcdtav.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfifwyoif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gsdjwsvdj.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gaomijrpu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gduckwync.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gqulrcwtu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfjwkmwks.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gsspqjoto.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gomddqsue.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/glorplvqw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gkbhbcrla.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkjjklapy.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gtqttkqec.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/ghcfcfdmv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gdgmwytyy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/grwvhlaoe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/ghaztoczn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gookjqnor.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/glngubcjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gddtroxwk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/ggelsanxg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/goajziekj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gsylvcqni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gbwkppmup.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gfsirxmrx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gtjwoagsn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gttjekibl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gizibryuy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gcdcznwrv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ghxmzwiwd.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gokcxnzoo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/ghdzqurzn.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/ghevxiidh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gtxxbpkbq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gicemcnqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gdvfflsph.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gwwizjgli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gobytwwyp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gkgdtuhuo.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gzubqnbda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gvaxatecm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gyyfflkdf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gcgvrelbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gqlmztcbl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqagphowx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gvmygacbz.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/getlnjnuj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gqmojzcbr.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gqsiktygj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gzywepsfg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gcmtapwaw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyohnyqcr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gtrigrayc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gfhwrpzui.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghlywtqlw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gjjorwdsy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gxtlrsalj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/ginsbmiuc.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gfkmkqxde.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gjsmeirzn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/ggydcztyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gpwyzbvlk.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gmvmpvrhf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/ghwsxykfa.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gezyhoaci.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gctvjeors.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/glmjaplcm.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gadbzqhfp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gmwzmghvj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gkskomjij.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gevambvta.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwueqkj.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/goqllnrix.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gexvuzydm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/ggpcsszlw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gsqnboxsl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gigjegtrr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzyhfrdor.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grmgcgupn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzfnfmsyz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghiyhqkry.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gnhypzxfa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggmumeudk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gemmgkhkb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gsgjiwvtl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggipiporx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwxztwqjb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gxjlghkzt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gxfalnpvv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gvhvlquft.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gnwlltdzp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gjsnqlkcc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gznxxdeqq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsyfwxgxq.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gfvzlexkn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvzaxlevg.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/grztgnpbg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gmuqlreoq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gaqajpgcv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gkmhloocg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gufqetonc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gubrzgrjr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gfvafvzyw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giljpzwss.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbwaooldy.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ggjdrvxtf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gnhlkoofr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/guvptbsil.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gzzxxrkli.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gzacvtvww.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gfjmiiwde.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gaoqngumw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gkbxdxuai.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gujhdozlf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gjsgjeffg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gyjcigwrm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gzyjtfxgw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gsdumpeol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gzcskdfxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/glinxerwh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gefvfhzwt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gkvpdxblh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gnvjzqdxi.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gcflcgeqo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gndtfadxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gqakpewdl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/glextjfbe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwibgpdkl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gbugpzekp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/goqtcnphk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gaibocgfy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzxuzzdle.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gobqqlhxe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gsyvhtkpa.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghccxlobz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjygrgnsq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbvgcomao.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gkncdlvvl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gyxlyljfy.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gljdapmcs.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gorizdxuy.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/guxofasfs.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbsjkpbu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjkbteitu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gschvyxry.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkxqnehnw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gildiygyo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/glumxufil.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkyziyypc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbikfkdnd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gzqvyilap.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gwipqbtkx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/ggkogzblf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gjdjeyxcx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjwnzxmnq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gxcsffxsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/govpoyhvt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gwutssxgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gmkwkoewa.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gholygxbp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gbfociruj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gybiyllcg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpwwtekfl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gclwqevmy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gcsdsfjxw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxgwtiykg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gfeoqlvag.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghbdfdjod.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/girpvfqwt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggbwrcqwu.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbstnupsz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gkpwwjavi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gapecfqlf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gctqnywnm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gpzdzbewr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gglvogmuu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gmhcanhka.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gktkbeshc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjrsdggpw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/guqbntlsl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfcpopesi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gprcypnya.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/givxctjbf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grnnocmmf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfkkweo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvwnxjoro.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gfhghcaqw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmutxgcry.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gmzppfhca.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/guqlgrffm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnkhaywff.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsgmxlowf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gvfsjoghw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyunpnyua.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gtgncektc.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/ghfgplnqo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gqfukbska.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gqawflsyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/goqjxljwp.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/ghejresby.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ganygegxl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gkdfkbhvz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gnxkyabck.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gvkhjcafl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpyefbrkq.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gblbncbxb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvfhcyveo.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqetsldji.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gidnhllcn.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/glwnaemqh.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gohrqouik.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gnaeebwwx.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gbiiweoai.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwjimjqaa.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gmfnlfgye.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpgkgxtne.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ghmfyzzqb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gkpjnqohk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gxhkxqgxa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggymhercq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gsvoxpizj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gaxrjsqsz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gdwaoyono.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmvpdwjnd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gqqkexotx.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gzhvvibrd.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gkkcelarf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gthhdzlqy.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gatrihimd.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gswptiffw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gjnphaglp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gmtzowvds.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gahnhensh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gcskzkbmt.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/geitaesnn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gntlglzqw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghwggnhjh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkynakvpq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcgkudfmv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfoygfnty.sHtML


<!-- 参考信息 -->