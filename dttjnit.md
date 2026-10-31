代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://np.asd995.cn

TS:   s.split(",")
来源：http://db.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ny.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sd.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://gi.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://al.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://xd.nicolike.cn

Py:   ",".join(items)
来源：http://tg.colortex.cn

PHP:  implode(",", $items);
来源：http://fl.muxihuayi.cn

JS:   items.join(",")
来源：http://cg.szsharing.cn

TS:   items.join(",")
来源：http://ux.shtwfgs.cn

Java: String.join(",", items)
来源：http://gq.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://mv.szsharing.cn

Ruby: items.join(",")
来源：http://xy.szxytkj.cn

C#:   string.Join(",", items)
来源：http://fa.nicolike.cn

[E09] 去除所有空白字符
来源：http://ev.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ui.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jj.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://fi.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://gj.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://cu.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ei.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://te.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uv.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://gb.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wn.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dt.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://rx.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ii.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://pr.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fe.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zq.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yb.jianghongdianzi.cn

[E11] 反转字符串
来源：http://xb.gzmigu.cn

Py:   s[::-1]
来源：http://fz.yuexingan06.cn

PHP:  strrev($s);
来源：http://ad.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://ha.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://qs.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gn.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vv.yuexingan06.cn

Ruby: s.reverse
来源：http://wz.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pi.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://jo.nicolike.cn

Py:   s.count("a")
来源：http://pu.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://um.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://oz.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://tx.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ur.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://cc.shxzukj.cn

Ruby: s.count("a")
来源：http://wn.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://ut.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://el.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://na.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oh.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gm.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gg.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hj.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jh.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hx.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sq.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://dy.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cl.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ot.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ey.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sv.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hi.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vf.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qg.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ft.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://io.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bj.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gh.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wb.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fd.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fh.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wk.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ca.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vi.shxzukj.cn

[E16] 数字千分位
来源：http://tc.nicolike.cn

Py:   f"{1234567:,}"
来源：http://kn.nszjky.cn

PHP:  number_format(1234567);
来源：http://ew.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pe.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mn.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://np.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nw.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sa.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ex.huanxung.cn

[E17] 首字母大写
来源：http://ig.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mi.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pq.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nz.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nq.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iz.nicolike.cn

Ruby: s.capitalize
来源：http://eo.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lr.shxzukj.cn

[E18] 模板占位符替换
来源：http://lt.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ut.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zu.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tg.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zo.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sw.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gx.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mq.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ri.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://zb.lnxyls.cn

Py:   s.splitlines()
来源：http://da.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yg.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://so.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://ga.521024.cn

Java: s.lines().toList()
来源：http://wo.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://xd.gzmigu.cn

Ruby: s.lines
来源：http://sa.newstarts.cn

C#:   s.Split('\n')
来源：http://el.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://er.yuntaijiaju.cn

Py:   if not s:
来源：http://zd.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tx.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sy.9csxet.cn

TS:   if (s === "") {}
来源：http://qa.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://kt.shxzskj.cn

Go:   if s == "" {}
来源：http://fh.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://qe.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ux.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://ck.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gv.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hu.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cp.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lr.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ok.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://wp.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ge.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rb.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://zm.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lw.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gs.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fa.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bn.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tx.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dy.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://cw.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cw.bookmarksfly.cn

================================================================================
来源：http://zg.wgjwhj.cn

F. 文件与目录
来源：http://nm.huixiangedu.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://gg.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sf.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://da.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iq.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ts.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://to.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nz.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://vu.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ss.shxzskj.cn

[F02] 逐行读取文件
来源：http://ge.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dm.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://in.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rb.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sy.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dc.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ve.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lb.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://zw.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vd.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kp.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://co.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lc.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://li.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ae.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://nx.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kx.gzmigu.cn

[F04] 追加写入文件
来源：http://id.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://om.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tg.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://po.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rc.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ui.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gp.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://au.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bl.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://dc.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fr.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://th.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://pc.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://qe.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xp.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rd.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://se.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://gg.newstarts.cn

[F06] 删除文件
来源：http://vy.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://tz.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://ge.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rb.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dj.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://na.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://ie.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://fj.colortex.cn

C#:   File.Delete("a.txt");
来源：http://ia.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ta.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://de.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rl.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nw.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tg.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xh.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vx.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oq.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://li.huixinmuqiang.cn

[F08] 遍历目录
来源：http://qb.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lk.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tv.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://tw.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://fr.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://da.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gy.asd995.cn

Ruby: Dir.children("dir")
来源：http://yk.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://oj.panjiajie.cn

[F09] 获取文件大小
来源：http://ic.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://us.colortex.cn

PHP:  filesize("a.txt");
来源：http://tx.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://jz.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://cu.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ct.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jc.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://mn.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://de.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://eh.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ih.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ry.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wm.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://qu.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ux.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iq.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ey.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pg.yuexingan06.cn

[F11] 复制与移动文件
来源：http://ur.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jv.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ii.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ku.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hf.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hc.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oy.haigaiapp.cn

[F12] CSV 读写
来源：http://ph.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lj.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mh.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hb.haigaiapp.cn

TS:   // 同上
来源：http://gw.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ay.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://az.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xq.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gk.gzmigu.cn

================================================================================
来源：http://ca.newstarts.cn

G. 面向对象
来源：http://rs.nszjky.cn

================================================================================
来源：http://td.hnjuh.cn

[G01] 定义类
来源：http://re.szxytkj.cn

Py:   class User: pass
来源：http://qm.huixiangedu.cn

PHP:  class User {}
来源：http://jm.bookmarksfly.cn

JS:   class User {}
来源：http://gv.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://rf.colortex.cn

Java: class User {}
来源：http://wd.shxzskj.cn

Go:   type User struct { Name string }
来源：http://wb.wgjwhj.cn

Ruby: class User; end
来源：http://zi.muxihuayi.cn

C#:   class User {}
来源：http://ph.wgjwhj.cn

[G02] 构造函数
来源：http://dg.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://oq.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ul.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://vj.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://qy.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://fu.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jt.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://yl.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://zl.shxzukj.cn

[G03] 实例属性
来源：http://qs.huanxung.cn

Py:   self.name = "x"
来源：http://fv.panjiajie.cn

PHP:  public string $name = "x";
来源：http://eb.newstarts.cn

JS:   this.name = "x";
来源：http://gj.szxytkj.cn

TS:   name: string = "x";
来源：http://ll.huixinmuqiang.cn

Java: private String name;
来源：http://mm.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pn.yuexingan06.cn

Ruby: @name = "x"
来源：http://uw.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://mb.szsharing.cn

[G04] 定义方法
来源：http://ri.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://hs.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ir.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://wh.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ye.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://as.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vf.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://fs.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://tn.nszjky.cn

[G05] 继承
来源：http://gg.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://vk.asd995.cn

PHP:  class Admin extends User {}
来源：http://fv.panjiajie.cn

JS:   class Admin extends User {}
来源：http://tt.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://fz.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://bx.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vw.hahajie.cn

Ruby: class Admin < User; end
来源：http://hx.nszjky.cn

C#:   class Admin : User {}
来源：http://oy.9csxet.cn


<!-- 参考信息 -->