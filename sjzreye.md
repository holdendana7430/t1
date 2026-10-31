代发 wailian999

[E06] 替换子串
来源：http://yz.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gu.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://yb.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mq.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://go.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yn.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ms.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mb.colortex.cn

C#:   s.Replace("a", "b")
来源：http://sa.colortex.cn

[E07] 按分隔符拆分
来源：http://kw.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fd.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kp.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pe.muxihuayi.cn

TS:   s.split(",")
来源：http://kf.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hh.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://do.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://jx.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ws.huanxung.cn

[E08] 数组按分隔符合并
来源：http://sc.huanxung.cn

Py:   ",".join(items)
来源：http://hk.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://if.muxihuayi.cn

JS:   items.join(",")
来源：http://pu.gzmigu.cn

TS:   items.join(",")
来源：http://av.shxzskj.cn

Java: String.join(",", items)
来源：http://fi.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://xv.huixiangedu.cn

Ruby: items.join(",")
来源：http://ls.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://dm.colortex.cn

[E09] 去除所有空白字符
来源：http://hg.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://no.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sh.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://lf.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://uw.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://ge.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yz.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://su.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wa.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://nb.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mq.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dl.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://ua.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://iy.huanxung.cn

Java: String.format("%03d", 7)
来源：http://ej.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oi.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mv.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bz.panjiajie.cn

[E11] 反转字符串
来源：http://gu.jctech888.com.cn

Py:   s[::-1]
来源：http://lo.hahajie.cn

PHP:  strrev($s);
来源：http://oj.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://dl.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://iy.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xs.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xy.muxihuayi.cn

Ruby: s.reverse
来源：http://iq.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ey.huanxung.cn

[E12] 统计某字符出现次数
来源：http://ol.asd995.cn

Py:   s.count("a")
来源：http://sh.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://yn.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://lb.nszjky.cn

TS:   s.split("a").length - 1
来源：http://lw.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sv.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://pz.9csxet.cn

Ruby: s.count("a")
来源：http://wv.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://bq.colortex.cn

[E13] 逐字符遍历
来源：http://oj.521024.cn

Py:   for ch in s: print(ch)
来源：http://wy.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kh.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rz.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qj.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mx.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qp.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yt.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jg.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://dh.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cf.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nt.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ed.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sp.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nw.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hu.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ap.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ik.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://sc.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ni.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tu.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ry.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bf.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ur.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://id.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rz.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oj.panjiajie.cn

[E16] 数字千分位
来源：http://ko.521024.cn

Py:   f"{1234567:,}"
来源：http://ti.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://ym.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wg.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xd.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ti.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ap.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mx.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://sn.huanxung.cn

[E17] 首字母大写
来源：http://bs.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tj.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yh.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ys.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hr.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ez.wgjwhj.cn

Ruby: s.capitalize
来源：http://we.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cb.yuexingan06.cn

[E18] 模板占位符替换
来源：http://iq.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yc.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yx.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xj.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kh.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://he.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kh.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bc.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kv.hahajie.cn

[E19] 多行文本按行拆分
来源：http://ql.lnxyls.cn

Py:   s.splitlines()
来源：http://ls.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sc.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://bs.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://xm.nszjky.cn

Java: s.lines().toList()
来源：http://gy.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://jy.panjiajie.cn

Ruby: s.lines
来源：http://qv.shxzukj.cn

C#:   s.Split('\n')
来源：http://pk.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://sq.hnjuh.cn

Py:   if not s:
来源：http://vf.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aa.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ur.hnjuh.cn

TS:   if (s === "") {}
来源：http://hf.521024.cn

Java: if (s.isEmpty()) {}
来源：http://ti.lnxyls.cn

Go:   if s == "" {}
来源：http://sk.bookmarksfly.cn

Ruby: if s.empty?
来源：http://to.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rb.hnjuh.cn

[E21] 超长截断加省略号
来源：http://cd.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kq.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nk.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uq.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gr.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://zz.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ew.nszjky.cn

