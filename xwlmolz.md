代发 wailian999

C#:   s.Replace("a", "b")
来源：http://or.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://va.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kl.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zl.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bj.hahajie.cn

TS:   s.split(",")
来源：http://tu.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oz.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uq.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://li.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wf.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://bb.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://vr.szsharing.cn

PHP:  implode(",", $items);
来源：http://zs.szxytkj.cn

JS:   items.join(",")
来源：http://fi.9csxet.cn

TS:   items.join(",")
来源：http://tf.yuexingan06.cn

Java: String.join(",", items)
来源：http://vd.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://kh.newstarts.cn

Ruby: items.join(",")
来源：http://yx.hnjuh.cn

C#:   string.Join(",", items)
来源：http://op.hahajie.cn

[E09] 去除所有空白字符
来源：http://ur.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jd.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ub.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kq.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://gl.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://vk.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ed.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kk.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jp.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://ue.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yy.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://od.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://qe.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ct.9csxet.cn

Java: String.format("%03d", 7)
来源：http://tr.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tw.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kw.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjjhwx.cn

[E11] 反转字符串
来源：http://qu.shxzskj.cn

Py:   s[::-1]
来源：http://bp.gzmigu.cn

PHP:  strrev($s);
来源：http://bk.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://mp.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://bh.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://su.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cc.panjiajie.cn

Ruby: s.reverse
来源：http://qx.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jq.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://oe.jctech888.com.cn

Py:   s.count("a")
来源：http://hf.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://kv.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://vf.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://qr.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vd.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://el.9csxet.cn

Ruby: s.count("a")
来源：http://bw.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://jv.521024.cn

[E13] 逐字符遍历
来源：http://xo.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://ih.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wa.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qj.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xm.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wt.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mp.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nx.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tq.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://ms.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://un.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ri.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sc.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xj.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zm.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fr.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://re.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yv.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://pa.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gq.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yd.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dw.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://di.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ix.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fx.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vn.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bw.yuexingan06.cn

[E16] 数字千分位
来源：http://dw.szsharing.cn

Py:   f"{1234567:,}"
来源：http://gv.lnxyls.cn

PHP:  number_format(1234567);
来源：http://qj.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nm.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://el.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qe.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ss.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ic.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://pl.muxihuayi.cn

[E17] 首字母大写
来源：http://wv.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ik.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bm.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://on.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qi.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hg.nszjky.cn

Ruby: s.capitalize
来源：http://ir.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vc.haigaiapp.cn

[E18] 模板占位符替换
来源：http://mk.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rh.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zl.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yb.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sx.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://po.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uq.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pm.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://de.9csxet.cn

[E19] 多行文本按行拆分
来源：http://nz.muxihuayi.cn

Py:   s.splitlines()
来源：http://gq.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yf.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://dg.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://pk.szsharing.cn

Java: s.lines().toList()
来源：http://lv.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://xq.huixiangedu.cn

Ruby: s.lines
来源：http://dt.colortex.cn

C#:   s.Split('\n')
来源：http://zt.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://vl.gzmigu.cn

Py:   if not s:
来源：http://vk.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ik.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hn.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ew.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ix.nszjky.cn

Go:   if s == "" {}
来源：http://pu.shxzukj.cn

Ruby: if s.empty?
来源：http://dg.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dg.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://dz.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lg.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://za.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xd.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uy.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ui.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://kw.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yd.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wf.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://xc.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hf.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gp.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ep.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://se.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hh.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://ei.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ge.yuexingan06.cn

================================================================================
来源：http://we.gzmigu.cn

F. 文件与目录
来源：http://ms.nszjky.cn

================================================================================
来源：http://nz.hnjuh.cn

[F01] 读取整个文件
来源：http://zg.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kq.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://ws.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sr.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yc.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://at.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nz.9csxet.cn

Ruby: File.read("a.txt")
来源：http://hy.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://lm.521024.cn

[F02] 逐行读取文件
来源：http://qx.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vb.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://md.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jo.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kx.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ey.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fl.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://om.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rl.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://cy.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ch.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kn.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ar.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fz.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ws.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sy.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://md.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aq.shxzskj.cn

[F04] 追加写入文件
来源：http://nz.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fb.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hq.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dt.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tt.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ft.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yh.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://km.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://pu.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rq.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://za.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://pm.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://dp.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ik.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ng.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://ru.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://jc.huixinmuqiang.cn

[F06] 删除文件
来源：http://wz.9csxet.cn

Py:   os.remove("a.txt")
来源：http://us.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://le.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yn.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oa.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://re.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://pu.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://hx.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://ev.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://si.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ia.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zh.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pi.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://or.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ie.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wy.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tr.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ze.muxihuayi.cn

[F08] 遍历目录
来源：http://gm.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gt.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uu.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://lt.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://vo.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dv.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pr.nszjky.cn

Ruby: Dir.children("dir")
来源：http://xu.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://ck.wgjwhj.cn

[F09] 获取文件大小
来源：http://aa.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://pz.huanxung.cn

PHP:  filesize("a.txt");
来源：http://za.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://iq.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://fx.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vi.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yu.newstarts.cn

Ruby: File.size("a.txt")
来源：http://zo.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://zi.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://nq.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xb.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mv.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ww.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://xz.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lk.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ya.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://av.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rm.521024.cn

[F11] 复制与移动文件
来源：http://nl.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://na.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jz.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xr.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bt.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kz.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nz.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ik.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zq.panjiajie.cn

[F12] CSV 读写
来源：http://qd.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yk.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rd.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://os.yuexingan06.cn

TS:   // 同上
来源：http://ub.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ml.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jn.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rc.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nw.jianghongdianzi.cn

================================================================================
来源：http://ss.yuexingan06.cn

G. 面向对象
来源：http://pn.9csxet.cn

================================================================================
来源：http://jc.yuexingan06.cn

[G01] 定义类
来源：http://ix.jianghongdianzi.cn

Py:   class User: pass
来源：http://zl.521024.cn

PHP:  class User {}
来源：http://la.szsharing.cn

JS:   class User {}
来源：http://oi.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ye.jianghongdianzi.cn

Java: class User {}
来源：http://gh.newstarts.cn

Go:   type User struct { Name string }
来源：http://xc.szxytkj.cn

Ruby: class User; end
来源：http://gu.jctech888.com.cn

C#:   class User {}
来源：http://er.huanxung.cn

[G02] 构造函数
来源：http://on.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://go.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://sw.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://dl.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://lf.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://ui.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qj.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://rm.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://yu.lnxyls.cn

[G03] 实例属性
来源：http://kg.yuexingan06.cn

Py:   self.name = "x"
来源：http://rm.521024.cn

PHP:  public string $name = "x";
来源：http://pp.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://tg.521024.cn

TS:   name: string = "x";
来源：http://rj.yuntaijiaju.cn

Java: private String name;
来源：http://ao.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hy.jctech888.com.cn

Ruby: @name = "x"
来源：http://ar.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://sd.panjiajie.cn

[G04] 定义方法
来源：http://ft.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ru.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wd.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://we.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://sh.asd995.cn

Java: String greet() { return name; }
来源：http://sn.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nj.gzmigu.cn

Ruby: def greet; @name; end
来源：http://sk.asd995.cn

C#:   public string Greet() => Name;
来源：http://sl.wgjwhj.cn

[G05] 继承
来源：http://fz.521024.cn

Py:   class Admin(User): pass
来源：http://bs.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://we.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://eg.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://xb.nszjky.cn


<!-- 参考信息 -->