代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://om.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vp.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qg.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://to.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ak.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://re.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xt.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wr.colortex.cn

[E06] 替换子串
来源：http://fn.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://co.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://sw.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gx.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://nv.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qt.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qs.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zz.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://vh.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://aw.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fu.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oy.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rg.newstarts.cn

TS:   s.split(",")
来源：http://si.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tq.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wj.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://ki.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gq.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://vr.haigaiapp.cn

Py:   ",".join(items)
来源：http://gp.shxzskj.cn

PHP:  implode(",", $items);
来源：http://px.shxzskj.cn

JS:   items.join(",")
来源：http://ku.521024.cn

TS:   items.join(",")
来源：http://ux.wgjwhj.cn

Java: String.join(",", items)
来源：http://cn.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://gc.muxihuayi.cn

Ruby: items.join(",")
来源：http://ja.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://gn.lnxyls.cn

[E09] 去除所有空白字符
来源：http://jc.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jr.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vh.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://hd.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://jy.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://dc.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xv.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xp.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://fh.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bd.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fz.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://nr.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://sc.521024.cn

Java: String.format("%03d", 7)
来源：http://lw.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pf.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ee.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gp.nicolike.cn

[E11] 反转字符串
来源：http://lj.szsharing.cn

Py:   s[::-1]
来源：http://ny.colortex.cn

PHP:  strrev($s);
来源：http://iv.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://mi.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://mv.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bw.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ao.9csxet.cn

Ruby: s.reverse
来源：http://kx.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nx.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ut.huixinmuqiang.cn

Py:   s.count("a")
来源：http://hj.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://an.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://mt.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://yr.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cq.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://rp.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://pw.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://fl.nicolike.cn

[E13] 逐字符遍历
来源：http://pi.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://on.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wf.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uu.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gm.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eu.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uu.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yf.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gc.asd995.cn

[E14] URL 编码与 Base64
来源：http://jw.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jg.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cp.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ha.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://er.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://or.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vi.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ba.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pk.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://td.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://so.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wh.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ql.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dh.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tu.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ye.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nw.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xc.shxzukj.cn

[E16] 数字千分位
来源：http://fq.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://wc.huanxung.cn

PHP:  number_format(1234567);
来源：http://uv.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jg.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://on.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rf.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ek.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://cd.muxihuayi.cn

[E17] 首字母大写
来源：http://om.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vj.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://km.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://to.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qr.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sl.szxytkj.cn

Ruby: s.capitalize
来源：http://wi.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hu.jctech888.com.cn

[E18] 模板占位符替换
来源：http://cv.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eq.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xa.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zj.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fi.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eb.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dq.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iz.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ek.szsharing.cn

[E19] 多行文本按行拆分
来源：http://gg.shtwfgs.cn

Py:   s.splitlines()
来源：http://gf.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://le.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://fn.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://dj.521024.cn

Java: s.lines().toList()
来源：http://cd.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://re.shtwfgs.cn

Ruby: s.lines
来源：http://bb.shxzukj.cn

C#:   s.Split('\n')
来源：http://xo.colortex.cn

[E20] 判断字符串是否为空
来源：http://ho.wgjwhj.cn

Py:   if not s:
来源：http://vt.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qq.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xi.muxihuayi.cn

TS:   if (s === "") {}
来源：http://vi.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://qw.hahajie.cn

Go:   if s == "" {}
来源：http://ov.huixiangedu.cn

Ruby: if s.empty?
来源：http://gt.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hw.shxzukj.cn

[E21] 超长截断加省略号
来源：http://na.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mw.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dv.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nz.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tb.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vp.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://wg.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sa.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://em.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://th.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zs.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ap.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pz.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vd.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dd.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fi.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://ap.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://os.newstarts.cn

================================================================================
来源：http://ov.huixiangedu.cn

F. 文件与目录
来源：http://iy.yuexingan06.cn

================================================================================
来源：http://dw.nszjky.cn

[F01] 读取整个文件
来源：http://bg.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uj.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://ys.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://om.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aa.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bp.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zz.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ub.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://lt.521024.cn

[F02] 逐行读取文件
来源：http://ge.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ly.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jn.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vl.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vv.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wa.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vg.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tz.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oo.asd995.cn

[F03] 写入文件（覆盖）
来源：http://jr.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ts.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gw.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rm.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wd.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hv.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rm.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://bp.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jc.huanxung.cn

[F04] 追加写入文件
来源：http://kz.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nr.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fz.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fi.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vp.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pm.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zi.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hi.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qm.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://lw.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kp.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://qu.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://at.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://sj.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kv.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yb.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://vu.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://ro.shxzskj.cn

[F06] 删除文件
来源：http://gw.nszjky.cn

Py:   os.remove("a.txt")
来源：http://wd.colortex.cn

PHP:  unlink("a.txt");
来源：http://yn.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://et.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nu.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mn.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://jx.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://us.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://pi.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://py.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gt.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bw.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vo.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rn.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ng.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gl.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nf.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bs.yuexingan06.cn

[F08] 遍历目录
来源：http://tn.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mx.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fk.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://ms.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://zm.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ft.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://na.colortex.cn

Ruby: Dir.children("dir")
来源：http://ap.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://kj.szsharing.cn

[F09] 获取文件大小
来源：http://oo.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://qy.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://vz.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://cf.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://um.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rv.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://uj.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://fd.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://di.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bc.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mq.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wb.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ls.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fu.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://to.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nx.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sl.chemitech.net.cn

[F11] 复制与移动文件
来源：http://uz.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rz.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rd.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jh.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ko.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ks.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cw.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vf.shxzukj.cn

[F12] CSV 读写
来源：http://fy.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://en.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://la.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vx.hnjuh.cn

TS:   // 同上
来源：http://fy.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yz.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zl.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://or.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ib.asd995.cn

================================================================================
来源：http://sj.hahajie.cn

G. 面向对象
来源：http://my.huanxung.cn

================================================================================
来源：http://pm.lnxyls.cn

[G01] 定义类
来源：http://hu.newstarts.cn

Py:   class User: pass
来源：http://jp.shxzskj.cn

PHP:  class User {}
来源：http://zq.shxzskj.cn

JS:   class User {}
来源：http://uc.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://gr.bjjhwx.cn

Java: class User {}
来源：http://pc.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://ti.521024.cn

Ruby: class User; end
来源：http://fk.asd995.cn

C#:   class User {}
来源：http://vm.shtwfgs.cn

[G02] 构造函数
来源：http://yl.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://gn.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://np.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jo.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://eo.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://ek.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://al.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://vt.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://hv.bjjhwx.cn

[G03] 实例属性
来源：http://zs.newstarts.cn

Py:   self.name = "x"
来源：http://pb.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://yd.chemitech.net.cn

JS:   this.name = "x";
来源：http://ml.huanxung.cn

TS:   name: string = "x";
来源：http://nz.huixinmuqiang.cn

Java: private String name;
来源：http://nu.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aa.colortex.cn


<!-- 参考信息 -->