[E22] 字节长度与字符长度
来源：http://mu.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qk.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ij.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pl.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zp.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tb.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ze.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://cl.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kx.haigaiapp.cn

================================================================================
来源：http://hi.shxzukj.cn

F. 文件与目录
来源：http://pa.huixinmuqiang.cn

================================================================================
来源：http://tp.nicolike.cn

[F01] 读取整个文件
来源：http://vj.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uc.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://ph.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xq.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dp.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://og.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uo.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://ia.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ao.colortex.cn

[F02] 逐行读取文件
来源：http://hb.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://by.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fn.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eq.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://el.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tz.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lv.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lh.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nf.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://sw.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qu.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ju.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bm.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uq.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nr.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://je.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://pj.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tn.szxytkj.cn

[F04] 追加写入文件
来源：http://vw.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xu.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zj.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sg.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://os.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rt.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ej.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zd.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://kc.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mr.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://cv.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ya.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://kj.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xr.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jx.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://uf.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://yb.huanxung.cn

[F06] 删除文件
来源：http://uq.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://gh.nicolike.cn

PHP:  unlink("a.txt");
来源：http://gj.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pu.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wx.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qd.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://ns.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://em.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://jc.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://hx.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mc.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ty.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cb.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ji.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zm.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ig.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gv.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ei.lnxyls.cn

[F08] 遍历目录
来源：http://ap.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qn.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://td.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://nk.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://zv.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wo.colortex.cn

Ruby: Dir.children("dir")
来源：http://ir.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://nu.muxihuayi.cn

[F09] 获取文件大小
来源：http://zp.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://pz.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://qe.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://jk.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://pb.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tw.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bz.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://qd.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://zc.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://po.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://db.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vy.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cy.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://is.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wc.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mb.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yx.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xp.colortex.cn

[F11] 复制与移动文件
来源：http://sp.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fx.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ls.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ti.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://et.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zo.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cn.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ei.huanxung.cn

[F12] CSV 读写
来源：http://nx.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tq.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xb.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://en.521024.cn

TS:   // 同上
来源：http://rk.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eg.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wm.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mm.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tk.newstarts.cn

================================================================================
来源：http://cu.nicolike.cn

G. 面向对象
来源：http://qp.jianghongdianzi.cn

================================================================================
来源：http://jq.jianghongdianzi.cn

[G01] 定义类
来源：http://or.wgjwhj.cn

Py:   class User: pass
来源：http://lq.chemitech.net.cn

PHP:  class User {}
来源：http://gp.jianghongdianzi.cn

JS:   class User {}
来源：http://xz.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://sc.yuexingan06.cn

Java: class User {}
来源：http://mz.nszjky.cn

Go:   type User struct { Name string }
来源：http://ly.szxytkj.cn

Ruby: class User; end
来源：http://bu.haigaiapp.cn

C#:   class User {}
来源：http://lp.shtwfgs.cn

[G02] 构造函数
来源：http://yo.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://pb.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://im.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://zj.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://bb.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://ix.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://if.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://gs.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://mt.chemitech.net.cn

[G03] 实例属性
来源：http://vg.haigaiapp.cn

Py:   self.name = "x"
来源：http://lk.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://hh.huanxung.cn

JS:   this.name = "x";
来源：http://wx.bookmarksfly.cn

TS:   name: string = "x";
来源：http://gg.szxytkj.cn

Java: private String name;
来源：http://lm.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ie.shxzukj.cn

Ruby: @name = "x"
来源：http://ye.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://xh.haigaiapp.cn

[G04] 定义方法
来源：http://ow.nicolike.cn

Py:   def greet(self): return self.name
来源：http://fk.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fh.nszjky.cn

JS:   greet() { return this.name; }
来源：http://nn.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://bi.gzmigu.cn

Java: String greet() { return name; }
来源：http://bl.bookmarksfly.cn


<!-- 参考信息 -->