代发 wailian999

================================================================================
来源：http://tw.szxytkj.cn

E. 字符串处理
来源：http://yg.hahajie.cn

================================================================================
来源：http://iv.nicolike.cn

[E01] 拼接字符串
来源：http://ku.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wo.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ie.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://na.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hl.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://au.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ce.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xi.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ru.jianghongdianzi.cn

[E02] 重复字符串
来源：http://er.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://wx.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ny.nicolike.cn

JS:   "ab".repeat(3)
来源：http://na.asd995.cn

TS:   "ab".repeat(3)
来源：http://sp.panjiajie.cn

Java: "ab".repeat(3)
来源：http://av.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://bt.huanxung.cn

Ruby: "ab" * 3
来源：http://xw.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wp.nicolike.cn

[E03] 截取子串
来源：http://ou.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wf.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sn.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dm.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://uz.nicolike.cn

Java: s.substring(1, 4)
来源：http://ih.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vs.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iw.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://sz.shtwfgs.cn

[E04] 查找子串位置
来源：http://lo.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://qo.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://sv.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vj.521024.cn

TS:   s.indexOf("x")
来源：http://mh.muxihuayi.cn

Java: s.indexOf("x")
来源：http://ke.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://cp.panjiajie.cn

Ruby: s.index("x")
来源：http://ww.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ld.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qz.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nf.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qj.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zw.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jf.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hd.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wh.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ko.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://to.bookmarksfly.cn

[E06] 替换子串
来源：http://ez.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mi.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://gz.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vs.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://bl.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nz.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ko.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ee.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://pt.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://so.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pd.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gt.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hu.9csxet.cn

TS:   s.split(",")
来源：http://ha.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sj.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ha.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://an.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zx.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://zm.shtwfgs.cn

Py:   ",".join(items)
来源：http://pu.panjiajie.cn

PHP:  implode(",", $items);
来源：http://hl.hahajie.cn

JS:   items.join(",")
来源：http://nc.nicolike.cn

TS:   items.join(",")
来源：http://st.521024.cn

Java: String.join(",", items)
来源：http://pg.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://pm.newstarts.cn

Ruby: items.join(",")
来源：http://ug.panjiajie.cn

C#:   string.Join(",", items)
来源：http://ye.lnxyls.cn

[E09] 去除所有空白字符
来源：http://wi.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dj.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://is.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://pv.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://tw.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://on.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rq.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bf.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bd.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://bp.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nl.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sk.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://ep.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://vi.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://mc.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://if.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ir.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vh.bjjhwx.cn

[E11] 反转字符串
来源：http://wl.hahajie.cn

Py:   s[::-1]
来源：http://bp.gzmigu.cn

PHP:  strrev($s);
来源：http://jl.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://yz.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://vw.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hv.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ne.wgjwhj.cn

Ruby: s.reverse
来源：http://cp.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sc.newstarts.cn

[E12] 统计某字符出现次数
来源：http://df.huixinmuqiang.cn

Py:   s.count("a")
来源：http://na.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ix.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://pt.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://qz.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ms.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://tt.haigaiapp.cn

Ruby: s.count("a")
来源：http://nn.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://dk.9csxet.cn

[E13] 逐字符遍历
来源：http://op.asd995.cn

Py:   for ch in s: print(ch)
来源：http://za.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yi.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zc.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rf.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sa.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kl.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lk.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yk.colortex.cn

[E14] URL 编码与 Base64
来源：http://jl.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nh.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tr.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yc.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hs.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jp.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gv.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kn.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bq.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://lx.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bu.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kn.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ky.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pe.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aw.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bb.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kg.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ud.huanxung.cn

[E16] 数字千分位
来源：http://wp.hahajie.cn

Py:   f"{1234567:,}"
来源：http://tm.szxytkj.cn

PHP:  number_format(1234567);
来源：http://bc.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gu.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ve.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pv.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://by.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://du.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://fy.9csxet.cn

[E17] 首字母大写
来源：http://jo.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dr.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sx.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fj.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sm.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zu.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ti.hnjuh.cn

Ruby: s.capitalize
来源：http://ij.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ci.jctech888.com.cn

[E18] 模板占位符替换
来源：http://lo.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zy.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://la.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vp.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ax.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ud.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mu.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://do.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://me.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ue.newstarts.cn

Py:   s.splitlines()
来源：http://fx.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qt.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://zp.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://nn.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://yi.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://sa.huixinmuqiang.cn

Ruby: s.lines
来源：http://lz.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://ma.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://pq.szsharing.cn

Py:   if not s:
来源：http://ze.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fs.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ct.asd995.cn

TS:   if (s === "") {}
来源：http://fh.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://kh.shxzukj.cn

Go:   if s == "" {}
来源：http://ym.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://wv.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wx.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://dd.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ul.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nc.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ns.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aq.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vf.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://xb.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ia.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://db.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://uw.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ic.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gc.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sa.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nn.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mp.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://uk.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oh.9csxet.cn

================================================================================
来源：http://lm.asd995.cn

F. 文件与目录
来源：http://vq.hahajie.cn

================================================================================
来源：http://fo.wgjwhj.cn

[F01] 读取整个文件
来源：http://ug.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mc.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://vi.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pp.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ir.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kl.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qy.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://yo.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://ph.szsharing.cn

[F02] 逐行读取文件
来源：http://uy.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ke.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rj.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gs.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ea.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zd.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ql.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ln.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tt.colortex.cn

[F03] 写入文件（覆盖）
来源：http://nm.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vg.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ia.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xp.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wh.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ut.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cs.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://zc.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fm.szxytkj.cn

[F04] 追加写入文件
来源：http://og.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hp.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://il.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://af.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oi.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qr.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wx.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mp.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nn.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://xm.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ph.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://bd.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://oy.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://ct.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dr.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://eu.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://cd.bjjhwx.cn

[F06] 删除文件
来源：http://fk.9csxet.cn

Py:   os.remove("a.txt")
来源：http://sh.9csxet.cn

PHP:  unlink("a.txt");
来源：http://mh.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lg.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yj.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ch.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://zn.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://kf.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://cw.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wm.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://md.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fm.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bp.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qk.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zr.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ji.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vu.szsharing.cn

[F08] 遍历目录
来源：http://rl.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zw.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xc.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://wy.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ny.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://my.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://am.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ol.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://rb.szsharing.cn

[F09] 获取文件大小
来源：http://aw.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://do.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://yy.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://li.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://hq.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lq.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tc.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://cv.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://kv.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://rp.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://me.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ke.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sd.colortex.cn

TS:   path.extname("a.txt")
来源：http://gp.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ht.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dq.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qq.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://um.szxytkj.cn

[F11] 复制与移动文件
来源：http://pb.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://su.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hc.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ys.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cj.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zc.szsharing.cn


<!-- 参考信息 -->