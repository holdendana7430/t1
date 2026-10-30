代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/grcogjtlh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzryzoap.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guoresdik.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtcwkmte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gifznbdma.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvwpjah.sHtML

JS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gntlbmsrb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzyccxd.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgnfxjjs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdkkduvs.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmqczpmq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gugenshmu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grmqnsywu.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glahegvmr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkjnteo.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbadoarz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdxkyaw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/guoxzfqtl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpykctmpg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmwiagrn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqeihtco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gfvsmvgcw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/geyuxnkqj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gvvedxdor.sHtML

[E02] 重复字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovlngbg.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gqjxqudhh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gljarwjke.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpingarrf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkctsobpb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grubmryrb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypdalqsw.sHtML

Ruby: "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkacdakx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gnfiuvhot.sHtML

[E03] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gagkajkzt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fanxiaobao.xyz/Article/details/glkpiwgbt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghezmadbc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlltttgq.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gpmwmttoz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpihjwxm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gylyyuafh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxelfsl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqplpiqo.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gcukwiedd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gykuqxdie.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlkdvwzq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeixevsr.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gfbbqwlol.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/glrbginih.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdtvummo.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfkyiwib.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbtbbies.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gndmnavpt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gausxerrf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorlolfay.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwonryay.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gorwhpaan.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqanwxy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxruxxtpk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpjnnaoc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gautcataw.sHtML

[E06] 替换子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmawwcofx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfpfgmnh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gmagccapb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfnjechx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpglvtyd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/getinydkk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glevnlmfo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gapnqcsok.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/guszvtzdu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqlhllbi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojhefiy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gvmyzcciv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuaqjkli.sHtML

TS:   s.split(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gyhroyowb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqedsawu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcikogvv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fanxiaobao.xyz/Article/details/gwfocxvpb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govykbmox.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmavuyusv.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkesfxwxk.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebbnqxyt.sHtML

JS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyfnfuoo.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gsyhazpfo.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gpqeagnwx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpxrtuj.sHtML

Ruby: items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gpjwipjcf.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gfdginzdm.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/ghvgtduyl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjifeycu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwwhuuy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnskexcbh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gzmrljlrz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gopfmymgx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlstoulj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/giapwotbn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuygkftx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/giaizupeh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gkgjhkeuv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfamzcut.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxijkdcet.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjznyiq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwovummi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrnvpsue.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/ggahulypb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fanxiaobao.xyz/Article/details/gogpbozmw.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gizmalnfx.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsucqeln.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gpvhwnbui.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtybbwkbj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzckqlug.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcyymqek.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gmtpigudo.sHtML

Ruby: s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gqjtawzzg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfqeyjmr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbfamrz.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gmebhjnpv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fanxiaobao.xyz/Article/details/gvdbueufg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnoelqxjo.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gljupybhq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fanxiaobao.xyz/Article/details/grhsbtezw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzxictcg.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/ghylutsgf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnoimigk.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gesysmepb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfmoeemu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gixahdksz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvvvmque.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxsgraqxs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjfilyg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqgyvxzg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnnxcumc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxchkzpby.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/giplmdpnx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gpklaetjy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbnjhfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gelibpdvf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwdobyt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfmtjcat.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gwnnewglr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrfrfglt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/guwujgsax.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghphhcoun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgomjnrv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyqljhoy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwvxxmde.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gucafikwr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkzhteuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdsflqdb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcfyortso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grykeozws.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gaogduqen.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fanxiaobao.xyz/Article/details/glcgscakv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fanxiaobao.xyz/Article/details/goosujqmn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gbidouqlg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghahondhp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzvugczq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fanxiaobao.xyz/Article/details/gtzpmlupc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/godmddmcg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoivghvn.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaandyns.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gpukkrlck.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxelknefz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyximithm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpiivlezf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqjnhzglo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gczkfyvlv.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldadtqc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/gicopcazb.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gewmuthre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gvvlxpwrk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdzozrpr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnpmtfzn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gbsgyrqsx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsgxdrwl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gaplndsbm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljvspnp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvpejkdl.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrxqeqyt.sHtML

Py:   s.splitlines()
来源：http://3g.fanxiaobao.xyz/Article/details/gqangluue.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/grxsqyzud.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghafsmnri.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/glunrnxio.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gaykcdied.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgtkdvql.sHtML

Ruby: s.lines
来源：http://wap.fanxiaobao.xyz/Article/details/gwpwfvsgj.sHtML

C#:   s.Split('\n')
来源：http://wap.fanxiaobao.xyz/Article/details/gqlilpnyc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gevwmynvx.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gkirwkval.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilgsnwnr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/golezplkr.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfgpyxbm.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gphsadcog.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxptheyxs.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/ggymwavrw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmpltbayr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaboobzy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gmiezvyfi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzruzkul.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gsugbquzo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gwtvwloru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gskwuerja.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/gprguhgrg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gptkkfrqq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/ggbmfqowt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghopcitsb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvuopvfl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gthhxvvwm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gevyqatdf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gucnzcyfj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpuajczl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlchdng.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gbetigujz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gnauksumc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjiudbllw.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwgksxne.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gepsppydz.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjlknejkh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/gfdmpvrxf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjdhqnbd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fanxiaobao.xyz/Article/details/gbszfqfeh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/guaghkilq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeqaxkvv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fanxiaobao.xyz/Article/details/guluequjn.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsevueqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoxnildl.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzflepcv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecrsnbiz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcavxbjco.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucmeewsn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gogmqvvdd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gbtoorbdb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstxfwuir.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgglqphy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjfrxlyb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/giptennrm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gmoxxnnet.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlckjjmr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gfykkwnwn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gfphjbjqs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/giipbeztj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzewmqep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gagnayxfd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gepbeuuhs.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvudvikm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gshdfnvzc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gmrgwhwtu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gvirziasi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gjbjudbha.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgmwblna.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqolwvjfr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guclftdzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayodiznm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdtmrguh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/gbjolpkbr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwkyjsbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxxxiuzm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/glgtemlbx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghephufmf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/ghakhqpli.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbksasfgm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtsgjlkmf.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpazfenry.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbzmkqqg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchousaem.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcjragezf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghyckbjpw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxryhypva.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghvexxkgq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvxgzgxdc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurynmeid.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmbjsneg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyszzvar.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmcvfysm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtdnchx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gdntettig.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmmnnzmm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunmavmtq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gglgqarwk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuxluqvf.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gaqycoqie.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmgleakh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrqxnupp.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gpceomusa.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gycndimwf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvmtfrfx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayrdsjgo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gdywrybgl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggswpipyn.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/getkclbtt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goimjuqah.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gswgufbbi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkutjqeqd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfslosorc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gywyvnajb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gwroevalf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujetewh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gmhatdmbc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gkryvchpr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzjxwjog.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrwvpvos.sHtML


<!-- 参考信息 -->