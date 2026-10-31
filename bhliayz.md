代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hc.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://og.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jt.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xa.chemitech.net.cn

[E02] 重复字符串
来源：http://wc.hnjuh.cn

Py:   "ab" * 3
来源：http://dq.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://so.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://bd.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://bd.panjiajie.cn

Java: "ab".repeat(3)
来源：http://cw.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://kb.lnxyls.cn

Ruby: "ab" * 3
来源：http://mp.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dy.huixiangedu.cn

[E03] 截取子串
来源：http://za.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ye.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aw.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://os.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://hy.colortex.cn

Java: s.substring(1, 4)
来源：http://nw.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gu.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://sj.wgjwhj.cn

[E04] 查找子串位置
来源：http://ss.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://tx.nszjky.cn

PHP:  strpos($s, "x");
来源：http://ao.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gc.huanxung.cn

TS:   s.indexOf("x")
来源：http://is.shxzukj.cn

Java: s.indexOf("x")
来源：http://tt.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://xj.bookmarksfly.cn

Ruby: s.index("x")
来源：http://bd.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://se.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qd.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pj.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vj.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://js.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xv.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pq.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cc.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pg.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ys.panjiajie.cn

[E06] 替换子串
来源：http://wj.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ag.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://cr.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ya.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://iq.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rg.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qy.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fj.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://pm.hnjuh.cn

[E07] 按分隔符拆分
来源：http://jz.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wp.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ox.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ea.9csxet.cn

TS:   s.split(",")
来源：http://sh.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cw.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lh.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://bs.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hn.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://cr.muxihuayi.cn

Py:   ",".join(items)
来源：http://oz.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://qz.huixinmuqiang.cn

JS:   items.join(",")
来源：http://sk.bookmarksfly.cn

TS:   items.join(",")
来源：http://eb.hahajie.cn

Java: String.join(",", items)
来源：http://qb.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://ta.szsharing.cn

Ruby: items.join(",")
来源：http://un.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://el.lnxyls.cn

[E09] 去除所有空白字符
来源：http://lu.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://is.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://il.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://in.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://hs.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://bj.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ef.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eh.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ws.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://zp.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dp.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ye.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://cz.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://ji.nszjky.cn

Java: String.format("%03d", 7)
来源：http://cq.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xg.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fv.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dh.yuexingan06.cn

[E11] 反转字符串
来源：http://dw.szxytkj.cn

Py:   s[::-1]
来源：http://gh.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://vs.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://bp.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://nx.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jw.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fs.muxihuayi.cn

Ruby: s.reverse
来源：http://ap.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ps.szsharing.cn

[E12] 统计某字符出现次数
来源：http://op.newstarts.cn

Py:   s.count("a")
来源：http://oh.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://bu.521024.cn

JS:   s.split("a").length - 1
来源：http://gc.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://gv.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uu.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://pe.haigaiapp.cn

Ruby: s.count("a")
来源：http://fi.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://tv.yuexingan06.cn

[E13] 逐字符遍历
来源：http://uw.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://lo.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://np.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sd.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zr.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uv.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mp.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vz.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jj.nszjky.cn

[E14] URL 编码与 Base64
来源：http://yk.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rb.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wp.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zp.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yj.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://np.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://if.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tv.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://et.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://xa.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pt.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mn.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dw.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cz.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dm.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yq.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://db.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jy.wgjwhj.cn

[E16] 数字千分位
来源：http://el.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://li.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://qx.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bn.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://np.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rr.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yw.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wo.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://hv.huanxung.cn

[E17] 首字母大写
来源：http://ud.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ve.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oo.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fc.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zg.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zi.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hd.shxzskj.cn

Ruby: s.capitalize
来源：http://qo.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wz.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://yk.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gg.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nj.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://te.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nx.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ov.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://px.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mq.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zt.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://ug.muxihuayi.cn

Py:   s.splitlines()
来源：http://hw.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ee.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://nl.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://hs.huanxung.cn

Java: s.lines().toList()
来源：http://ne.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://md.yuntaijiaju.cn

Ruby: s.lines
来源：http://uo.wgjwhj.cn

C#:   s.Split('\n')
来源：http://yk.colortex.cn

[E20] 判断字符串是否为空
来源：http://de.yuexingan06.cn

Py:   if not s:
来源：http://ml.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xy.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ar.asd995.cn

TS:   if (s === "") {}
来源：http://ed.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://hu.newstarts.cn

Go:   if s == "" {}
来源：http://uc.szsharing.cn

Ruby: if s.empty?
来源：http://zh.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zf.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://cz.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rn.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uq.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pd.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jf.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://so.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://zq.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mr.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ky.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ln.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yd.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cx.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tj.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kf.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ry.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rj.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://lk.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mg.lnxyls.cn

================================================================================
来源：http://iy.9csxet.cn

F. 文件与目录
来源：http://la.asd995.cn

================================================================================
来源：http://qv.wgjwhj.cn

[F01] 读取整个文件
来源：http://wx.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bt.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://as.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lx.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hk.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hn.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bv.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://uk.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ar.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ab.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ms.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fy.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hb.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bn.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kg.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lk.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://os.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ax.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://hs.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sg.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ae.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kg.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yx.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ds.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jr.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://yw.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ia.hnjuh.cn

[F04] 追加写入文件
来源：http://fl.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ft.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zt.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qs.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pl.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vn.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ne.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vv.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ga.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://wo.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://up.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://vn.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://pt.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://ns.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uj.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fe.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://oh.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://zd.shtwfgs.cn

[F06] 删除文件
来源：http://uu.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://fm.colortex.cn

PHP:  unlink("a.txt");
来源：http://mk.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ix.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yk.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yo.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://ue.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://hl.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://xm.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://nk.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ox.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nd.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://br.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hx.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://al.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wm.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kl.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gt.521024.cn

[F08] 遍历目录
来源：http://gs.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ak.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rr.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://sh.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://hr.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tz.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mq.521024.cn

Ruby: Dir.children("dir")
来源：http://px.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://hw.shxzukj.cn

[F09] 获取文件大小
来源：http://qr.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://zu.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ee.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://uj.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://be.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dv.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nt.521024.cn

Ruby: File.size("a.txt")
来源：http://wc.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ii.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://nq.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fe.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xc.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://di.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://sa.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wb.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gy.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cx.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qm.shxzukj.cn

[F11] 复制与移动文件
来源：http://cg.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ki.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pl.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ot.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ae.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gq.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://js.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cm.nszjky.cn

[F12] CSV 读写
来源：http://rz.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bp.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pg.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://my.colortex.cn

TS:   // 同上
来源：http://ij.shtwfgs.cn


<!-- 参考信息 -->