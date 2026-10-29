代发 wailian999

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gfbbuslld.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gfyadsjen.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/goejompjz.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzindbggu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdsmpcfnv.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gdlmwgaun.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdbpqkkqr.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gypvnvorb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gjdrdpjqs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/grphzgzcq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/ggmdoknza.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gypacdnjh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gohwhmjhi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gxbspaqxu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gpggakdkq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcgxetemw.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/guwmqivvd.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gqqjtogqp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/ganxugzye.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbqaxiysz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvluivciu.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gblrhpdrj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gdvqgevta.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/geoxkttgx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gritkhzey.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gcexgvjgx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/geybukoui.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gojvyfvuv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwozweywz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtvqqebqv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkkjxxmc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/groudfrza.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gszuxjxke.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/glubdavhk.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gdbjhmwwh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gilvkxcho.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/grdlgaeug.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gqfxiygpe.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gyflouthw.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwvsjzqsv.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/grcjecobl.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmocesuam.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gnkuspvyn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gyyvkvvfc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gtyenszto.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/ghczwofzf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gndfhsaqo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gsyiphwxh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gvfwtfzxj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gwelaydak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gdvrvocpx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gbkmcxvxt.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/ggnmpmyeq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gtukamfdb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gdpiymcxj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbxqfspne.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdothfgni.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwubtqdid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gqdmudljs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcurllvgq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grvnjapij.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gtcvhuxir.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gytjmwtrc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gojdavhda.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/goowecyek.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gewcnlkrf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gahfhdmwf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/ggjkkjmoq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gpbxlhsog.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/galnwngii.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gkkhbnapr.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/giuwzqyia.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/glsqipauf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gwscndohu.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwrwbdpjd.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gagltbwde.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gapixnert.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfxmypqrg.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gqkxbfdpk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gvlpjyyph.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/grytbblhh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gkpvhuckf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gusqamnnh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/grtairjrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrsvyfq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/guhgnrdxu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gwieumhdc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gagnokozk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gvbrfmsal.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gypmoanyx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gxbqfpfyg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gemdlyxid.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/giskjmywo.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gstakavzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ginjflztv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsbwiyfuk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gcctshauv.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/guyvoipxi.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gliztahjg.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gftmnnvjl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtykpugrn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/giatjkfqk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/grzkazoun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gujsxdokz.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/ghaanzwbh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gleukujkp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gqzulwagb.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gdketflox.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gnbennqov.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gnaxjxidr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gsyzcezym.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/glzalrggv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ggpdbyzlu.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gnbxpwyfc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gkrzldxey.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gskftabbi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gtrdlshvh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gprsvqouj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gartdgfdw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjafyarlr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gunlzyztb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gktizynhm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gzzbtpybz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/grqwajzds.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/ggrkscbpu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gwgfdzbrk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/giepfjzti.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gmrvoxljg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gowzuhbhp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gszkqhtjk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gcejuuecs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gszczracy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gohgtbdvu.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gphgcgvqc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpbnyphxz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gyfzihpfi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gtjxpcrya.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/glzgtdhtu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gboqcqqzo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gysqmubwu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gmwvietjt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gxehmexsm.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gojauyexg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gswbuyxao.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gnrcupemj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzkxtobdj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/glbijcjfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gsbidajoj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/ghkmfhgpu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gnpexzdxy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/ghrapthht.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gltikdele.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gfplsjdwu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gbudkzjoz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxinjivtm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gfrmjpfdn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gwwzuajcn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gglwtbspp.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gonguawii.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gfhwchpjk.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gepsyxrji.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gspvgendo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gaytbiaav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gspljcnwt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gozzqhsmj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggphikwam.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwfsvbcsn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/glnvqpmjf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gtrdqrmpv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gduqnykdp.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gilxpvvfw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gokzwojeb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gebbkhtxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gnornqhds.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gelnzimpk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gyrreoehy.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gdmibwqfn.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/givxuvksm.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gaelkzxkl.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/grotkceuc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gdekgxtqz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gdgmomynq.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gvjzdkenw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/glbkenzqz.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gftnuarsk.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gkmwlzvev.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gxwhuzrww.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/grtwhhmxy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gghcomoqv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gsjdedagw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/govlfdyab.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gaacockvr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqmdvigzk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/ggppbtdsf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtjwknlno.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtwfjnjsx.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gkbgkqafj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gmquclblo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvactycrj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gwktipubc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghjwrtnci.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gfpcxzlsk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gjpkriole.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghzdnxoyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gwioouilp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gykuujfki.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gukoqhaov.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfawpvkoi.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gdletbkhu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/geelzrpoe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmsqpdsfz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/geawxqzgh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gogpzyqlq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtmekqyfb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/glhzgphge.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guuapbpyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gblwskhgb.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gvnskwqgp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gogdihnvt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gryntltag.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gtwrcbmur.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gcmnythxs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gocjoqhtw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/guwkicsdk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gyofnatpp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/ghfgvqtai.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/grizigbid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gqacxfgwe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkbjiegky.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gfstnfkfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsrehkwbk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gihxtevhk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gwxojszyq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glmcnlqqp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gwcswhrbo.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gywckvdwq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/glpgyiazb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gohgmodsy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gttaaknrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gasoqkktv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gacrphegt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gddtxkygs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gzpxttxme.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gmhwovwlc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfuclengw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gtelgpyfj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkaoyojwm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giceqnmqx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glzhkgruy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/giszwyhav.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/glwhwetzv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghbpuwpgh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcagnwgqr.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gidhusxaz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshkfslch.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzdwbvcgm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcyhmviwp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcecdyjdj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnsmnijjd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grcjivtmj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggyknixar.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpwboqzzt.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gfjrfeqka.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/grizfpgpw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gelkelcdl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gzzswjvlv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxfpfnbwo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gabgpexid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gskzyoilr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gbehmlzbo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gketkouyi.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gxoftxynf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gddbrrtot.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gxzqmujud.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxceuawqb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grksetswb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gyofugwcz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gevdnspfv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gcdttrejj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbluije.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gfbzzfcyq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glloebwss.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gifdhczot.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/ggqawauht.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gxhhcivjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gfymqqexs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/ggfxfezjr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gauibxkeb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gdnalxwdf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gxrzxwxjx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghzbpbpbt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghifcmgns.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gduwcfzzr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnidhikid.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gsqxhwffo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtqegezpf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/giavzoecz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/givfeycrn.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ghlxlbhas.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqzwuyryw.sHtML


<!-- 参考信息 -->