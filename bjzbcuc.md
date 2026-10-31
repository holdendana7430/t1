代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ol.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ck.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dn.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kx.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://th.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wb.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kf.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xr.yuntaijiaju.cn

[E06] 替换子串
来源：http://xg.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dy.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://fe.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vz.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://uy.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jo.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zo.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vo.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://yd.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://dd.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gu.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ne.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yy.nicolike.cn

TS:   s.split(",")
来源：http://hv.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sf.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qv.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://pf.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://be.newstarts.cn

[E08] 数组按分隔符合并
来源：http://ub.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ca.521024.cn

PHP:  implode(",", $items);
来源：http://hr.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ji.bookmarksfly.cn

TS:   items.join(",")
来源：http://zz.gzmigu.cn

Java: String.join(",", items)
来源：http://av.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://jn.yuexingan06.cn

Ruby: items.join(",")
来源：http://ou.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://tu.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://ri.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pg.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ue.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://vp.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ve.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://lo.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://on.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dy.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lf.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://tq.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uz.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nz.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://iz.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://rf.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://eq.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kv.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zc.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gk.nszjky.cn

[E11] 反转字符串
来源：http://ou.huixiangedu.cn

Py:   s[::-1]
来源：http://ww.lnxyls.cn

PHP:  strrev($s);
来源：http://om.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://xo.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://ov.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kp.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wx.chemitech.net.cn

Ruby: s.reverse
来源：http://mm.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ts.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://mw.panjiajie.cn

Py:   s.count("a")
来源：http://ht.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ll.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://qg.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://gw.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gn.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://km.nszjky.cn

Ruby: s.count("a")
来源：http://qm.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://yt.szxytkj.cn

[E13] 逐字符遍历
来源：http://bi.521024.cn

Py:   for ch in s: print(ch)
来源：http://zd.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uj.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pz.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ym.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qh.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oh.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ny.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gh.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ou.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cy.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vw.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vs.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pw.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sg.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vo.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rr.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://st.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://de.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kq.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fs.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ez.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://my.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://le.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ti.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tz.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mv.haigaiapp.cn

[E16] 数字千分位
来源：http://pk.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://rk.521024.cn

PHP:  number_format(1234567);
来源：http://hi.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://py.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ey.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kx.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rz.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aq.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://wg.nicolike.cn

[E17] 首字母大写
来源：http://fp.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ho.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://db.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ev.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dk.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wq.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bj.huixiangedu.cn

Ruby: s.capitalize
来源：http://up.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dy.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://wm.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ar.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xw.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xw.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rs.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xp.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://le.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nx.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bq.nicolike.cn

[E19] 多行文本按行拆分
来源：http://rf.muxihuayi.cn

Py:   s.splitlines()
来源：http://bw.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nj.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://cx.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://nu.huixiangedu.cn

Java: s.lines().toList()
来源：http://id.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://hp.shxzskj.cn

Ruby: s.lines
来源：http://od.szsharing.cn

C#:   s.Split('\n')
来源：http://au.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://bi.jctech888.com.cn

Py:   if not s:
来源：http://fd.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nt.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sd.bjjhwx.cn

TS:   if (s === "") {}
来源：http://sm.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://rl.asd995.cn

Go:   if s == "" {}
来源：http://aq.szxytkj.cn

Ruby: if s.empty?
来源：http://jk.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hs.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://qe.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pm.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eg.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sr.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zt.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://no.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://fe.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gn.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iw.nicolike.cn

[E22] 字节长度与字符长度
来源：http://nv.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pe.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yi.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rz.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vq.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gg.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lk.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://zh.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yg.colortex.cn

================================================================================
来源：http://zj.nszjky.cn

F. 文件与目录
来源：http://mm.nicolike.cn

================================================================================
来源：http://dp.bjjhwx.cn

[F01] 读取整个文件
来源：http://jh.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hb.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://pc.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cy.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mg.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rg.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vc.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://hp.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://pg.521024.cn

[F02] 逐行读取文件
来源：http://st.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kl.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ge.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ff.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uk.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://il.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ia.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fu.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vz.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://sk.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yj.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ae.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wc.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ke.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qe.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://br.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://tk.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fp.haigaiapp.cn

[F04] 追加写入文件
来源：http://td.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xi.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bo.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cg.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eo.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pd.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mj.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ta.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qv.521024.cn

[F05] 判断文件或目录是否存在
来源：http://vq.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ui.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://tj.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://zo.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://xq.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zs.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sz.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ux.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://ob.bookmarksfly.cn

[F06] 删除文件
来源：http://ur.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://hz.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://cm.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dp.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hv.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rr.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://te.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ps.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://ls.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://nv.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ss.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vq.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yo.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tr.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wb.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gp.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bq.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://of.nszjky.cn

[F08] 遍历目录
来源：http://pb.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uv.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://su.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://aq.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://rm.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fz.nszjky.cn

Ruby: Dir.children("dir")
来源：http://xy.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://nm.wgjwhj.cn

[F09] 获取文件大小
来源：http://ih.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://nw.colortex.cn

PHP:  filesize("a.txt");
来源：http://sq.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://sk.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://zr.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zd.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iu.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://ed.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://vs.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://rl.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cg.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qm.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mf.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://va.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gc.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bs.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ut.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://et.newstarts.cn

[F11] 复制与移动文件
来源：http://er.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iz.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iz.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uc.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yk.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bx.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mi.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://po.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fu.9csxet.cn

[F12] CSV 读写
来源：http://ph.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xz.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://of.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ig.521024.cn

TS:   // 同上
来源：http://tm.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://se.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ry.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bz.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mg.nszjky.cn

================================================================================
来源：http://ts.haigaiapp.cn

G. 面向对象
来源：http://nf.wgjwhj.cn

================================================================================
来源：http://mn.hnjuh.cn

[G01] 定义类
来源：http://ve.jctech888.com.cn

Py:   class User: pass
来源：http://uv.shtwfgs.cn

PHP:  class User {}
来源：http://ic.yuntaijiaju.cn

JS:   class User {}
来源：http://wr.asd995.cn

TS:   class User { name: string = ""; }
来源：http://hk.lnxyls.cn

Java: class User {}
来源：http://rq.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://iv.lnxyls.cn

Ruby: class User; end
来源：http://zj.yuntaijiaju.cn

C#:   class User {}
来源：http://df.bookmarksfly.cn

[G02] 构造函数
来源：http://oh.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://go.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://uk.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://rr.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://jg.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://pu.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ky.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://hn.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://mn.newstarts.cn

[G03] 实例属性
来源：http://ck.haigaiapp.cn

Py:   self.name = "x"
来源：http://aj.hnjuh.cn

PHP:  public string $name = "x";
来源：http://ri.jctech888.com.cn

JS:   this.name = "x";
来源：http://sh.shtwfgs.cn

TS:   name: string = "x";
来源：http://bs.hnjuh.cn

Java: private String name;
来源：http://bx.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ue.shxzskj.cn


<!-- 参考信息 -->