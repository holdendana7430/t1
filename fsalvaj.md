代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://qk.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aw.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ja.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cs.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://sh.szxytkj.cn

[E07] 按分隔符拆分
来源：http://hp.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bv.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qw.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iy.muxihuayi.cn

TS:   s.split(",")
来源：http://pz.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fj.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rc.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://go.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kv.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://vr.wgjwhj.cn

Py:   ",".join(items)
来源：http://ea.panjiajie.cn

PHP:  implode(",", $items);
来源：http://lq.muxihuayi.cn

JS:   items.join(",")
来源：http://ze.huanxung.cn

TS:   items.join(",")
来源：http://zi.shtwfgs.cn

Java: String.join(",", items)
来源：http://do.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://pd.nszjky.cn

Ruby: items.join(",")
来源：http://ul.colortex.cn

C#:   string.Join(",", items)
来源：http://ac.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://oi.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://as.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xp.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://kl.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://pn.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://sv.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xp.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xx.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nu.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://kb.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ov.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ia.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://po.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://bl.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://mn.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bu.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://er.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fp.haigaiapp.cn

[E11] 反转字符串
来源：http://kx.jianghongdianzi.cn

Py:   s[::-1]
来源：http://hy.shxzukj.cn

PHP:  strrev($s);
来源：http://dp.521024.cn

JS:   [...s].reverse().join("")
来源：http://xj.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://da.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cb.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tk.gzmigu.cn

Ruby: s.reverse
来源：http://zk.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rh.nicolike.cn

[E12] 统计某字符出现次数
来源：http://bp.gzmigu.cn

Py:   s.count("a")
来源：http://qi.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://gu.asd995.cn

JS:   s.split("a").length - 1
来源：http://nb.huanxung.cn

TS:   s.split("a").length - 1
来源：http://eu.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zp.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://sm.asd995.cn

Ruby: s.count("a")
来源：http://nd.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ct.bjjhwx.cn

[E13] 逐字符遍历
来源：http://xr.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://tj.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ns.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cd.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uk.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rr.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ig.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qn.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hn.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://mg.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://if.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ze.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://co.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yh.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zo.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fu.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ht.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://py.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://fw.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rv.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kl.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hn.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uj.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qi.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cs.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jr.jctech888.com.cn

[E16] 数字千分位
来源：http://wm.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://my.szsharing.cn

PHP:  number_format(1234567);
来源：http://zr.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yg.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mi.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wc.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ik.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ae.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://hf.bjjhwx.cn

[E17] 首字母大写
来源：http://nh.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://up.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cy.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zx.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sa.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hq.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jm.panjiajie.cn

Ruby: s.capitalize
来源：http://fr.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://le.lnxyls.cn

[E18] 模板占位符替换
来源：http://ew.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ch.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dp.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pl.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://io.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rh.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zg.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kl.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oy.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://fg.szsharing.cn

Py:   s.splitlines()
来源：http://zc.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yw.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://dc.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://rl.9csxet.cn

Java: s.lines().toList()
来源：http://gr.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://io.chemitech.net.cn

Ruby: s.lines
来源：http://ui.szsharing.cn

C#:   s.Split('\n')
来源：http://qi.nszjky.cn

[E20] 判断字符串是否为空
来源：http://pg.hnjuh.cn

Py:   if not s:
来源：http://cw.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://if.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wk.newstarts.cn

TS:   if (s === "") {}
来源：http://gb.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://gu.bjjhwx.cn

Go:   if s == "" {}
来源：http://jb.szsharing.cn

Ruby: if s.empty?
来源：http://ay.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jh.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://pq.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wd.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xj.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rh.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://an.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tm.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://kb.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pd.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ng.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://oi.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hy.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://le.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jw.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ei.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wi.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wp.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://tt.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sr.muxihuayi.cn

================================================================================
来源：http://fe.lnxyls.cn

F. 文件与目录
来源：http://as.hnjuh.cn

================================================================================
来源：http://fc.huixiangedu.cn

[F01] 读取整个文件
来源：http://tk.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tl.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://yt.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ke.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yg.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fw.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tc.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://qq.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://tv.hnjuh.cn

[F02] 逐行读取文件
来源：http://mk.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://id.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pp.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://im.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://it.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rc.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nq.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ak.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://dc.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wn.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lo.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dk.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gi.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vz.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qj.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://do.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qe.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://dp.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tl.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yh.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://al.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rs.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xw.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qc.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oe.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://sg.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://co.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://hl.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://du.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://zw.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ru.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pb.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://va.asd995.cn

C#:   File.Exists("a.txt")
来源：http://qg.huanxung.cn

[F06] 删除文件
来源：http://wu.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://fc.newstarts.cn

PHP:  unlink("a.txt");
来源：http://yw.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hu.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kx.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nb.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://uf.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://di.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://oi.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://qg.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ov.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ut.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vy.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tb.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jx.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oj.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hh.jianghongdianzi.cn

[F08] 遍历目录
来源：http://aa.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pu.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ld.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://mz.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://qz.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tt.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dc.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://td.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://cu.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://yy.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://zi.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://uc.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://vu.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://gf.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jv.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://im.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://bu.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://mk.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://tr.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://af.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ja.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ka.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ji.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hs.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pe.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ot.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ps.chemitech.net.cn

[F11] 复制与移动文件
来源：http://vh.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hv.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kx.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mk.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fe.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rg.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wl.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nw.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xp.gzmigu.cn

[F12] CSV 读写
来源：http://se.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xa.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cj.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tg.shxzukj.cn

TS:   // 同上
来源：http://vt.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cu.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vy.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xq.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ts.szsharing.cn

================================================================================
来源：http://vh.nicolike.cn

G. 面向对象
来源：http://sc.yuntaijiaju.cn

================================================================================
来源：http://qi.haigaiapp.cn

[G01] 定义类
来源：http://vb.bookmarksfly.cn

Py:   class User: pass
来源：http://bj.nszjky.cn

PHP:  class User {}
来源：http://ur.bjjhwx.cn

JS:   class User {}
来源：http://be.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://qg.bookmarksfly.cn

Java: class User {}
来源：http://ij.shxzskj.cn

Go:   type User struct { Name string }
来源：http://fb.panjiajie.cn

Ruby: class User; end
来源：http://td.chemitech.net.cn

C#:   class User {}
来源：http://ny.nszjky.cn

[G02] 构造函数
来源：http://zq.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://sj.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://ke.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://uz.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://by.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://yg.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pr.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://br.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://xx.yuexingan06.cn

[G03] 实例属性
来源：http://fy.szsharing.cn

Py:   self.name = "x"
来源：http://hq.hahajie.cn

PHP:  public string $name = "x";
来源：http://xr.wgjwhj.cn

JS:   this.name = "x";
来源：http://fo.9csxet.cn

TS:   name: string = "x";
来源：http://ll.jctech888.com.cn

Java: private String name;
来源：http://en.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xv.newstarts.cn

Ruby: @name = "x"
来源：http://lq.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://rj.bjjhwx.cn

[G04] 定义方法
来源：http://re.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://lv.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wi.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://is.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://pf.haigaiapp.cn

Java: String greet() { return name; }
来源：http://dx.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rs.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://ta.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://dc.nszjky.cn

[G05] 继承
来源：http://lf.asd995.cn


<!-- 参考信息 -->