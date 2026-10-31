代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://nw.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://pp.bjjhwx.cn

[E04] 查找子串位置
来源：http://md.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://ru.nicolike.cn

PHP:  strpos($s, "x");
来源：http://ix.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ce.huanxung.cn

TS:   s.indexOf("x")
来源：http://np.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://pz.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://th.shxzukj.cn

Ruby: s.index("x")
来源：http://vm.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://un.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vr.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xc.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ie.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pr.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ee.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lc.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qs.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://en.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wa.jianghongdianzi.cn

[E06] 替换子串
来源：http://ek.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kk.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://dq.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hm.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://xh.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://op.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pw.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oe.colortex.cn

C#:   s.Replace("a", "b")
来源：http://wd.hnjuh.cn

[E07] 按分隔符拆分
来源：http://bx.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xm.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ip.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://er.yuexingan06.cn

TS:   s.split(",")
来源：http://sf.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oz.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pa.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://xs.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rz.huanxung.cn

[E08] 数组按分隔符合并
来源：http://sp.shxzukj.cn

Py:   ",".join(items)
来源：http://pt.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://de.jctech888.com.cn

JS:   items.join(",")
来源：http://kc.521024.cn

TS:   items.join(",")
来源：http://uc.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://nw.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://av.huixiangedu.cn

Ruby: items.join(",")
来源：http://xh.colortex.cn

C#:   string.Join(",", items)
来源：http://zq.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://dw.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fx.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pl.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://yj.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://iq.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://cw.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uj.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zn.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lq.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://gv.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ox.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ef.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://xq.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ro.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://wv.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qd.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wc.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cj.shxzskj.cn

[E11] 反转字符串
来源：http://dl.shtwfgs.cn

Py:   s[::-1]
来源：http://cq.szxytkj.cn

PHP:  strrev($s);
来源：http://sp.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ws.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://fm.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hl.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gu.szsharing.cn

Ruby: s.reverse
来源：http://rv.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eb.hahajie.cn

[E12] 统计某字符出现次数
来源：http://un.9csxet.cn

Py:   s.count("a")
来源：http://ld.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://nr.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://vg.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://ix.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bk.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://ie.colortex.cn

Ruby: s.count("a")
来源：http://rh.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://ql.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://pe.colortex.cn

Py:   for ch in s: print(ch)
来源：http://lu.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vh.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bs.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kq.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ju.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://no.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vd.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ge.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://kk.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pc.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ec.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wk.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ng.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zm.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ct.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gn.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sx.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://pz.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ys.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://og.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ij.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://di.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uh.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jk.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pu.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mf.jctech888.com.cn

[E16] 数字千分位
来源：http://ht.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://pv.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://rl.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ls.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ps.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jo.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lc.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bc.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://rv.yuexingan06.cn

[E17] 首字母大写
来源：http://pe.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qh.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wp.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qu.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ys.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zj.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bc.newstarts.cn

Ruby: s.capitalize
来源：http://na.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ae.wgjwhj.cn

[E18] 模板占位符替换
来源：http://ca.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wk.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ez.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ev.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cd.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xe.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ro.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iy.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zq.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://oo.wgjwhj.cn

Py:   s.splitlines()
来源：http://rv.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fk.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ks.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ll.hnjuh.cn

Java: s.lines().toList()
来源：http://qx.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://fz.colortex.cn

Ruby: s.lines
来源：http://uy.jctech888.com.cn

C#:   s.Split('\n')
来源：http://hr.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://fb.shxzukj.cn

Py:   if not s:
来源：http://lx.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nv.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wk.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://mk.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://bz.hahajie.cn

Go:   if s == "" {}
来源：http://qs.chemitech.net.cn

Ruby: if s.empty?
来源：http://ld.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bp.shxzskj.cn

[E21] 超长截断加省略号
来源：http://dq.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yx.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vz.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ar.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vp.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://ai.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bv.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hy.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://qs.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pl.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ju.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tl.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vk.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dw.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ku.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://gm.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ez.hahajie.cn

================================================================================
来源：http://uc.bjjhwx.cn

F. 文件与目录
来源：http://ma.szsharing.cn

================================================================================
来源：http://ms.asd995.cn

[F01] 读取整个文件
来源：http://xn.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ba.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://ik.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ly.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ts.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pi.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bh.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://fj.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://tv.bjjhwx.cn

[F02] 逐行读取文件
来源：http://vt.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sz.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nn.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sv.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ic.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dr.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ux.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qt.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ie.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://sr.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qe.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ly.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ew.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zp.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jn.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://db.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://rl.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hu.szsharing.cn

[F04] 追加写入文件
来源：http://ru.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://db.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wq.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ci.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gb.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xa.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ez.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ir.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zq.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://it.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://od.asd995.cn

PHP:  file_exists("a.txt");
来源：http://pu.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://kj.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://xy.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ja.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yt.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://ed.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://ni.szsharing.cn

[F06] 删除文件
来源：http://bm.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ow.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://nz.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sn.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sh.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zr.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://ft.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://mi.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ex.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://vz.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gn.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cn.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ws.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bn.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kc.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dw.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bv.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oh.yuntaijiaju.cn

[F08] 遍历目录
来源：http://py.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vu.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://es.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://ci.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ns.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sw.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sw.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://je.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://lt.521024.cn

[F09] 获取文件大小
来源：http://vx.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://lb.huanxung.cn

PHP:  filesize("a.txt");
来源：http://et.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://zs.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ip.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ca.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://os.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://py.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ml.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://zz.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://om.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qe.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lu.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://lp.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lt.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://am.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fm.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tg.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ol.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ol.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rh.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jb.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qv.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://by.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wc.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wr.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pg.panjiajie.cn

[F12] CSV 读写
来源：http://fc.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zq.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bi.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iw.bookmarksfly.cn

TS:   // 同上
来源：http://gd.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iq.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rz.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aj.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tu.hahajie.cn

================================================================================
来源：http://yw.colortex.cn

G. 面向对象
来源：http://mj.nicolike.cn

================================================================================
来源：http://is.jctech888.com.cn

[G01] 定义类
来源：http://sv.shtwfgs.cn

Py:   class User: pass
来源：http://bl.yuntaijiaju.cn

PHP:  class User {}
来源：http://fh.lnxyls.cn

JS:   class User {}
来源：http://pd.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://oi.asd995.cn

Java: class User {}
来源：http://fn.shxzskj.cn

Go:   type User struct { Name string }
来源：http://sb.shxzskj.cn

Ruby: class User; end
来源：http://ue.lnxyls.cn

C#:   class User {}
来源：http://ix.asd995.cn

[G02] 构造函数
来源：http://ee.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://hk.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://yp.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qe.nszjky.cn


<!-- 参考信息 -->