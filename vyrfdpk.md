代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://la.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ln.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ne.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ud.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zv.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://oc.szxytkj.cn

[E04] 查找子串位置
来源：http://ds.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ku.nicolike.cn

PHP:  strpos($s, "x");
来源：http://tq.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sg.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://jf.newstarts.cn

Java: s.indexOf("x")
来源：http://sp.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://iy.nszjky.cn

Ruby: s.index("x")
来源：http://ih.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ik.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vn.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wx.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uj.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pm.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xx.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ep.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nq.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sl.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fk.yuntaijiaju.cn

[E06] 替换子串
来源：http://dp.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lm.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://fi.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sz.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://fv.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ey.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rb.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://mk.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://ua.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cf.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nt.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rz.wgjwhj.cn

TS:   s.split(",")
来源：http://ri.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ia.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ce.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://lh.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ee.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://jn.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ca.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://na.yuntaijiaju.cn

JS:   items.join(",")
来源：http://yu.szsharing.cn

TS:   items.join(",")
来源：http://ly.haigaiapp.cn

Java: String.join(",", items)
来源：http://co.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ta.nszjky.cn

Ruby: items.join(",")
来源：http://da.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://ws.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://os.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oy.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yf.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://hl.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://au.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://zw.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sk.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qn.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://en.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://qj.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dn.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fl.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://xf.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://qd.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://di.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iq.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sn.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rm.haigaiapp.cn

[E11] 反转字符串
来源：http://rc.gzmigu.cn

Py:   s[::-1]
来源：http://kv.9csxet.cn

PHP:  strrev($s);
来源：http://fg.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://cq.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://re.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nv.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sm.asd995.cn

Ruby: s.reverse
来源：http://fn.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gb.huanxung.cn

[E12] 统计某字符出现次数
来源：http://dm.muxihuayi.cn

Py:   s.count("a")
来源：http://fx.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://ab.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://nv.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://mf.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cw.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://zg.lnxyls.cn

Ruby: s.count("a")
来源：http://pf.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://kd.newstarts.cn

[E13] 逐字符遍历
来源：http://md.colortex.cn

Py:   for ch in s: print(ch)
来源：http://re.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dj.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jb.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tz.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zp.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ul.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kf.9csxet.cn

[E14] URL 编码与 Base64
来源：http://od.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gq.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ej.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ds.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wi.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ks.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pf.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oq.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dp.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://zp.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oo.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sl.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bu.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ht.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ro.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kh.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fo.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://or.huixiangedu.cn

[E16] 数字千分位
来源：http://sa.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ev.szxytkj.cn

PHP:  number_format(1234567);
来源：http://qc.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qq.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ps.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kv.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ej.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hv.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://na.bjjhwx.cn

[E17] 首字母大写
来源：http://we.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tu.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qr.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ex.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vu.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sv.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sa.jctech888.com.cn

Ruby: s.capitalize
来源：http://yl.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jm.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://zj.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cu.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tq.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wp.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://am.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fi.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pd.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gm.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fa.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://vv.hahajie.cn

Py:   s.splitlines()
来源：http://yy.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ri.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://gk.521024.cn

TS:   s.split(/\r?\n/)
来源：http://he.szxytkj.cn

Java: s.lines().toList()
来源：http://aj.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ed.jianghongdianzi.cn

Ruby: s.lines
来源：http://rz.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ba.9csxet.cn

[E20] 判断字符串是否为空
来源：http://bx.nszjky.cn

Py:   if not s:
来源：http://gn.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nf.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dv.shxzukj.cn

TS:   if (s === "") {}
来源：http://kp.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://mp.huixiangedu.cn

Go:   if s == "" {}
来源：http://ml.hnjuh.cn

Ruby: if s.empty?
来源：http://en.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sa.hnjuh.cn

[E21] 超长截断加省略号
来源：http://aj.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://et.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cn.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aw.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://so.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qo.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://qe.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xy.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gp.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ml.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bh.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sb.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qx.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://br.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ky.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xt.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://vc.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mt.szxytkj.cn

================================================================================
来源：http://mv.wgjwhj.cn

F. 文件与目录
来源：http://ht.jianghongdianzi.cn

================================================================================
来源：http://sv.muxihuayi.cn

[F01] 读取整个文件
来源：http://zf.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fl.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://up.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hm.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://io.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xo.newstarts.cn

Ruby: File.read("a.txt")
来源：http://gi.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://xo.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://vp.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://st.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://on.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lq.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gc.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xn.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ol.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bn.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yp.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://qm.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ju.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://al.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ue.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iu.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ji.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ys.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://vy.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ny.huixiangedu.cn

[F04] 追加写入文件
来源：http://lw.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yb.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zk.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wq.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sp.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cq.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rc.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sp.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ui.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://yy.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hl.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://vi.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://ao.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://wi.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dw.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tp.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://be.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://hb.hnjuh.cn

[F06] 删除文件
来源：http://bi.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://vt.asd995.cn

PHP:  unlink("a.txt");
来源：http://gw.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://th.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qs.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rh.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://gh.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://il.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://vi.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://tk.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kr.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://st.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xn.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ov.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oc.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kw.bookmarksfly.cn

[F08] 遍历目录
来源：http://tr.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tm.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wp.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://dt.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://ax.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tb.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fj.colortex.cn

Ruby: Dir.children("dir")
来源：http://ho.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://va.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://nz.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://ve.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://xx.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://lh.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://lv.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wb.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://be.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://oj.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://ng.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jb.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ql.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://px.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://ar.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lu.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cf.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zc.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sr.wgjwhj.cn

[F11] 复制与移动文件
来源：http://jg.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cf.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://va.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ji.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bv.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jz.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ax.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://id.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vi.panjiajie.cn

[F12] CSV 读写
来源：http://rl.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zm.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://re.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uo.jianghongdianzi.cn

TS:   // 同上
来源：http://bz.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ny.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nm.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xe.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rw.panjiajie.cn

================================================================================
来源：http://xa.shxzukj.cn

G. 面向对象
来源：http://pu.yuntaijiaju.cn

================================================================================
来源：http://vs.shtwfgs.cn

[G01] 定义类
来源：http://ws.lnxyls.cn

Py:   class User: pass
来源：http://af.lnxyls.cn

PHP:  class User {}
来源：http://ny.colortex.cn

JS:   class User {}
来源：http://tr.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://as.szsharing.cn

Java: class User {}
来源：http://tr.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://nx.nszjky.cn

Ruby: class User; end
来源：http://as.shxzukj.cn

C#:   class User {}
来源：http://jb.chemitech.net.cn


<!-- 参考信息 -->