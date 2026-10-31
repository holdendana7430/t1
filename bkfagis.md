代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bn.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tx.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ca.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wm.shtwfgs.cn

[E06] 替换子串
来源：http://cc.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ip.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ww.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rx.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://cn.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fq.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bp.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ac.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://jl.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://dr.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nr.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ud.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ti.yuntaijiaju.cn

TS:   s.split(",")
来源：http://or.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jl.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bu.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://lg.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vm.nszjky.cn

[E08] 数组按分隔符合并
来源：http://nb.gzmigu.cn

Py:   ",".join(items)
来源：http://fo.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://gn.hnjuh.cn

JS:   items.join(",")
来源：http://no.9csxet.cn

TS:   items.join(",")
来源：http://st.521024.cn

Java: String.join(",", items)
来源：http://jx.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://hz.szxytkj.cn

Ruby: items.join(",")
来源：http://cm.gzmigu.cn

C#:   string.Join(",", items)
来源：http://sq.shxzukj.cn

[E09] 去除所有空白字符
来源：http://xi.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fm.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gk.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://re.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://hw.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://vs.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nl.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bx.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wp.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://yo.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zd.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mx.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://lb.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://yd.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://bd.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gb.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ix.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ap.shxzskj.cn

[E11] 反转字符串
来源：http://fx.muxihuayi.cn

Py:   s[::-1]
来源：http://oq.szxytkj.cn

PHP:  strrev($s);
来源：http://hv.521024.cn

JS:   [...s].reverse().join("")
来源：http://gn.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://rd.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://om.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://th.colortex.cn

Ruby: s.reverse
来源：http://ih.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cf.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://kg.521024.cn

Py:   s.count("a")
来源：http://bd.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://lv.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://rn.nszjky.cn

TS:   s.split("a").length - 1
来源：http://yc.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xv.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://dd.haigaiapp.cn

Ruby: s.count("a")
来源：http://ok.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://rc.hnjuh.cn

[E13] 逐字符遍历
来源：http://ay.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://zz.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://da.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ha.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://db.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eq.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jq.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vw.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cu.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://cd.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://th.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hb.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ok.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fc.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kx.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vl.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zz.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mr.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://gx.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ik.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wu.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bz.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ds.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gj.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uc.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pd.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eg.muxihuayi.cn

[E16] 数字千分位
来源：http://md.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://gu.nszjky.cn

PHP:  number_format(1234567);
来源：http://eb.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tl.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bi.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kc.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://du.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qp.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://pz.szsharing.cn

[E17] 首字母大写
来源：http://ry.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ju.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yy.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cw.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qu.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xx.hahajie.cn

Ruby: s.capitalize
来源：http://na.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mt.jctech888.com.cn

[E18] 模板占位符替换
来源：http://ru.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://py.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://du.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pk.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://me.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mx.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vh.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xv.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rt.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://kv.szxytkj.cn

Py:   s.splitlines()
来源：http://vt.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://je.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://rm.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://xy.szxytkj.cn

Java: s.lines().toList()
来源：http://gw.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ex.chemitech.net.cn

Ruby: s.lines
来源：http://yy.huixiangedu.cn

C#:   s.Split('\n')
来源：http://ov.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://oc.521024.cn

Py:   if not s:
来源：http://cy.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tb.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qy.9csxet.cn

TS:   if (s === "") {}
来源：http://zx.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://dq.lnxyls.cn

Go:   if s == "" {}
来源：http://vg.chemitech.net.cn

Ruby: if s.empty?
来源：http://si.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zn.lnxyls.cn

[E21] 超长截断加省略号
来源：http://hp.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tz.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://og.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xx.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ax.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ur.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ym.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cm.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ir.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://eb.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ot.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nv.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hd.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pg.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://al.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://rv.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ii.panjiajie.cn

================================================================================
来源：http://pr.hahajie.cn

F. 文件与目录
来源：http://kr.jctech888.com.cn

================================================================================
来源：http://go.muxihuayi.cn

[F01] 读取整个文件
来源：http://gk.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lt.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://cr.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ar.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tv.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sl.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vr.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ut.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ph.szsharing.cn

[F02] 逐行读取文件
来源：http://cv.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yz.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bx.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ez.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yy.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bc.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pz.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mi.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lb.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://uq.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qd.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pf.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://by.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rw.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pj.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dv.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://sv.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ii.bjjhwx.cn

[F04] 追加写入文件
来源：http://xn.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oh.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wf.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gu.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fs.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aq.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://im.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sa.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ay.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://qr.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://du.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://ow.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://hl.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://sr.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hl.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hb.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://jb.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://dw.colortex.cn

[F06] 删除文件
来源：http://kn.nicolike.cn

Py:   os.remove("a.txt")
来源：http://ba.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://yh.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oc.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rd.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://py.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://vy.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://tu.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://vd.521024.cn

[F07] 创建目录（含多级）
来源：http://os.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://at.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qq.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ws.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qz.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hf.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gr.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yr.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://of.yuntaijiaju.cn

[F08] 遍历目录
来源：http://qb.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ud.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lm.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://zn.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://yr.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iq.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ny.521024.cn

Ruby: Dir.children("dir")
来源：http://gs.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://nt.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://pd.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://qn.huanxung.cn

PHP:  filesize("a.txt");
来源：http://mu.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ai.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://fc.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oq.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xw.9csxet.cn

Ruby: File.size("a.txt")
来源：http://gy.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://de.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://gy.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ms.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mi.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://oj.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ia.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tm.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hb.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ol.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://oy.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://og.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sf.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jw.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hl.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rr.gzmigu.cn

[F12] CSV 读写
来源：http://bx.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ee.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ic.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mw.shtwfgs.cn

TS:   // 同上
来源：http://xk.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zo.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vf.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ez.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ys.bjjhwx.cn

================================================================================
来源：http://vi.gzmigu.cn

G. 面向对象
来源：http://or.wgjwhj.cn

================================================================================
来源：http://tl.hahajie.cn

[G01] 定义类
来源：http://xd.jctech888.com.cn

Py:   class User: pass
来源：http://yb.wgjwhj.cn

PHP:  class User {}
来源：http://gy.huixinmuqiang.cn

JS:   class User {}
来源：http://rh.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://qd.hnjuh.cn

Java: class User {}
来源：http://ak.hnjuh.cn

Go:   type User struct { Name string }
来源：http://vm.nicolike.cn

Ruby: class User; end
来源：http://ab.huanxung.cn

C#:   class User {}
来源：http://qr.wgjwhj.cn

[G02] 构造函数
来源：http://ui.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://dh.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://us.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://jt.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://xk.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://hx.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hh.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://jh.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ww.huixinmuqiang.cn

[G03] 实例属性
来源：http://lr.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://ss.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://sv.chemitech.net.cn

JS:   this.name = "x";
来源：http://ui.szsharing.cn

TS:   name: string = "x";
来源：http://lw.haigaiapp.cn

Java: private String name;
来源：http://dn.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pv.bookmarksfly.cn

Ruby: @name = "x"
来源：http://yk.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://io.szsharing.cn

[G04] 定义方法
来源：http://wl.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://lc.huixiangedu.cn


<!-- 参考信息 -->