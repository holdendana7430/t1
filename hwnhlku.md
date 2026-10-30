代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gfscifvvq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzjpqefa.sHtML

JS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnmyvulo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbalzdrqd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnrdnmlw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjzokscv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbrpiybk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqojigpi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnnwoknf.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/geepxqzfn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gggjcflez.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmnmztiou.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcyggnhe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gyscslgzd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gxjitxqik.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsczvwmqx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gducziazf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gfejaykfj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgelqxgj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/glvgtjcdx.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtivdvxma.sHtML

Py:   "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/guafelmrd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guhmswbok.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbuepyrpb.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpdrfjgl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyjxqbre.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgbvgbmv.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmvodny.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhcowhc.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/garccvouk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwlrraeh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guanvfqxw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkxqfwjk.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmkeqnnh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxcccfsd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdnekyp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbihrxon.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnebfmkqo.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkvvptyd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynddrcqi.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fanxiaobao.xyz/Article/details/gotbhpday.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fanxiaobao.xyz/Article/details/gtyrxsgqx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcqxqmhk.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkteomgvh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafprthpw.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvigbzsbj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddllhge.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/giroifxyf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gozbfumek.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnupmexkp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/grytibgug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdmjvvgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwbaxtoo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnwtrwue.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxxvuyui.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gcjfvazde.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/glxlpfiye.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyymeisqd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbhuovd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfccoivrs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdqlalmn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhkvhvak.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzimlgkup.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdgslpv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gaihlmwiv.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/geusjeesh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkmregog.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbusrdc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gqfjnmjdp.sHtML

TS:   s.split(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gccakncoi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gotyziyqf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwjxrstt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzcgraeq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/giomfgesr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvqdntqo.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gapuvbpkf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxowzswmm.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gzjwyzshm.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpocofwjo.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/glebuzjvb.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkieedfn.sHtML

Ruby: items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyklartyk.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/ggugctedf.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/ggeclzyeo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgmfpro.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzozjznv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gmrtzkple.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuhvhhps.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gekcqlvnu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwukyxuui.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqhfdwon.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gwyajzcmz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/gyurvtnuh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/giswagjny.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwihbnuxl.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gipxzgpdc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfujvloh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvyydarm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqeppyfj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleqgggjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goozlivco.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goqrceasw.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrzwbyyt.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjgrzrf.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gdjjcrfbi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcegukvuf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbncmhdq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gbripglfo.sHtML

Ruby: s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gxkmsqrtb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnvpdzxs.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsdpejw.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlxzrtew.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fanxiaobao.xyz/Article/details/gwbecctrd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtmesjtc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gttgcuigt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fanxiaobao.xyz/Article/details/gbrreapyr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fanxiaobao.xyz/Article/details/gzyumbqul.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqchmppku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmejosmi.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/guvgfjbqa.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fanxiaobao.xyz/Article/details/gxmljobip.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqryayny.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwckhmzi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grihkukbm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glecvvlco.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpvukvxr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqawwrekp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbokehdwp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmsbwuiq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxzjgcfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaospzay.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkvxvign.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzxwdzpga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbrtnmzp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fanxiaobao.xyz/Article/details/ghqunfaeb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/gmybgawcx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gougjoegh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzcatvbn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtzrviytc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbbukol.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaggqekbd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gauagistm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gepgayjsu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/giualhhyz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/geilzlpqk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfthviqvz.sHtML

[E16] 数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxeoovbg.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gowwhzceh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbdkoqph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gacdjjzbc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkluxqk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhlsdzas.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galiexbun.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpdlfhjp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fanxiaobao.xyz/Article/details/gfeofxlku.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmytncnq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsqxebjf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmzoojdg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjiyutefh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gptkmnoey.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gizmhuqsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcvdunvq.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gesnhmluu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/giudigwlr.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypxvqeyo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gdlxutibf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gtlcijxfz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gecjsfzif.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogvhtok.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmpeusyl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdtfzipe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/giaefiwbv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gypsayhac.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gvdzkrris.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjxayxlw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehwcgmlj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/guwagxzwy.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/glvxlenvt.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gebvqllhb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gygeylsfw.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppseyvdc.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvwsdagk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fanxiaobao.xyz/Article/details/gpioxvadd.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gnlffswro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrupqvzj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkzchamqv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgggipef.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwogtvtap.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmintmmy.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/geiznbefh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwciwfux.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geptuzzmt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gykoktekq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gmyizomra.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbqombms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwygmvgsc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsencyy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gblfauygn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/grorbwxpr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gmdhlenvc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoxvqlct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruczgnts.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/grumkomrv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzjvdwhh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gvuqkegoa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyrsejbl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/guojbdmqm.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugbgqgv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gusgsqube.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gstgaobrg.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvwjkezn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goqorheom.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gayzduyjl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmjlpivb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ghpeseiud.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gtthwofah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gmymodnhc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gcexjkyec.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/geyjvupmb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gglltqjzd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqaknctc.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guutmthgn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqynabu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbdfbxn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grpijjctb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghctedtsc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqciepdpm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gommazkkz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gdojowzgu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gduvbjrjg.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmmkxznx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdqgiouh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliwtzcce.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdhgwvrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbhpccy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhomnkos.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnlsdpkj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guswadfjb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghynthmcu.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/gecawtuyp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gkfbivylj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gkeepiffy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvfnlnhf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gkyslknsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwnasib.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrkrdasv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwvumfzm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlrhbgqt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gojbibnjo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gmpqlggek.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gtmtglost.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvruxjaux.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gyzotisgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzkarkjdw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqzcxppz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gmsrkropv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gousazjvz.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/guzgglyvy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gusokuprx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gengubxkw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gndcdipyk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqlqisasq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gknazylnb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhzhxjcc.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfojayleb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzaydclo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/genhzctnn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/glvdfmrqd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/giuxczmev.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/ghsrtnhbl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gbnjpjuch.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gawqhbfnd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojipeed.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhxqpjhg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgolhjgw.sHtML

[F08] 遍历目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gycwryrfs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwguxhm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guqrfnnei.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyhubxoi.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvzlmssj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/goydlniek.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gwbrpvbup.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gdmgcyxfh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmigdfbwb.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gdcicyqto.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwaoeof.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gkjhljpsu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gvaubvnto.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gelrciihq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgmgihdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gtjibxpri.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gwmcvycre.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskjjsbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyfkmagk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gelzqyjup.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/grvaobjbw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlskjnkm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/guggaozqi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzhoehkb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ggctsydra.sHtML


<!-- 参考信息 -->