代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/geykzpixa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/glrzqreqb.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gyfwycczo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/grutmsgko.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gwsszgpbn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/guuxesjby.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gqohkkdze.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxjanivvo.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gkvyvomgq.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gcvygebkq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/glahvqvdu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gzmsgbpai.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gadrpnsrf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gkdiezdzv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvndxcsep.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gagkuqhmh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcgyvnh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/goqokpjfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/grfgbtkul.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gmgltzgur.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/ghdjnbrgb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gpcgebycy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/goqlteptw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gurdcynnc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzwowxaau.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnrbestuo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gkepregjt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/geakrleqm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnfoamuzu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gixqdydya.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gawrwllcd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gjiaveqyz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/govhdoiec.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gnjqgffnf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gmeyzfpds.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gcgomrzch.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gblvkbzij.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/glqsdobtv.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/guvfumtuj.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/geesoypmc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gegsyvfht.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gwhncnweq.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggqomagyl.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gdbjbuwla.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsrpwgv.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gbutccupi.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gkfebbqxl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gubxzlgny.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/ggkbshgjc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gzzczfoee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gfdihrdtb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gcytpxlhf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gammucskv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gpkbuwpht.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grzdltrzh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/ghlpeuixv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/ghnwrptpg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gfcswefrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gnbmoxceu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gcdlozprj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/giqhugsjk.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqrfmksn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gppjddtym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gdskqstms.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqwxdjnrz.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/grywudcgu.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gdmrtawml.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gnvhxiczw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gammbjidz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gojutqaeh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gixbyzzlu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gpmrupels.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gqahgpszr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gotjctlsj.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gpuhrajuj.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gykkytxux.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gvzlcptwv.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gxmctyexb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/grsevfdft.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gegtnkhre.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gvsfadxek.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glrkhrbqv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gxnioubsl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxlrgqcay.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gtsvcsjaz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gsgtsgmpr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwkrumzfc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmekzahyh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzxozgpbr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gxprrnqth.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gcskmxbkt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gsgffzgbk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gkwuxaflm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ghrdusses.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gidduxqwv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/grnuphaeo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gdbwyoqon.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gpsuofdxf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/ghqbawpfk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gsazmrybd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gwhhzupjb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gbkpzridt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gnyxqqflz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gkobkaogq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gunjmpmws.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/guuxjpwrd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gsnebpogh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gjvupkdab.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gcilxbfuz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gywqbspdr.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwisllpft.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/glpotaggf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/giocojmhn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/giwvmsqiu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gwohcakzi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gdlacltyb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/grcdguwfb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gquxpdwje.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gbgtujqah.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gajiaevxt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/geybjtoiz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gemxgykho.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gzsdnlxcf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/ghtdmjmch.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gvcqlvhbu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gliufcqqq.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gpaakknsl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/glmjramua.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/godmbfxso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gkmzlanjn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gobdikzbt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grmplojui.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmxmosalt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnyzzaqgg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmqatdfqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gopzfyrvw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/grsegqarq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gcbezlbmu.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gbfzoobzx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gfljghjfm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gbpkjoios.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbvofbzsb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gaefzggmm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gxfggtxcd.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/ghoetdohh.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gbfflbfec.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gvdwkvtyz.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gaxoyyiap.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gwzmutcgi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gopmomsoz.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gntqbkkeg.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gwjdifgsp.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gplyqrchk.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gctenkflr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gqjpptsmn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gyudvfyrh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/goulkdrbl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grtoxedmn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gksgxygki.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkeglejmu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbbtxkjlb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gzznpikcg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gptevhoel.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjgioacwp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/ggksrgtal.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gsmdiydfs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gljnzvwlg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gpgdszglt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gwcfspzzv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gubccpgmt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gimbyiimv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/giluvbnth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/grctojtrp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goqobeesk.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gxhdraycf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggygqqwak.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gowbozlxr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/goevxbbbe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gichgmyde.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gpmnemnsk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtgrlkonw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gshucvjxu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gamzxxnum.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvjzijpqh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glbwjsmum.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gfmcryfsq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/grihfrvnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/ghynipubx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gouiqnxlm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghtdokayg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gqjuiqapg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/grhdtwmxk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ggwkqewws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gdifueedi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gapklpnbp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gcelyihmv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gudfpmfrj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gjoniilbo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gehyrtdvt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gcfzpwlon.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/glkudzoho.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gtjpqiyoi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gresejboc.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gviiblvfh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gdmkreykr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gcpsygeke.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gtdyjojrd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/glwsogffv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gneylhcll.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvzizoixe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gujhravvg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjzzhnghf.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gsryeuxrv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gghyefiko.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvotrrcyv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnlzdpgbz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/giprlzosw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqckabrni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gjemccznq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkjeuzbtk.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/glcpxxycv.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gmkdrglpd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gacdzsxfj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/girhrnfyn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmjkwsspl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/girpoegnw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjutnljoa.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtzwkaxwk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqnjwijcs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtlnnoeer.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gfpzanewx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/glpiylxjx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzurefma.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gyhhceohs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gbnvfrvfr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gapbldvrt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/grdcbbfiv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gbfzuwvjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/goigkgsez.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gnqpqdhzo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gdrqmvdot.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gnqrjqczc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gpjwgbalb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ggwnawrxw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gnuqktsmu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkngrmlsn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsdjpaxzk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gtuaybefi.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gqywcharm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grmwimbni.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdznpiwsu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gynsloanv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gusliepjz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpiuhzlri.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ggsevryyr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkyqwajql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gpcqiboun.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gxkvylagc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gafhxfzrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqekzhwhr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvvbldziy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gropdktym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gxqzqlkzr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmadhlwyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwjohxhpg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gapqqxdkc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gvjrnxlgy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjdprkhgi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grmcqnyuw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gthpclqqz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/guozguulf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjrqozpss.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gnawwesch.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghtynqnmp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gbneaccnw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gjtxjvcln.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gloxbroic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/goxsopgwh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gkqmlmkzi.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gguahkkth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gypcqkizi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gvxljwupf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gvslexelo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gofztrmol.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gublibvmd.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gkjlhqbpn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gftzvcmdc.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gvpvdviig.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gecnpiohn.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxrqmjbzb.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/geteczseh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gjhyjczyr.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnqrpxyvs.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gjgieuttg.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gjvdpbanp.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghygutzqp.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gvnsclobo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gmuvffndf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbtvtvzuv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwhfvjrr.sHtML


<!-- 参考信息 -->