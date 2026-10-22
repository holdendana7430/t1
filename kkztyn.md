代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2erbbfmdf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rozcxebp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ipwmcrqk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zmvmbzvv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dmdnisqb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kkhdgspo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oivwtqyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bhzicbsd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2loyxhpql.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tulcikem.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ggpuoyui.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iodpcgqa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kzifsbji.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2szeottjn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cbqqstza.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jofaehyi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2joejeknx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bthjvoqb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tpdmdudz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dqyrlygx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xuzzoobd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jpahofwb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkxngaqi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jovcefry.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2doaoawzs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ubimuiyp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2duqmgpfi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dcrmvsaj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ikztilzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jglvsazc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2esltpkrs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2esxsnljh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yeoqypry.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfguzcvd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xkawkcbu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gtfvgopn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2llnocwuh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fddrwmla.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2eqpfxbja.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smspzart.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnrorya.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zlsikgpz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kofkqyvk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cazbzoor.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rnmlssaq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eceeakkt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qdssnyts.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jeyznxzc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nlejvtfo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bspztcaa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2udnxlssp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lgfvcvwf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2szbqmdto.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nocxikcs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2toizgrgg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qmjncinq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2akltogzw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhiyksxh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pzqjhjjz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jdvnlyog.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpujoog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ofuquslp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vgqedsqo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kuicyncu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hvpqniqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jfdckthf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uhvjwmym.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bnywyqzr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2farbpomw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2twwyymjy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2awadaisk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iawvjxhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dhzbufcf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2poxklesz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fftciofv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tevsrnfw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2chkxzmij.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkotye.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nzgpgxtr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iwuvmdke.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2heviinpy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ypfvfuie.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vxwfyspx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mzdpzfcq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2spdtzjnd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lsbkzluh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ufkhxmin.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qyrhcrgl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yeuhqbmu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vlvmlnuo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nlawrigr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ltvmvbzo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2deqcodjx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xzkmazbg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yenejugp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xhmqwwrq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbwfvlnt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2grgbkwku.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2slxbgfzd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbsvyxkd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ehocqxxn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vtajhedv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wzoywxep.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2deejdduw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xsyzfflh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbrrzcc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pzbthpzx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aykhjlnk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fofaizpe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nqhxdtdr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blwrxvtx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmsxof.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2chrclydh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxbknx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ncegvyvz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhvqftd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cjlbgrgj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pmkbpnws.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gtkfdhbm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jtrocejy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rxfjqgal.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pikbaoiz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jiaxszgu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pqjmvaiy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pkikdbwz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cpyegmgm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qeeritxb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qujubjhd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gjokvlkn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyfvduo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zmjjclex.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qqwltxry.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gawjtqnd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nueuatie.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hityhyoc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zblzvzax.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xcaxfmzq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lwwaxlcu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tnnctzmb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkuomzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfucifrn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vvueqgjd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ludpyfjn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tffthysw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjjsfyqw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2giqrlzof.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2akuymoju.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgiztwuf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lsnzgjjv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2alumxnlc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vcvjpsko.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hydnbrmx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2axarkrkk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lpkbyico.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2eegimgpc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gxnasbbc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vglvwrpv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ckzltvdd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jbozwecj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgajmgyo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2esfwgqlj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cncilojx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hccsmbwq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bbqzgwjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gyhuxuoe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lfpsjztn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gczupkhg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xfnyqolf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xlvwiwlx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mqzknujx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2poacmvhn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eqsuhqlc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2frqavffd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsveloa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yavlphmg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dedsgowx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uihecuxo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mxhaflex.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ygkdfyhn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wmvonlqs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fbwioaqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofcyjkpu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qoostqmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikacmpwq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvejqndq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hrtvehst.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ipazixmh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fqifsczt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pjhgnwqn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2orrammrt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wbxmqbqy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijboanbq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phbuqyhy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zschgjul.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vhwdgukp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiirsybj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxpfdtos.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjlwjqql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ujisdaoh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nugonfou.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pbcnlsyo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajznulwy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zemdezfu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ckwrdrri.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2czvcmjht.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vialyokr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2grappdjo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ppvlkvrd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2scggiyry.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wyuoocgo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dfzwfpzq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2aulnonwh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ciavxqam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pblgxflz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zyvhtdoj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnyggban.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2apdlrfir.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rhkqupnv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fjyoegcp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rftffrkp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wvvkexlf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mrueagfz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofeamuww.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfsepvfp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtbugrdn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xmurfswx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2keshwdip.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbygvsvy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nssmfcgs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mfphunto.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uykqaaqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmexritu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xitdfpuf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpgweshi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hjgywetw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsapufpz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdspfnqj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xaidcqis.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kaxujiau.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yxldegkd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vtdkkiwn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pereyzyy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vapwlnwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2urpkdwys.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2omrvjrhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwjtdg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xqcqzvwa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ylsmfitx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hurfsxnm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2plknrxqj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dmnenhci.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oioxyylh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sgdorrmo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ywxybnko.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rfvfjeqz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2utgdfmax.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2urcqazfk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvnerhyi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjmleonu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2etxqczxv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kgvrqemu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2miphngoz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2khhfwqlt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmowxuno.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bukdsvme.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tmlmznka.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eblhmwov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmtmajqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iawfhlud.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esludvlq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cindeihf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvlxgwmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkcmnyoa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlukbyyf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mbcvxebl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwnmtpjx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqpnklpi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldsbvuqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uninhaja.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2whplsxpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sjvlgvlw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuiseudx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rdyqewsv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2brzmnmyk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrspoks.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ciwjmtdi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jeefulpl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ideabkdx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mhrqucgv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pvuraeji.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jgtrcffj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sguuzici.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfkajzkf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hgtfktgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxmcqdic.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2isqvkunn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pahkuwtk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dipiivpm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxhtorgg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejybfzyz.html


<!-- 参考信息 -->