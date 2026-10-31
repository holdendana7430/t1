代发 wailian999

[E02] 重复字符串
来源：http://wt.nszjky.cn

Py:   "ab" * 3
来源：http://du.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ff.hahajie.cn

JS:   "ab".repeat(3)
来源：http://eo.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://pa.panjiajie.cn

Java: "ab".repeat(3)
来源：http://sm.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://jj.colortex.cn

Ruby: "ab" * 3
来源：http://yy.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nd.wgjwhj.cn

[E03] 截取子串
来源：http://hj.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qk.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sq.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sa.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://rs.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ng.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ig.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gs.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://ve.newstarts.cn

[E04] 查找子串位置
来源：http://xo.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://cr.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://rt.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bt.panjiajie.cn

TS:   s.indexOf("x")
来源：http://et.gzmigu.cn

Java: s.indexOf("x")
来源：http://tk.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://zg.gzmigu.cn

Ruby: s.index("x")
来源：http://sj.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ts.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ma.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hc.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://we.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zs.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lf.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://co.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ed.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iq.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fi.huanxung.cn

[E06] 替换子串
来源：http://dc.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://af.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://eo.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oa.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://vp.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qe.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kq.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://jm.newstarts.cn

[E07] 按分隔符拆分
来源：http://xv.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ii.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jt.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gu.szsharing.cn

TS:   s.split(",")
来源：http://it.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uj.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ah.521024.cn

Ruby: s.split(",");  s.split
来源：http://nw.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://il.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ib.shtwfgs.cn

Py:   ",".join(items)
来源：http://jw.hnjuh.cn

PHP:  implode(",", $items);
来源：http://sn.nicolike.cn

JS:   items.join(",")
来源：http://ww.panjiajie.cn

TS:   items.join(",")
来源：http://zw.wgjwhj.cn

Java: String.join(",", items)
来源：http://lp.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://el.huixiangedu.cn

Ruby: items.join(",")
来源：http://rb.lnxyls.cn

C#:   string.Join(",", items)
来源：http://gf.colortex.cn

[E09] 去除所有空白字符
来源：http://dn.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ug.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kk.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://gb.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://zf.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://yf.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hw.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hf.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://xy.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nk.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xy.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://km.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://rq.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://at.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eb.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zl.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jq.chemitech.net.cn

[E11] 反转字符串
来源：http://vs.asd995.cn

Py:   s[::-1]
来源：http://kv.szxytkj.cn

PHP:  strrev($s);
来源：http://de.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://hz.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://fy.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://no.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sr.muxihuayi.cn

Ruby: s.reverse
来源：http://yx.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://so.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://ab.haigaiapp.cn

Py:   s.count("a")
来源：http://ve.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://cy.newstarts.cn

JS:   s.split("a").length - 1
来源：http://ru.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://vi.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bi.521024.cn

Go:   strings.Count(s, "a")
来源：http://ht.nicolike.cn

Ruby: s.count("a")
来源：http://ex.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://ge.huanxung.cn

[E13] 逐字符遍历
来源：http://ko.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ex.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jg.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hs.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hg.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ov.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://np.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lx.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ht.9csxet.cn

[E14] URL 编码与 Base64
来源：http://ld.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ug.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ww.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ia.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mn.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nn.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gj.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ub.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://in.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://iy.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lx.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://af.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://om.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vu.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ty.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qy.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kz.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hu.jctech888.com.cn

[E16] 数字千分位
来源：http://dl.nicolike.cn

Py:   f"{1234567:,}"
来源：http://yz.gzmigu.cn

PHP:  number_format(1234567);
来源：http://qu.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ut.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ed.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://co.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mw.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://em.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://dp.wgjwhj.cn

[E17] 首字母大写
来源：http://ev.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wa.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yi.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hs.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ys.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://az.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gi.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://ng.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nn.hahajie.cn

[E18] 模板占位符替换
来源：http://ae.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://re.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yv.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qs.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gk.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ai.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fm.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rd.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cq.nszjky.cn

[E19] 多行文本按行拆分
来源：http://mi.colortex.cn

Py:   s.splitlines()
来源：http://sv.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wk.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://jn.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://cu.nicolike.cn

Java: s.lines().toList()
来源：http://uf.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://jr.chemitech.net.cn

Ruby: s.lines
来源：http://ko.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://qi.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://uc.colortex.cn

Py:   if not s:
来源：http://ri.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rs.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://au.yuexingan06.cn

TS:   if (s === "") {}
来源：http://mz.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://ic.gzmigu.cn

Go:   if s == "" {}
来源：http://nu.szsharing.cn

Ruby: if s.empty?
来源：http://qh.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cs.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://jo.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cy.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jw.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mc.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cc.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://my.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://re.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tq.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bg.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://qy.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sf.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://re.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yh.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qg.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bh.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qf.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://wh.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hd.newstarts.cn

================================================================================
来源：http://wh.wgjwhj.cn

F. 文件与目录
来源：http://cg.yuntaijiaju.cn

================================================================================
来源：http://sy.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://cq.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zs.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://zf.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ft.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hi.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yq.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pa.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://va.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://lu.9csxet.cn

[F02] 逐行读取文件
来源：http://oc.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mp.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fw.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cx.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://py.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qb.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lz.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nv.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://da.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://oy.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eg.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qr.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sl.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://st.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uh.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://bb.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xz.bjjhwx.cn

[F04] 追加写入文件
来源：http://bd.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ap.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kk.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ae.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ua.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xd.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tw.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://zu.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kp.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://cm.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ld.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://fq.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cs.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ws.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://ni.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://ww.shxzskj.cn

[F06] 删除文件
来源：http://ci.nszjky.cn

Py:   os.remove("a.txt")
来源：http://ra.nszjky.cn

PHP:  unlink("a.txt");
来源：http://zs.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ly.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fj.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fd.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://tu.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://jy.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://sb.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://dj.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nv.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lu.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jn.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yi.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lk.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mu.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gr.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wy.521024.cn

[F08] 遍历目录
来源：http://hw.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gh.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xl.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://ue.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://vb.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oi.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ni.szsharing.cn

Ruby: Dir.children("dir")
来源：http://pd.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://th.nszjky.cn

[F09] 获取文件大小
来源：http://wt.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://pa.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://xt.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://qg.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://dg.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mq.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pr.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://tp.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://jq.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://hn.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qo.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vp.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://du.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://vb.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://of.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kg.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rb.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://si.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://bh.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dy.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zj.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ny.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dn.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ao.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ab.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gu.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kz.gzmigu.cn

[F12] CSV 读写
来源：http://ay.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dd.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qw.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yt.panjiajie.cn

TS:   // 同上
来源：http://fk.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wa.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fw.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gu.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vj.jctech888.com.cn


<!-- 参考信息 -->