代发 wailian999

C#:   s.Replace("a", "b")
来源：http://sj.nszjky.cn

[E07] 按分隔符拆分
来源：http://yi.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gs.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kz.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yj.bjjhwx.cn

TS:   s.split(",")
来源：http://li.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fg.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wv.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://yx.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ox.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://wy.521024.cn

Py:   ",".join(items)
来源：http://tk.nicolike.cn

PHP:  implode(",", $items);
来源：http://jj.shxzukj.cn

JS:   items.join(",")
来源：http://ju.shxzukj.cn

TS:   items.join(",")
来源：http://yq.muxihuayi.cn

Java: String.join(",", items)
来源：http://he.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://mk.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://fg.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://rd.szxytkj.cn

[E09] 去除所有空白字符
来源：http://hl.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://up.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dw.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://io.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://lu.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://vx.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gm.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hg.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nx.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://cl.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ga.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://de.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://ea.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://fm.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://ba.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hp.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sm.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://he.szxytkj.cn

[E11] 反转字符串
来源：http://cj.9csxet.cn

Py:   s[::-1]
来源：http://td.bjjhwx.cn

PHP:  strrev($s);
来源：http://ru.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://ol.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://eb.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jj.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wo.521024.cn

Ruby: s.reverse
来源：http://iz.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oi.nicolike.cn

[E12] 统计某字符出现次数
来源：http://kz.huixiangedu.cn

Py:   s.count("a")
来源：http://vv.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://vb.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://iu.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://st.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ku.asd995.cn

Go:   strings.Count(s, "a")
来源：http://pn.jctech888.com.cn

Ruby: s.count("a")
来源：http://go.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://in.nicolike.cn

[E13] 逐字符遍历
来源：http://ek.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://af.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sf.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hc.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gn.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tr.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ac.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tk.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xm.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://go.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://za.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://po.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xs.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cl.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jr.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fe.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vv.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pl.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://hb.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gp.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xa.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xt.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sn.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kr.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ek.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fv.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nc.huixiangedu.cn

[E16] 数字千分位
来源：http://tu.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://na.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://zd.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hk.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pj.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ht.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ll.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fe.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://kc.lnxyls.cn

[E17] 首字母大写
来源：http://hn.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mg.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ck.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xl.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yg.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ah.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sh.9csxet.cn

Ruby: s.capitalize
来源：http://ja.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yb.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://vo.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jf.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ln.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xf.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dk.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wn.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lw.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zb.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nt.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://vv.szsharing.cn

Py:   s.splitlines()
来源：http://zk.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zb.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://zz.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://cu.huixiangedu.cn

Java: s.lines().toList()
来源：http://ph.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://rj.shxzukj.cn

Ruby: s.lines
来源：http://af.lnxyls.cn

C#:   s.Split('\n')
来源：http://bi.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ti.shxzskj.cn

Py:   if not s:
来源：http://sa.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://us.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rk.huixiangedu.cn

TS:   if (s === "") {}
来源：http://ci.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://hw.yuexingan06.cn

Go:   if s == "" {}
来源：http://ne.chemitech.net.cn

Ruby: if s.empty?
来源：http://yv.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gu.asd995.cn

[E21] 超长截断加省略号
来源：http://wy.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://db.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ox.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tq.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mm.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fs.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://qg.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bm.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ct.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://tg.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zo.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lz.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kk.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ft.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mk.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://to.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dd.hnjuh.cn

================================================================================
来源：http://mv.asd995.cn

F. 文件与目录
来源：http://kv.huixinmuqiang.cn

================================================================================
来源：http://gh.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://xq.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hq.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ws.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tq.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ok.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mb.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ov.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://tw.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://hh.haigaiapp.cn

[F02] 逐行读取文件
来源：http://xv.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bf.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ob.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xq.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bi.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dx.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://or.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ga.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zt.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://cm.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ar.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bz.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sx.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dm.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vf.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kb.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://sq.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jt.9csxet.cn

[F04] 追加写入文件
来源：http://by.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ed.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qn.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ge.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://md.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ym.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ot.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ez.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zb.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://vx.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kk.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://zk.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://yp.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://tb.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bx.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://go.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://sv.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://en.yuntaijiaju.cn

[F06] 删除文件
来源：http://sw.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://ft.521024.cn

PHP:  unlink("a.txt");
来源：http://bc.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mq.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ha.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oh.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://py.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://aw.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://nv.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://ya.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://li.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fw.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ri.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bo.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yo.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wt.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pd.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jm.szxytkj.cn

[F08] 遍历目录
来源：http://dg.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ml.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rr.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://kf.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://oy.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ce.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mi.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://qu.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://fv.shxzukj.cn

[F09] 获取文件大小
来源：http://le.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://bb.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://tc.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ie.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://br.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bp.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bc.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://qg.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://tp.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://nb.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fa.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hl.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gj.asd995.cn

TS:   path.extname("a.txt")
来源：http://zf.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tt.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pz.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xf.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hi.nszjky.cn

[F11] 复制与移动文件
来源：http://yr.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mn.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://re.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ox.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hi.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jz.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ym.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zc.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qs.nszjky.cn

[F12] CSV 读写
来源：http://sv.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kp.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pm.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nn.newstarts.cn

TS:   // 同上
来源：http://ne.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xg.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nz.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xq.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bk.nszjky.cn

================================================================================
来源：http://iy.hahajie.cn

G. 面向对象
来源：http://mq.gzmigu.cn

================================================================================
来源：http://ae.yuntaijiaju.cn

[G01] 定义类
来源：http://gq.asd995.cn

Py:   class User: pass
来源：http://gw.asd995.cn

PHP:  class User {}
来源：http://ai.yuntaijiaju.cn

JS:   class User {}
来源：http://vy.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://dd.huixiangedu.cn

Java: class User {}
来源：http://ko.szsharing.cn

Go:   type User struct { Name string }
来源：http://ml.huanxung.cn

Ruby: class User; end
来源：http://dp.shxzukj.cn

C#:   class User {}
来源：http://ma.yuntaijiaju.cn

[G02] 构造函数
来源：http://yq.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://gb.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://sv.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://iv.colortex.cn

TS:   constructor(public name: string) {}
来源：http://rf.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://qr.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gw.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://tr.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://yh.bjjhwx.cn

[G03] 实例属性
来源：http://hs.gzmigu.cn

Py:   self.name = "x"
来源：http://no.gzmigu.cn

PHP:  public string $name = "x";
来源：http://ce.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://zc.nszjky.cn

TS:   name: string = "x";
来源：http://uk.asd995.cn

Java: private String name;
来源：http://gl.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cc.newstarts.cn

Ruby: @name = "x"
来源：http://zh.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://xn.haigaiapp.cn

[G04] 定义方法
来源：http://gx.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://fj.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hi.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://ee.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://zg.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ah.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://my.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://zu.newstarts.cn

C#:   public string Greet() => Name;
来源：http://bt.huixiangedu.cn

[G05] 继承
来源：http://ry.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ef.colortex.cn

PHP:  class Admin extends User {}
来源：http://uu.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://cq.szxytkj.cn

TS:   class Admin extends User {}
来源：http://yz.wgjwhj.cn


<!-- 参考信息 -->