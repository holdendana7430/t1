代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/ghqymcpde.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gazyecgas.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gfbkoracy.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gniogbwqu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gglorqckm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvyrxiyvn.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gdxymezsz.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gycnykosg.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/grqcloeas.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gpwovtksq.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gtaydmlyw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gahevatpm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfinaouwz.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gkcaemjpa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmhbbyzcp.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/ghylnmzrg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gcgdpaxuf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gdblvahie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdfpgbqbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gjunjlxwb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gifncbtlh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gxyifkiwt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gxzrmjspu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdcrjytpl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtmxkehev.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/grloitbcr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/govzjldah.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gpgpqmwtc.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gslflmszn.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gqmadywhy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gmciirhzx.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gplrdeqaw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gjnuxuplp.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gpcytbdxc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gudjwwumv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gishkyhae.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gkfxhzvyh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gmyrmjxut.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gipjfwyvl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gcpnbcuzq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gifdaodzb.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gxhdenwvp.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gdrcffjjt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gvwdfgcom.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gwenhwwfo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/ghbfmnnev.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvklikeuy.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gccnjzdtv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gxesnvmna.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/ggwzuyyks.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gynxvtbie.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gwfuiskco.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gkfobgael.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/giltycqyk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gaxthrzvd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gdslisreq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/giiyxvzbd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gbxnuhltb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/getzgsgdb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gadauzeqs.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gpzglapmg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gzbthwcjx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gswflcrrs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gapeejhyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggfwnmltw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkrrvlmke.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/glgoozmls.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjwsnqwxc.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpklqdzhl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gbmaledys.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/giglbltix.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gafpvvcdd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gexmybczl.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gdiceglfw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gkhbycywl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gxaoiwvbd.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gaunniyhe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/ghgcobpdn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gihxlbjhr.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gsqfpxtpg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gyyqbcjvy.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gaiksjbyl.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gylnvxabv.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gttmdbflo.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gcatyjemw.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gjjsffndh.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gwugewgug.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gugefkqkg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/giwnippqy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glkwcbbfn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxrxiwu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gkrslgspc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/geyczwhoz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gadqmztob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/ghakzyzzs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gwwxywcbe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gmkufekmv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gcyhmkzhz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gcnczkxoz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbhyytbnl.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gprncyswc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gppqdoyzu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/geqvdtobg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/giwikfhty.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gxcfbvawh.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gtptgcmzi.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ggwdghlpo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gaxbxrctl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfgzsomvb.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gyrgqnalq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/guxsyhumc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gxprsquwm.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gshrktjoz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gydyfvtjh.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gbnohunay.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gqreqfayq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gslmnkhor.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gudxddiib.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gnngahxyc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gxhqbhpoe.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/ghwzluivr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggbmerodo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/guxrgarvx.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gxavdvqzh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gqeavzugo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gusdkiirv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsucdxkss.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzopwbjwn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqymqurrf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gfcklsxjk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gkoijvmlw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmcdlwquo.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gvikotbio.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/grgewxenl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbldzhujy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gelktdvoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gfusmrhlh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gslrlilro.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/glgpehhai.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gaxhqtzwf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gczidfiiq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gasitmcna.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gqyptqwok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gmyhuedyd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/grkgugzca.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gdkqvjhcn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/givjbemwj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gndohkzmt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gtjasrygn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gnbcdwpzz.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gfnapykam.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gsqdeqmcg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/guqjdpibo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gxssdzjop.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gvmjczizk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gxbxbbnfv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gphbiqylg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gmbvqnsaw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gqdfiylix.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gawjjhlmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwwhuzfkn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjvkjzmdr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwfaopscv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gohlsvpkz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gpygcaotq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gdbakewsh.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gjfsgzzyx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gyobaamzh.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gxpsqokkx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gtjtiyucy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmittogak.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvgqwfjsj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gidsonqly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyjpegwtc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghlhjcpxk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gigsvavxa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gpvqalcpk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gsxpmvdbw.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gmputabyj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/glyrfhcmr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gdvygvqrz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gvmsgnpso.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/geetjajyj.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gjtqdpqkd.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gbwjobjny.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gonvwjdfg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gnfeehcvt.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gphtnbnxj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gebumbcod.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gcbrimeyh.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/ganvizgly.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwqrrscnd.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gkhwzxbqr.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gxhcvqfbl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gbbfgpdvx.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gapulsict.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/ghhctudcr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/giwvhfvtv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsynlvutv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghuinkobs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqpgpxifd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/giubamosv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwtvgaied.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gqiwckgta.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/grbrlstgp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gcpxnythb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxdbtfzgy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gecdkrrwu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gdkkediok.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gygfajnib.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gzhermcaf.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqflnxyxw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gldjafapm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gerjqxqkg.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gqjioxtkz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwokaamnh.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/grwgusgxv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxzksfnnb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcojjppfw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gfjcwhyin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gztlzygcg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmjhtwzfj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gvgaezxus.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbgnvoiur.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdtvepidv.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gvfbxocat.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gnxipjldd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gcuydaclt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gmgotdrsf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gctjwjsuy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gtvhuwoma.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gjzsegsfu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gcilfyutx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/givjgclqs.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gvaorflxq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gydsqhiie.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ghgshsgwq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtjpylfsq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gejfvkhux.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gsfurrwfj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gemupdxmh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gsiefvlcl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glbstorvo.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gnyyihvvg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gwbzjxfoo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gziiymaxq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwkixwgic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gpwgoeryn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/glpjoqrrh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gdmxadouw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gwjbvpxby.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gqbvvrzlh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gebwbfbrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gpgusozyz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/goqyptxts.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvotldlja.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtkyblewn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gawbendrk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gfscomxgn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gziyeeobb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwzubsdpk.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gwwthavox.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gifeneify.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaamjytns.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdzgzbzkj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/govwukvwx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gsjeyoowy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvrwvvohb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghngqhclu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtveotdii.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gwqpqjflz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjyieanfo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gjjyiwaje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gudkchhpt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcvbhsruy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gjokddcii.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gfmyrvbxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gzhujyikl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/glqumwbqy.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gyaxcqsur.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gmbkgncxd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gsjmuijdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcdijiywg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjdyebjlw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwffrkcjz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gawxjdybk.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/ggzzmgadm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/ghzpgzczd.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gteslrksv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjhwkjzrj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnnnuiigw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gubvpkuok.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gykfgdegp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grosdaicm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gqfrpuivz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqhbtekv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gqderbuob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gxzywdmuq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glejswlre.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpayxnzjr.sHtML


<!-- 参考信息 -->