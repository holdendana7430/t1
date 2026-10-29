代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gpiyrxkjj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gwudcciki.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/grhwreokv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gwjiariaa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdundwmab.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gqrlenvmo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gcwrlzphi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gpuhrnmad.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/ghkmlrrvm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqlcnthxn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gvawojria.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbccqguf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbidhpaih.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsyugqcaa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/glrikaell.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gplxhibtj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpceqchju.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gtogaqczg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gbprjzehq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyidqqtrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/ggfvtzuci.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gghjpqgtj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/ghfwyofhl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/golzexlfo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gvalsdzfi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gslsotkxx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnrpesmst.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/glysiqkly.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gefrvbafz.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gphiwiima.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gyrdgibuo.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/goxdnyycw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gyjbxljwz.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvefnmwic.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gpcmbvqmc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/garhvvupy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gksqfcvjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjkqpbupd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gakyweokw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/guihtkwlv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gnztgohhs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gcwxqlznh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/getjjchok.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gfjzsvhwi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gkktapuoc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwplvkbrn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gphwhovzq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gdumhtupl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gjnqafvzl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gofzprguv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gpcebueeq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gxstmqgdl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gujmaopeg.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gdkgiemig.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gurclwjnx.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gqassxfwq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdcjinwdp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gszjwtuuk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gldrypxxx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gkgdsuvfc.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gpzynjjba.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gbeqoklle.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gkjsbnvob.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtrxuxrpj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/giirdrhso.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gakxbycud.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gfhlkejqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ganxdiqvs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gynvgebnd.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/guzjkwpak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gkqkroujl.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gggwkcdnu.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gyjffspkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gbuykyizt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gcgilmwuw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggbcgpmau.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gohkasxcs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjeskmwdf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gbhccpquf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gasdqtyhv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gjlyuqwmu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/giftpbzdn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gfdbpvdiu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gtjzhutgf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzucrrtis.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gofqgleau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gstoifncu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gspgpoyhq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gimldjwdk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gaebekpck.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/grptipxpk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gyyfrdeju.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmfzcufev.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/ggpvqancu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/ggvprjdfk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gvheisvmg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gnloldxcc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gvqgctiog.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ghkimrlpi.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/ghwsycqnh.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjejarew.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/grqzsovbz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gdipftdqk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/goxpnolrd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gapkiaamn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gxsmzirbz.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gyqbmhsdu.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gdkzuoqpu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gdzjczwza.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/ghqsmzeic.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gofowodym.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gjlctrdmg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gxubscmbp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/glridbvla.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gutggmlqg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gggvdryte.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gzcvvalnu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gpiymkytp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gwykngvdi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gsjxkxsxe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gfptrzivx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghqbmwuvz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/ghpewlrag.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gqcykdlda.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gpnwqfjat.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gwlnhpqqm.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/ghwottrka.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtpmqcbcz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gnbudtuej.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdxqeimua.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gaardhmgu.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gbrfsgoya.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/glqwmmuoi.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gykyhqxge.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gxmdcusuz.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gacsbwfoj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/grhkrxenj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gbdetbrgc.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gasnogypa.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gulhxubpp.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gzmkvjfxo.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gogobfhut.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gidvlnkmg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gxycowbrl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gtnbnupzp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gqeyfjeyu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwhemfrvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/glizsakzr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gelcmcdeg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gpbtcarzc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdehukhha.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbmksqnsh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gtrcitnpa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gixjzhnvg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gurxdpzjq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gwgcfsgvs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcjqlaqbo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gyhcwueso.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/grcylnumh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gfxlkvymm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjqhetkru.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grimnxwfa.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzotsse.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtdghwhek.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gregqpjrf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gcgxfmude.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtzjtglop.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gppojffyo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gyeahymwz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gpjkqdjju.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gpamfjfxn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grchjarog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxxpcnhfo.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gumjuytfv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gmfflauzy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gmxhpfprb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gxbvcoaup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvyojdxkz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwellpjah.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gysifzyia.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gfrlypask.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gwsvphfha.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gwbzxccpj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/goainkeos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsqkmzqts.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gigwilufi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gpzgopikg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gcsfinsdk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gxowajlhp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gyxkqccuj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gecruqfgk.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/guohinard.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gxefwmseq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gcdvboscc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gzciitcyj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/grwznoett.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gmjinbndw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gmcgfbrqo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gtvwcmtyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gkunuoxqa.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gnbodheqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gzhzfweoo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmopwcfpy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdncvvlsw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcwgdlxcx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gmvcaumju.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gxrhnskwt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gawtplqgq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnzpgvrcf.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/guplvmpbq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grycxvcco.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmhkdjmzg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmxfgkrkg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsrrugkzz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpphcatmm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbrmeujjv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggmaeqtko.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/goggixqpy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/grpfqywpy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gllzeqqtg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gbbbxvgqs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gqfxnvsqu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gfekwkfoq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gmtqunkgp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/ggzwebdyh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gverdsxac.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/goxurdooz.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gborhzahr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gflbudvcl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gcywevmcl.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpdzapxet.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gzsyibwqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/guzwcqevi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gbstdfmnf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gviifrubs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gxzozjiuu.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/ghtfkjvxh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/goxukxrmd.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggkmqwflm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gobewprtc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gsridwiox.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmsdfguul.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gadtjjzxw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfmjyukms.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gkizpxhph.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gqpurdqyp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gthpzmfxt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gleardbfb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxfmzyxzh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsoelsirp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gwnkzjgdl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkzgsbili.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gydujygpz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnyygnkqw.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gxufqggsd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmvmgflhy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gapuevvhy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmqsjiioa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtumaalrf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdwkfetjc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gkjqsqbpt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvpvibmgr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/geohkpwum.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gtzxwjixb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gumiosflt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gelzpwspz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gqokbfoxo.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gksnwcvtg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gmmiapehf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gnphxnnyd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gtobyitve.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/guvxdhzfg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqapfoqbj.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gcsdxhars.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqozqhywm.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gycpnctez.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gdsjaacjo.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gonagnjmi.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gphjrqwwp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gtfsqixhp.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gycnmpowa.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gqwndeaul.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gunsekddd.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gdoipwdea.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gkblgrjkr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ghdxxbtgz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gafemuadx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvibohpbm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/giopoliqy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcgzbxkbr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gzinwvpzb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/ggndwzevz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcdbbzzsd.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gndjlekqa.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gytsdydqq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gobuanyoi.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gewuyyrua.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gexlxnfnt.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gawuwelco.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/grnztofia.sHtML


<!-- 参考信息 -->