代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yn.521024.cn

TS:   s.slice(1, 4)
来源：http://zd.huanxung.cn

Java: s.substring(1, 4)
来源：http://fd.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rd.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pb.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://qf.shxzskj.cn

[E04] 查找子串位置
来源：http://su.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://nb.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://qn.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xb.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://tq.hnjuh.cn

Java: s.indexOf("x")
来源：http://zx.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://cl.newstarts.cn

Ruby: s.index("x")
来源：http://wl.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://fx.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sq.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aw.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vi.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xj.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zm.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vq.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wr.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ij.nszjky.cn

[E06] 替换子串
来源：http://ez.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dg.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://ss.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://po.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://vn.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ya.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xq.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rv.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://bk.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://hu.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://my.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qu.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zw.lnxyls.cn

TS:   s.split(",")
来源：http://wk.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wm.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qk.asd995.cn

Ruby: s.split(",");  s.split
来源：http://la.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gv.szsharing.cn

[E08] 数组按分隔符合并
来源：http://pv.shxzukj.cn

Py:   ",".join(items)
来源：http://sk.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://nv.szsharing.cn

JS:   items.join(",")
来源：http://ps.asd995.cn

TS:   items.join(",")
来源：http://dk.hnjuh.cn

Java: String.join(",", items)
来源：http://ya.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://xx.9csxet.cn

Ruby: items.join(",")
来源：http://so.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://kk.panjiajie.cn

[E09] 去除所有空白字符
来源：http://dd.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fv.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jq.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://ng.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://rd.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://xm.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kp.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fc.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ub.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://qa.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cs.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jo.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://dy.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://il.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://hb.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jw.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hr.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tm.huixinmuqiang.cn

[E11] 反转字符串
来源：http://lz.shxzukj.cn

Py:   s[::-1]
来源：http://bx.asd995.cn

PHP:  strrev($s);
来源：http://nb.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://ia.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://cm.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xm.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gt.hnjuh.cn

Ruby: s.reverse
来源：http://np.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://um.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://mk.bjjhwx.cn

Py:   s.count("a")
来源：http://tp.521024.cn

PHP:  substr_count($s, "a");
来源：http://jf.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://xc.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://tg.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sk.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://sq.newstarts.cn

Ruby: s.count("a")
来源：http://gw.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://hr.colortex.cn

[E13] 逐字符遍历
来源：http://vn.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://pl.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lc.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lk.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://co.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pk.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xs.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://no.huanxung.cn

[E14] URL 编码与 Base64
来源：http://nd.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rm.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://st.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ui.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wh.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kn.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ly.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iz.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bb.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://kt.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://px.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dv.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nz.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://io.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jk.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bm.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tj.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bl.hnjuh.cn

[E16] 数字千分位
来源：http://zu.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://cr.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ab.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zk.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tn.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hr.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ho.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qh.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://af.newstarts.cn

[E17] 首字母大写
来源：http://aa.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ti.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ex.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xv.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zs.szxytkj.cn

Ruby: s.capitalize
来源：http://he.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ay.gzmigu.cn

[E18] 模板占位符替换
来源：http://ua.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kv.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sb.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xg.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ih.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qc.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qd.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ec.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pj.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://lv.shtwfgs.cn

Py:   s.splitlines()
来源：http://do.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eh.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://dw.521024.cn

TS:   s.split(/\r?\n/)
来源：http://jg.shxzukj.cn

Java: s.lines().toList()
来源：http://hz.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://kt.hahajie.cn

Ruby: s.lines
来源：http://uh.nszjky.cn

C#:   s.Split('\n')
来源：http://qk.asd995.cn

[E20] 判断字符串是否为空
来源：http://ly.9csxet.cn

Py:   if not s:
来源：http://ah.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rm.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jb.newstarts.cn

TS:   if (s === "") {}
来源：http://ij.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://fc.asd995.cn

Go:   if s == "" {}
来源：http://wf.newstarts.cn

Ruby: if s.empty?
来源：http://hj.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wo.nszjky.cn

[E21] 超长截断加省略号
来源：http://ze.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gk.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pl.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ue.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ev.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bd.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://lx.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ko.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tz.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://hm.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qs.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jr.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eq.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://om.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gj.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://pb.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qf.panjiajie.cn

================================================================================
来源：http://uz.szxytkj.cn

F. 文件与目录
来源：http://jz.yuntaijiaju.cn

================================================================================
来源：http://it.jctech888.com.cn

[F01] 读取整个文件
来源：http://sc.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zf.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yz.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zj.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bb.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xe.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ui.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ew.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://hi.hahajie.cn

[F02] 逐行读取文件
来源：http://jk.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fd.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rh.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zy.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zf.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sx.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xy.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ry.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tv.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://ek.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nb.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ip.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oc.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yq.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lf.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://de.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://fv.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ri.gzmigu.cn

[F04] 追加写入文件
来源：http://ou.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pe.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nd.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rz.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wk.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jd.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cr.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mb.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gm.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://ef.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://no.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://io.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://eo.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://kr.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eg.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jz.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://pi.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://do.huixinmuqiang.cn

[F06] 删除文件
来源：http://qv.newstarts.cn

Py:   os.remove("a.txt")
来源：http://bb.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ei.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rs.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pg.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gx.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://vj.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ae.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://uq.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://de.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kp.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ah.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mq.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cy.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sx.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sb.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xi.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ul.bjjhwx.cn

[F08] 遍历目录
来源：http://sn.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ji.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ul.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://mn.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://lg.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zz.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ue.hahajie.cn

Ruby: Dir.children("dir")
来源：http://zf.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ii.bookmarksfly.cn

[F09] 获取文件大小
来源：http://mb.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://zl.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://fi.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ra.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://zw.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pl.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tm.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://fk.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://fb.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://be.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ey.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sh.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://np.asd995.cn

TS:   path.extname("a.txt")
来源：http://ey.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bj.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ee.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xb.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ik.huixiangedu.cn

[F11] 复制与移动文件
来源：http://ge.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lv.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bb.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hk.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nf.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xo.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bs.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://px.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ax.jianghongdianzi.cn

[F12] CSV 读写
来源：http://pj.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oi.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xi.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rz.bookmarksfly.cn

TS:   // 同上
来源：http://cm.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xo.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mk.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pv.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bx.haigaiapp.cn

================================================================================
来源：http://gz.hnjuh.cn

G. 面向对象
来源：http://jb.panjiajie.cn

================================================================================
来源：http://ph.asd995.cn

[G01] 定义类
来源：http://qs.wgjwhj.cn

Py:   class User: pass
来源：http://qq.jctech888.com.cn

PHP:  class User {}
来源：http://be.panjiajie.cn

JS:   class User {}
来源：http://yp.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://sx.lnxyls.cn

Java: class User {}
来源：http://jz.asd995.cn

Go:   type User struct { Name string }
来源：http://rw.lnxyls.cn

Ruby: class User; end
来源：http://qj.9csxet.cn

C#:   class User {}
来源：http://ua.bjjhwx.cn


<!-- 参考信息 -->