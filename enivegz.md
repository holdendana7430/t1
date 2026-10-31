代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iw.asd995.cn

[E03] 截取子串
来源：http://kh.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uk.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ef.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uf.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://lf.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://aq.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jc.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fq.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://jf.wgjwhj.cn

[E04] 查找子串位置
来源：http://oh.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://ng.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://ux.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ik.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://mt.521024.cn

Java: s.indexOf("x")
来源：http://hs.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://nu.shtwfgs.cn

Ruby: s.index("x")
来源：http://zi.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ih.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jt.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rh.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uk.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kl.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://re.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kp.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qh.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hk.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://de.szsharing.cn

[E06] 替换子串
来源：http://ni.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://en.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://uy.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ww.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://uc.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pr.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dq.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://fy.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://lw.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ej.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hn.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fc.bookmarksfly.cn

TS:   s.split(",")
来源：http://ew.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qn.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://il.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://rm.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xi.hahajie.cn

[E08] 数组按分隔符合并
来源：http://qm.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://ny.hnjuh.cn

PHP:  implode(",", $items);
来源：http://cc.huanxung.cn

JS:   items.join(",")
来源：http://vv.nicolike.cn

TS:   items.join(",")
来源：http://zo.wgjwhj.cn

Java: String.join(",", items)
来源：http://pj.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://nx.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://eo.521024.cn

C#:   string.Join(",", items)
来源：http://kz.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://jv.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zq.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://um.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://oh.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://cw.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ec.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ll.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nc.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://al.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://vm.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mz.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yl.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ra.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://rd.nicolike.cn

Java: String.format("%03d", 7)
来源：http://su.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ut.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jj.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zf.521024.cn

[E11] 反转字符串
来源：http://br.asd995.cn

Py:   s[::-1]
来源：http://gj.panjiajie.cn

PHP:  strrev($s);
来源：http://jz.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://wo.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://xv.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dj.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ox.huixinmuqiang.cn

Ruby: s.reverse
来源：http://gs.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ko.colortex.cn

[E12] 统计某字符出现次数
来源：http://jx.hahajie.cn

Py:   s.count("a")
来源：http://pf.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://dp.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://rq.colortex.cn

TS:   s.split("a").length - 1
来源：http://so.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vy.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://uv.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://yz.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://mg.shtwfgs.cn

[E13] 逐字符遍历
来源：http://wa.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://cx.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vq.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pn.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bw.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nf.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oz.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lx.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oe.nicolike.cn

[E14] URL 编码与 Base64
来源：http://pk.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nq.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cq.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fw.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qy.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yz.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ob.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uf.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cm.521024.cn

[E15] HTML 转义 / 反转义
来源：http://az.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://el.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vy.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cq.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yn.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pe.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ba.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nw.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yw.lnxyls.cn

[E16] 数字千分位
来源：http://fu.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://vp.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://pa.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sr.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kf.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zi.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qg.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gf.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://vs.jctech888.com.cn

[E17] 首字母大写
来源：http://zx.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nh.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yu.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ev.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jk.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vv.szxytkj.cn

Ruby: s.capitalize
来源：http://yj.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xg.hnjuh.cn

[E18] 模板占位符替换
来源：http://vb.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uv.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wi.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hj.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cz.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mw.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eh.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ir.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lk.hahajie.cn

[E19] 多行文本按行拆分
来源：http://gm.jctech888.com.cn

Py:   s.splitlines()
来源：http://fe.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qr.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://km.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://jh.newstarts.cn

Java: s.lines().toList()
来源：http://up.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://lx.hahajie.cn

Ruby: s.lines
来源：http://cd.muxihuayi.cn

C#:   s.Split('\n')
来源：http://km.szsharing.cn

[E20] 判断字符串是否为空
来源：http://bn.nszjky.cn

Py:   if not s:
来源：http://xy.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iz.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gy.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://sn.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://jn.bjjhwx.cn

Go:   if s == "" {}
来源：http://tt.newstarts.cn

Ruby: if s.empty?
来源：http://lr.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yl.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://rr.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mc.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xp.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xd.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ui.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ta.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://uo.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mw.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vq.colortex.cn

[E22] 字节长度与字符长度
来源：http://wl.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kr.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ly.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tl.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wl.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mi.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://xw.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ye.colortex.cn

================================================================================
来源：http://sd.muxihuayi.cn

F. 文件与目录
来源：http://ot.gzmigu.cn

================================================================================
来源：http://fm.asd995.cn

[F01] 读取整个文件
来源：http://jd.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yn.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://mx.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wc.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bi.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cb.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bu.huanxung.cn

Ruby: File.read("a.txt")
来源：http://xd.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://sv.haigaiapp.cn

[F02] 逐行读取文件
来源：http://xe.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://km.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://se.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hm.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eu.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pj.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uz.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hk.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wd.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://fs.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mo.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lt.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ro.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dl.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ts.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zx.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ac.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tk.jctech888.com.cn

[F04] 追加写入文件
来源：http://nh.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://md.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rr.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dj.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sp.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://li.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ab.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lo.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zg.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://wn.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jd.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://nw.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://tc.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://xu.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ye.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://se.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://me.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://sx.nicolike.cn

[F06] 删除文件
来源：http://go.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://eu.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://te.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jg.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vy.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://yj.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://mv.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://aw.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://it.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ma.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gy.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hs.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ab.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ta.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ol.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fy.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pk.nicolike.cn

[F08] 遍历目录
来源：http://hs.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dm.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pw.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://hh.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://nk.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yg.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://re.nicolike.cn

Ruby: Dir.children("dir")
来源：http://xw.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://rc.521024.cn

[F09] 获取文件大小
来源：http://cq.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://df.huanxung.cn

PHP:  filesize("a.txt");
来源：http://ww.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://ik.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://gn.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pi.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fp.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://dz.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://eh.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://hx.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yq.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://om.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wa.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://vi.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iz.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://os.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ol.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gz.muxihuayi.cn

[F11] 复制与移动文件
来源：http://mh.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bt.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wf.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nw.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gb.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aa.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://md.9csxet.cn

[F12] CSV 读写
来源：http://bf.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ce.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gp.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.huixiangedu.cn

TS:   // 同上
来源：http://ge.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://id.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zj.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xk.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zy.asd995.cn

================================================================================
来源：http://fo.shxzskj.cn

G. 面向对象
来源：http://vg.shxzukj.cn

================================================================================
来源：http://jc.lnxyls.cn

[G01] 定义类
来源：http://be.9csxet.cn

Py:   class User: pass
来源：http://en.wgjwhj.cn

PHP:  class User {}
来源：http://ay.szxytkj.cn

JS:   class User {}
来源：http://bm.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ut.wgjwhj.cn


<!-- 参考信息 -->