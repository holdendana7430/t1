代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fn.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tw.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ji.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zv.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jg.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qw.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tj.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mp.wgjwhj.cn

[E06] 替换子串
来源：http://sr.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fc.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://gt.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ss.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://dd.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lm.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tc.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qv.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://bo.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://mp.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yc.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cc.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://es.hnjuh.cn

TS:   s.split(",")
来源：http://xk.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://em.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nv.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://et.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://go.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://ke.szsharing.cn

Py:   ",".join(items)
来源：http://vn.9csxet.cn

PHP:  implode(",", $items);
来源：http://qd.huixiangedu.cn

JS:   items.join(",")
来源：http://bh.hahajie.cn

TS:   items.join(",")
来源：http://dk.muxihuayi.cn

Java: String.join(",", items)
来源：http://cf.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://ck.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://iu.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://jn.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://mb.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rw.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tw.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ph.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://rx.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://zq.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vj.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ty.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nw.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://uv.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ki.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nl.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://kp.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://rc.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://kr.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mj.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rk.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gd.asd995.cn

[E11] 反转字符串
来源：http://lm.muxihuayi.cn

Py:   s[::-1]
来源：http://rj.jctech888.com.cn

PHP:  strrev($s);
来源：http://zj.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ff.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://wt.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qv.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ci.huanxung.cn

Ruby: s.reverse
来源：http://xa.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gl.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://sr.shtwfgs.cn

Py:   s.count("a")
来源：http://zf.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://wo.9csxet.cn

JS:   s.split("a").length - 1
来源：http://zt.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://cv.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bc.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://tk.nszjky.cn

Ruby: s.count("a")
来源：http://la.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://ol.nicolike.cn

[E13] 逐字符遍历
来源：http://st.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://ln.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hp.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dm.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jz.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kr.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fr.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zl.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uk.asd995.cn

[E14] URL 编码与 Base64
来源：http://fb.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rt.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bk.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lu.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://op.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rz.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ds.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vp.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ik.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://vm.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bs.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jw.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://de.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ob.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://km.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://on.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://px.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wv.shtwfgs.cn

[E16] 数字千分位
来源：http://vg.nszjky.cn

Py:   f"{1234567:,}"
来源：http://wo.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://wx.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iu.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lo.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zz.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pk.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hm.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://tp.gzmigu.cn

[E17] 首字母大写
来源：http://pt.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hr.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ie.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qg.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ci.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gc.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://os.haigaiapp.cn

Ruby: s.capitalize
来源：http://xz.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jr.nicolike.cn

[E18] 模板占位符替换
来源：http://hx.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ju.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mu.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tp.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fb.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vz.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gr.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bm.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qs.nicolike.cn

[E19] 多行文本按行拆分
来源：http://je.szxytkj.cn

Py:   s.splitlines()
来源：http://gg.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jn.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://sl.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ej.bookmarksfly.cn

Java: s.lines().toList()
来源：http://yf.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://dr.shxzskj.cn

Ruby: s.lines
来源：http://vi.hahajie.cn

C#:   s.Split('\n')
来源：http://ex.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://yc.huanxung.cn

Py:   if not s:
来源：http://yd.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jt.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xb.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://hy.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://vj.9csxet.cn

Go:   if s == "" {}
来源：http://rb.9csxet.cn

Ruby: if s.empty?
来源：http://rc.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://th.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://di.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kt.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ce.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sf.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ny.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://du.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://qy.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ig.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uh.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://ar.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://do.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sb.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pj.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gh.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mm.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://dq.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ne.asd995.cn

================================================================================
来源：http://uj.huixiangedu.cn

F. 文件与目录
来源：http://yi.hahajie.cn

================================================================================
来源：http://qz.panjiajie.cn

[F01] 读取整个文件
来源：http://tv.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qy.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ow.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ql.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lh.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sr.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mb.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://wn.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://ie.hahajie.cn

[F02] 逐行读取文件
来源：http://yt.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ju.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vi.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kx.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ha.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sr.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tp.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ox.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hk.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://bp.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://np.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vd.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sc.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://er.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iv.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qy.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://rn.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cs.nszjky.cn

[F04] 追加写入文件
来源：http://wp.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fz.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sh.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://za.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uy.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tj.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wr.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gj.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wi.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://gr.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hi.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://xm.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ga.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://nt.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bi.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xs.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://iu.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://zw.wgjwhj.cn

[F06] 删除文件
来源：http://sy.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://vm.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://bk.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jm.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hd.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://di.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://dj.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://vj.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://md.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://kh.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ex.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jc.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hv.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vm.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qy.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nh.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ha.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pt.haigaiapp.cn

[F08] 遍历目录
来源：http://db.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lu.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hv.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://pg.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://qe.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kf.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oy.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://fg.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://vj.shxzukj.cn

[F09] 获取文件大小
来源：http://lu.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://lt.asd995.cn

PHP:  filesize("a.txt");
来源：http://ly.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://nb.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://tc.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vy.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ks.9csxet.cn

Ruby: File.size("a.txt")
来源：http://kt.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hr.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://dz.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nk.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qo.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qv.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ij.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xv.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xa.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://at.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://am.szxytkj.cn

[F11] 复制与移动文件
来源：http://ug.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sa.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cg.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yy.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ex.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fl.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wd.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yi.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iz.huixiangedu.cn

[F12] CSV 读写
来源：http://ce.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pm.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cz.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://at.shxzskj.cn

TS:   // 同上
来源：http://wf.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ei.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gc.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vh.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cz.hahajie.cn

================================================================================
来源：http://ei.bookmarksfly.cn

G. 面向对象
来源：http://sd.9csxet.cn

================================================================================
来源：http://gm.jianghongdianzi.cn

[G01] 定义类
来源：http://wz.haigaiapp.cn

Py:   class User: pass
来源：http://eb.hahajie.cn

PHP:  class User {}
来源：http://cz.bookmarksfly.cn

JS:   class User {}
来源：http://vj.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://he.huanxung.cn

Java: class User {}
来源：http://sc.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://hj.shxzskj.cn

Ruby: class User; end
来源：http://rp.muxihuayi.cn

C#:   class User {}
来源：http://bb.yuexingan06.cn

[G02] 构造函数
来源：http://wr.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://ut.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://so.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://pc.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://hf.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://vx.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jl.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://fx.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://bf.lnxyls.cn

[G03] 实例属性
来源：http://vl.panjiajie.cn

Py:   self.name = "x"
来源：http://ne.asd995.cn

PHP:  public string $name = "x";
来源：http://zj.wgjwhj.cn

JS:   this.name = "x";
来源：http://ss.asd995.cn

TS:   name: string = "x";
来源：http://rh.yuexingan06.cn

Java: private String name;
来源：http://tl.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jx.521024.cn


<!-- 参考信息 -->