代发 wailian999

Go:   strings.Index(s, "x")
来源：http://qx.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://gn.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ij.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dm.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sg.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sl.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://my.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pt.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sw.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ex.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vz.newstarts.cn

[E06] 替换子串
来源：http://ow.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ek.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://sa.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yw.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://dl.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://af.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vq.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dw.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://qa.colortex.cn

[E07] 按分隔符拆分
来源：http://gy.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yh.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cg.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://po.9csxet.cn

TS:   s.split(",")
来源：http://ow.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://js.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://te.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://gd.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lo.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://be.muxihuayi.cn

Py:   ",".join(items)
来源：http://mw.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://aw.nicolike.cn

JS:   items.join(",")
来源：http://eo.yuexingan06.cn

TS:   items.join(",")
来源：http://vu.shxzskj.cn

Java: String.join(",", items)
来源：http://ct.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://ov.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://rt.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://vf.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://gk.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fi.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ur.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://qs.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://kq.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://pv.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bt.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ks.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ar.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://ri.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ho.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oj.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://hc.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://le.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://ed.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lz.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bg.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ji.hnjuh.cn

[E11] 反转字符串
来源：http://yq.nicolike.cn

Py:   s[::-1]
来源：http://ns.chemitech.net.cn

PHP:  strrev($s);
来源：http://fr.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://qj.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://fq.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ij.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kb.yuexingan06.cn

Ruby: s.reverse
来源：http://wi.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jh.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://ow.shxzskj.cn

Py:   s.count("a")
来源：http://ys.colortex.cn

PHP:  substr_count($s, "a");
来源：http://qx.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://qx.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://pv.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qo.521024.cn

Go:   strings.Count(s, "a")
来源：http://ea.huanxung.cn

Ruby: s.count("a")
来源：http://pf.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://bi.shxzskj.cn

[E13] 逐字符遍历
来源：http://pz.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://sq.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fw.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://za.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wy.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cp.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lm.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wv.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://sm.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gd.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bn.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oy.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ca.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uq.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ij.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nx.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nf.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ag.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cj.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ux.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iw.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ti.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ui.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yf.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hh.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qv.shxzskj.cn

[E16] 数字千分位
来源：http://gq.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://pq.panjiajie.cn

PHP:  number_format(1234567);
来源：http://kh.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ms.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ey.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://no.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lp.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sd.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://gv.nszjky.cn

[E17] 首字母大写
来源：http://os.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yq.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ox.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bv.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vg.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pi.nicolike.cn

Ruby: s.capitalize
来源：http://gv.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fr.jctech888.com.cn

[E18] 模板占位符替换
来源：http://qd.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ci.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vg.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://as.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://po.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pg.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gr.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wf.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://us.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://nl.huanxung.cn

Py:   s.splitlines()
来源：http://dz.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://oy.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ne.hahajie.cn

Java: s.lines().toList()
来源：http://jy.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://wh.hahajie.cn

Ruby: s.lines
来源：http://cl.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://pz.szsharing.cn

[E20] 判断字符串是否为空
来源：http://ze.nicolike.cn

Py:   if not s:
来源：http://fe.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xb.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cl.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ry.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://vb.shxzskj.cn

Go:   if s == "" {}
来源：http://zq.haigaiapp.cn

Ruby: if s.empty?
来源：http://us.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tv.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://zk.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xz.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zy.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zb.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hb.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ra.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://pe.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kn.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mp.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://mw.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bq.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yo.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rs.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tn.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://av.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kx.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://qq.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kt.jctech888.com.cn

================================================================================
来源：http://bi.huixinmuqiang.cn

F. 文件与目录
来源：http://rb.newstarts.cn

================================================================================
来源：http://cv.hahajie.cn

[F01] 读取整个文件
来源：http://cc.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wl.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://ol.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dh.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lz.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://za.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://zw.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://iq.shxzskj.cn

[F02] 逐行读取文件
来源：http://jy.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://st.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://de.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dm.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qu.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oo.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dt.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ja.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bf.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://qq.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tk.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zn.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pf.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yq.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nx.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pv.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://xu.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pm.jctech888.com.cn

[F04] 追加写入文件
来源：http://cs.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cx.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ub.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rk.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wp.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sm.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ka.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xc.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vg.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://ja.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aq.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://lc.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://nx.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://uz.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uh.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fu.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://md.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://bz.521024.cn

[F06] 删除文件
来源：http://fi.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ur.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://mm.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://et.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cd.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nu.colortex.cn

Go:   os.Remove("a.txt")
来源：http://gh.colortex.cn

Ruby: File.delete("a.txt")
来源：http://ja.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://vm.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ku.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ae.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ip.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tb.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pj.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yd.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dt.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://my.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bp.nicolike.cn

[F08] 遍历目录
来源：http://gg.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lx.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sy.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://ph.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ht.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wz.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xb.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://qg.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://ye.nszjky.cn

[F09] 获取文件大小
来源：http://ay.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://iy.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://kr.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://hi.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://hn.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://al.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rq.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://zb.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://te.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ay.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ow.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qo.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qx.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ho.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://th.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vm.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ic.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fj.szxytkj.cn

[F11] 复制与移动文件
来源：http://rw.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ee.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fi.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rn.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ri.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gs.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ji.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jw.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mu.huixiangedu.cn

[F12] CSV 读写
来源：http://lg.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cf.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cv.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pq.colortex.cn

TS:   // 同上
来源：http://cz.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rd.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vd.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ts.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ar.szsharing.cn

================================================================================
来源：http://fc.nszjky.cn

G. 面向对象
来源：http://gs.wgjwhj.cn

================================================================================
来源：http://ov.521024.cn

[G01] 定义类
来源：http://xn.521024.cn

Py:   class User: pass
来源：http://lf.colortex.cn

PHP:  class User {}
来源：http://ka.shtwfgs.cn

JS:   class User {}
来源：http://zn.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ox.haigaiapp.cn

Java: class User {}
来源：http://nz.shxzskj.cn

Go:   type User struct { Name string }
来源：http://sj.jianghongdianzi.cn

Ruby: class User; end
来源：http://cj.huanxung.cn

C#:   class User {}
来源：http://wp.chemitech.net.cn

[G02] 构造函数
来源：http://oe.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://mt.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://nv.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://tx.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://da.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://uf.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hm.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://mp.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://rm.bjjhwx.cn

[G03] 实例属性
来源：http://gs.nszjky.cn

Py:   self.name = "x"
来源：http://mm.szxytkj.cn

PHP:  public string $name = "x";
来源：http://pf.huixinmuqiang.cn


<!-- 参考信息 -->