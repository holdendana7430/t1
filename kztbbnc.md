代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/glueyothl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gbksssclq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gjfdgwzep.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gxfwbxvau.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gumcfarpe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gusuyebms.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/grpfolnek.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkvywadro.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpxbaeavm.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gxjeqeafz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gfcjoxqat.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gkaorusjk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gouiyejxo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlryjoqd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gcjvduwhs.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ghzmxkqmr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/ghlnchars.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqgjtzuix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gtejxybnd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkmmwvtpk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gqaglnaax.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gslxgvrou.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gevjztbtn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gwonzinrq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gtxvehzmb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gztakfaue.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gnjrdxozh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gofrupeyt.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gdiobqblw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/geidcdmxa.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ggxmdqubu.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gayldsmdn.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gqhntjdks.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gujyntdpt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gcztdbtmt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/guvptlutp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gbumpdhsg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gitvzvkxo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gajmzgxge.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gyahbkmdr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gjoqhidfh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gyndjmghp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gylgdrywp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbznbarfn.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gxpdlsyke.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gotecjveq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gorsuzwhp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqbdyimfm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gevwcykik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/goffmddkf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gndonkdny.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gfowewfad.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpppkzoxq.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gfbvabcrz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gkcchuvyz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gqqbzyjon.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gkmwtsjcz.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtaakcjcg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gsjuaybbj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvrhusaty.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/ghkfyojwv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gklfnhjbj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gvwywbqwx.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gpixvartd.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gjgktipwb.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtuawujbe.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/guimructg.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/goyepvvpx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gcevdpaxu.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/ggwvppwav.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gfhitdlif.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/ggddtlfsy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gfjnsjzgl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gyqpvfxsc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gqvqfdkef.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gdimxerzl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gskxvgtjv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/geowgfupu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gcvaubgmj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gmgqkfqfg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/glzofplnx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gsuigmasq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gifjddxvb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gsjuoqvdd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ggzhyouek.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghmhnzwas.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gbrkxshvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gacoarmjd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/ggphzwvdg.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gdjyzynct.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/ganavgjst.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gbhkcbubb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/grgpofhuu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gagoywqmz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gxjngvfhj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gggwtlgvo.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gslabsmer.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glpxewvhd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gzvxrmsgb.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gdcbvkmih.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gyqwmsrah.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ghfmbupxh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gnmhgevcd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gfkxgoqzr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/grjglqbnw.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/grluwbzvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gkgdlmtls.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzsfrxeqi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gkqgqyktd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbzvbjgi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ggzqwlpcb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gmsdhnunm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gdzsjjixy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfrpueeym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gszeipakp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gdxydtlyv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gcusbhvgi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gompmctbq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gqnoyddvr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/grtazatld.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gvxevijoj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxxobdzln.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gqcgpujgr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/glrkanapv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrfipem.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gbyjpzxxp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gmffsilbg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/geiivbkvk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gdhoatzop.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gspyzxyln.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gizrwjzjw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gmqgavxhp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gbnzoxzpv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/ghgmbnkvx.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtpwipdwt.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gegqdwnok.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gxkqvseqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/guuhademo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grahgsvyq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzdkfozpc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/goyczjsme.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gbfjaaxhy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gsdwnatod.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gvbzvmwfg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gzqatqqib.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gvobvemeq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdhvacvir.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gtnjtfpfw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gdkideifv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/glomvchkx.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gqmlnvzex.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gqxidzujj.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gkhlfsbcu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gixsgerkj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/glessrcbk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gcsuxbpca.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdaecuezu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gipqrwtbs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grdjaxwjq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grvuulelo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gavjrmfuc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gkujirolm.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gzncycdgt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/guuhtfohm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gtpdlajmz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gxwbfmiuc.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gcocpttui.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gzjcapyab.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gxammmomu.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gpasmgpjm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gbfauzbny.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/guftemcsw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/ghwkmeghz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gynwnycbp.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ggbjtjocd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/guuvnwwip.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gguqjtptx.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gvhrifagy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gmpyeipsx.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gjqeypeoh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gnacdcieq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/giwlqczyk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gynkhddng.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gnnnlchdg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/goejbjxgp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gckmgbyxz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzoxebpxz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gamwlezfm.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gizmzbrtg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/ghfrueicu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glflzpidb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/glqchkfcu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/garmcsddp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gqaaqacfu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gbzsuuwno.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/glytgalle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gtycrfwti.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gessolfyg.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gkjjimhrr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gybnpvkgk.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/glynfrzzh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gmwykxwgo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpolkcjvx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gfhrncjmb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gieztsylm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzleuxagu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gqnlnmvpy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzfzlmzok.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpqzhavfu.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gubngvkse.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gidzqckkk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gcturzmsc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/guxscbqoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/ghyfqsalw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/glvgasxrs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gdxkrbpdl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gabyldliy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gjxmhisld.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gnsogrlqv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gjfopouxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/geodmsfte.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gundfupdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbeookcqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gwmzjoiig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/glynucysw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxqmhwgej.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ghyejtqzw.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gryqkzgqb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gobvyfaal.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/ghulzipeo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gmfxdofyh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtauqereo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/ggjrjegav.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gucxtedfv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/godmoonir.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gkbbccvsr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gyumphoxc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gpaypodhx.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzwnqfowm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gotenqgod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsstjfnec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzndwgnjv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gwtdiyasi.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdmoawjzx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gomdncnwx.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gqttcaytg.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gggsovvom.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gksgjmkho.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gipehsqds.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtfgbakvl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gljgmlcwk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggohtlntc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goqkrizhm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjdnttdbz.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/ggucjfccy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gvpdaswxs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gvpykbrhp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gzhuamusj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gvmmedtcp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gquyqtnst.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gnvcembxl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gbaggigit.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gkwjqdstv.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gjewyyydt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gfaejdwfb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/grhnzejph.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjnpsnrib.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gcrssrmbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvzfqrnoo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gksaulpcf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gbhfclypw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gcgubjnpe.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gilljvnmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geieahquo.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjyqdewyv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gctskolhr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gxuchbydj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gojxiaazt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gfoblecqy.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfyrfpqtv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gkdbrgcxc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gpakqugyv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gopbjooiu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbhkxmxuh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtmmekhzk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gluzrdedl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/glwqixcvv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdapztbax.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmtovxxps.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwajjpvwd.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gluybbjbj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkstgtame.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gwuqdbuaz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwuimrfob.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggcehdcjw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gorfzlzzu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gyocprepg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gplbxxzse.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gydgsadzl.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gxmcznvhq.sHtML


<!-- 参考信息 -->