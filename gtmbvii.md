代发 wailian999

PHP:  strpos($s, "x");
来源：http://zw.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ba.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://qh.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://fj.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://zb.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://vc.nicolike.cn

C#:   s.IndexOf("x")
来源：http://gx.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rk.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qm.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ph.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qf.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sv.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xv.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gw.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zz.bjjhwx.cn

[E06] 替换子串
来源：http://ll.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tc.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://mn.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://br.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://om.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://me.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qb.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qd.asd995.cn

C#:   s.Replace("a", "b")
来源：http://sa.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://mk.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ce.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yc.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hu.colortex.cn

TS:   s.split(",")
来源：http://sk.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gp.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yf.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://tl.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://db.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://rx.wgjwhj.cn

Py:   ",".join(items)
来源：http://pb.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://rh.gzmigu.cn

JS:   items.join(",")
来源：http://xe.huixiangedu.cn

TS:   items.join(",")
来源：http://rf.gzmigu.cn

Java: String.join(",", items)
来源：http://nb.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://fl.nszjky.cn

Ruby: items.join(",")
来源：http://yz.asd995.cn

C#:   string.Join(",", items)
来源：http://ka.nszjky.cn

[E09] 去除所有空白字符
来源：http://ed.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pb.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://se.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://sp.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://qh.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://xj.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yq.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ty.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gi.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://vh.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ei.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://af.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://li.521024.cn

TS:   "7".padStart(3, "0")
来源：http://nr.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://mq.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wq.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tk.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qc.huanxung.cn

[E11] 反转字符串
来源：http://bs.nicolike.cn

Py:   s[::-1]
来源：http://oc.szsharing.cn

PHP:  strrev($s);
来源：http://jb.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://lm.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://bz.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rk.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pl.nicolike.cn

Ruby: s.reverse
来源：http://ll.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xd.hahajie.cn

[E12] 统计某字符出现次数
来源：http://ve.lnxyls.cn

Py:   s.count("a")
来源：http://ep.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://kh.colortex.cn

JS:   s.split("a").length - 1
来源：http://gd.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://qi.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nm.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://dw.yuexingan06.cn

Ruby: s.count("a")
来源：http://qh.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://py.huanxung.cn

[E13] 逐字符遍历
来源：http://fi.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://yl.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zv.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://at.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jk.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tr.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sc.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ry.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hk.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://ah.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zm.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yk.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ac.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fv.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ee.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wb.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://or.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ne.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://nf.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lk.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rw.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://js.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tx.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ii.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mw.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gg.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tk.shxzskj.cn

[E16] 数字千分位
来源：http://vj.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://sm.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ze.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yc.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gn.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dl.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gj.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sq.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://iy.nicolike.cn

[E17] 首字母大写
来源：http://ys.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nh.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ui.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nh.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ho.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wn.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kq.shxzukj.cn

Ruby: s.capitalize
来源：http://cm.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://la.9csxet.cn

[E18] 模板占位符替换
来源：http://vo.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bc.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fo.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qc.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ul.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ql.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vo.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bl.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zb.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://fm.hnjuh.cn

Py:   s.splitlines()
来源：http://gm.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sb.521024.cn

JS:   s.split(/\r?\n/)
来源：http://an.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://bj.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://fa.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://hb.hnjuh.cn

Ruby: s.lines
来源：http://ij.asd995.cn

C#:   s.Split('\n')
来源：http://tz.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://jh.521024.cn

Py:   if not s:
来源：http://ps.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fe.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fk.shxzskj.cn

TS:   if (s === "") {}
来源：http://hc.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ai.panjiajie.cn

Go:   if s == "" {}
来源：http://gn.szsharing.cn

Ruby: if s.empty?
来源：http://ue.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ez.shxzskj.cn

[E21] 超长截断加省略号
来源：http://vq.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fq.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://il.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qq.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://xe.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fz.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mi.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://fu.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zo.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qq.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://st.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lv.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yo.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://fd.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rs.huixiangedu.cn

================================================================================
来源：http://kf.asd995.cn

F. 文件与目录
来源：http://dy.haigaiapp.cn

================================================================================
来源：http://mh.huanxung.cn

[F01] 读取整个文件
来源：http://za.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nw.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://nl.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tc.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sk.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://td.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lp.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://pd.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://pt.muxihuayi.cn

[F02] 逐行读取文件
来源：http://sp.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cp.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ov.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kl.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nx.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cq.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xp.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rw.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jx.colortex.cn

[F03] 写入文件（覆盖）
来源：http://vr.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fg.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://je.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rk.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tg.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nr.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sk.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://qq.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ed.szxytkj.cn

[F04] 追加写入文件
来源：http://mc.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cm.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dx.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ga.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pd.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sn.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yp.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sg.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qh.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://lv.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ga.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ui.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ni.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://sl.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sv.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dc.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://dy.521024.cn

C#:   File.Exists("a.txt")
来源：http://zf.muxihuayi.cn

[F06] 删除文件
来源：http://bp.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://dn.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://vu.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ho.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hm.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pl.colortex.cn

Go:   os.Remove("a.txt")
来源：http://fn.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://qu.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://hd.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://sn.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ka.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yt.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hf.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wn.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xq.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zk.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pa.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vo.shxzskj.cn

[F08] 遍历目录
来源：http://cf.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oi.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vb.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://mp.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://gy.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xu.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mc.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://pg.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://sx.newstarts.cn

[F09] 获取文件大小
来源：http://gh.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://kq.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://bp.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://sw.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://bx.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fz.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://db.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://mv.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://co.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://in.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fd.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ac.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lk.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ys.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dt.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hs.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yc.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ge.bjjhwx.cn

[F11] 复制与移动文件
来源：http://ed.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ot.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nk.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lw.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vz.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vx.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://he.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dd.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qd.panjiajie.cn

[F12] CSV 读写
来源：http://cu.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xg.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xd.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://om.bjjhwx.cn

TS:   // 同上
来源：http://vi.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fa.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cj.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iw.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cn.huixiangedu.cn

================================================================================
来源：http://nw.panjiajie.cn

G. 面向对象
来源：http://uy.szxytkj.cn

================================================================================
来源：http://jy.colortex.cn

[G01] 定义类
来源：http://hy.huanxung.cn

Py:   class User: pass
来源：http://lf.nszjky.cn

PHP:  class User {}
来源：http://eb.bjjhwx.cn

JS:   class User {}
来源：http://bg.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://va.9csxet.cn

Java: class User {}
来源：http://mn.panjiajie.cn

Go:   type User struct { Name string }
来源：http://sd.jianghongdianzi.cn

Ruby: class User; end
来源：http://gr.9csxet.cn

C#:   class User {}
来源：http://bx.jianghongdianzi.cn

[G02] 构造函数
来源：http://aw.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://tx.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://gs.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://qr.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://yb.521024.cn

Java: User(String name) { this.name = name; }
来源：http://ax.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://is.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://rc.haigaiapp.cn


<!-- 参考信息 -->