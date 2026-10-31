代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://wy.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://gu.szxytkj.cn

[E04] 查找子串位置
来源：http://wo.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://hk.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ld.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ps.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://kv.gzmigu.cn

Java: s.indexOf("x")
来源：http://fr.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://uj.haigaiapp.cn

Ruby: s.index("x")
来源：http://az.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ps.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qi.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ug.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ai.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dl.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rg.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cp.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ci.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ia.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pm.wgjwhj.cn

[E06] 替换子串
来源：http://cx.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ym.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://pr.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nw.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://jg.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://is.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rs.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ew.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://ks.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://bu.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ol.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wj.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kv.haigaiapp.cn

TS:   s.split(",")
来源：http://iz.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eo.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xn.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://le.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qt.521024.cn

[E08] 数组按分隔符合并
来源：http://ck.hahajie.cn

Py:   ",".join(items)
来源：http://qv.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://oc.haigaiapp.cn

JS:   items.join(",")
来源：http://zm.shtwfgs.cn

TS:   items.join(",")
来源：http://yc.szsharing.cn

Java: String.join(",", items)
来源：http://sc.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://jr.nszjky.cn

Ruby: items.join(",")
来源：http://rl.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://hu.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://kq.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ab.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ic.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://ln.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://jc.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://mn.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pb.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dd.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ld.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://ac.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gk.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ev.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://vk.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://by.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://qe.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bt.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vo.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ik.panjiajie.cn

[E11] 反转字符串
来源：http://jx.muxihuayi.cn

Py:   s[::-1]
来源：http://yr.hnjuh.cn

PHP:  strrev($s);
来源：http://ed.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://hn.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://mh.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://el.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pg.newstarts.cn

Ruby: s.reverse
来源：http://lj.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ho.nszjky.cn

[E12] 统计某字符出现次数
来源：http://jv.hahajie.cn

Py:   s.count("a")
来源：http://iw.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://ng.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://kv.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ex.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ew.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://dr.muxihuayi.cn

Ruby: s.count("a")
来源：http://zm.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://fq.panjiajie.cn

[E13] 逐字符遍历
来源：http://mw.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://cm.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oz.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fi.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ed.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gt.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vq.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://em.hahajie.cn

[E14] URL 编码与 Base64
来源：http://as.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yp.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sf.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sb.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ak.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ze.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jd.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cd.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pe.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://pn.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kz.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ta.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ow.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dl.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bv.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ta.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hn.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xy.shxzskj.cn

[E16] 数字千分位
来源：http://fd.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://qw.shxzskj.cn

PHP:  number_format(1234567);
来源：http://ve.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dc.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://op.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rx.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jd.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gv.asd995.cn

C#:   1234567.ToString("N0")
来源：http://df.jctech888.com.cn

[E17] 首字母大写
来源：http://cm.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ho.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://by.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iu.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xl.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iv.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://or.newstarts.cn

Ruby: s.capitalize
来源：http://av.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://br.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://iq.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mo.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kt.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rl.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vi.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vd.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://un.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gd.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yf.9csxet.cn

[E19] 多行文本按行拆分
来源：http://ve.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://rz.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dz.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://bb.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://zz.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://pl.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://mx.colortex.cn

Ruby: s.lines
来源：http://aq.yuexingan06.cn

C#:   s.Split('\n')
来源：http://yp.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://cj.gzmigu.cn

Py:   if not s:
来源：http://uh.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ys.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ac.panjiajie.cn

TS:   if (s === "") {}
来源：http://eq.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ep.szxytkj.cn

Go:   if s == "" {}
来源：http://uz.szsharing.cn

Ruby: if s.empty?
来源：http://vn.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cl.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://ts.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xh.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zp.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rw.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eq.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ad.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://fy.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://no.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gc.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://kz.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tt.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kx.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kd.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pb.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bg.521024.cn

Ruby: s.bytesize;  s.length
来源：http://mh.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ja.bookmarksfly.cn

================================================================================
来源：http://ek.huanxung.cn

F. 文件与目录
来源：http://xu.haigaiapp.cn

================================================================================
来源：http://wj.nszjky.cn

[F01] 读取整个文件
来源：http://ke.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dj.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://az.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vk.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dn.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xp.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ji.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://qw.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ql.hahajie.cn

[F02] 逐行读取文件
来源：http://og.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nq.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ai.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rk.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qs.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pg.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oz.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oh.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rg.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://rb.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xv.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cq.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ff.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ka.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://si.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://lx.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pl.shxzskj.cn

[F04] 追加写入文件
来源：http://xx.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uu.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nr.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oo.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yd.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://br.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vo.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hl.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ly.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://xa.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ux.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://sv.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://ja.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://dl.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://at.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qc.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://wn.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://cg.szxytkj.cn

[F06] 删除文件
来源：http://rc.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://dm.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://xl.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tp.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aq.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://la.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://rn.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://my.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://zn.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://sr.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://en.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tl.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zj.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xn.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wy.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ky.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rn.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cf.yuntaijiaju.cn

[F08] 遍历目录
来源：http://ba.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eh.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://te.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://of.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://bd.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qz.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pz.nszjky.cn

Ruby: Dir.children("dir")
来源：http://ov.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://zp.nicolike.cn

[F09] 获取文件大小
来源：http://lu.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://lw.szsharing.cn

PHP:  filesize("a.txt");
来源：http://qj.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://qv.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://fd.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oo.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://su.colortex.cn

Ruby: File.size("a.txt")
来源：http://os.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://gu.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://yz.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cd.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fv.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xe.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://pt.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ng.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yw.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vx.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sc.gzmigu.cn

[F11] 复制与移动文件
来源：http://ef.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qu.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://la.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gb.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pq.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wp.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pj.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qs.nszjky.cn

[F12] CSV 读写
来源：http://xd.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nj.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fg.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ez.bookmarksfly.cn

TS:   // 同上
来源：http://aq.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ig.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cu.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qj.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ss.shxzukj.cn

================================================================================
来源：http://od.chemitech.net.cn

G. 面向对象
来源：http://zo.bookmarksfly.cn

================================================================================
来源：http://hx.lnxyls.cn

[G01] 定义类
来源：http://yq.gzmigu.cn

Py:   class User: pass
来源：http://rb.nicolike.cn

PHP:  class User {}
来源：http://lr.huanxung.cn

JS:   class User {}
来源：http://qe.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://qs.huixiangedu.cn

Java: class User {}
来源：http://jg.panjiajie.cn

Go:   type User struct { Name string }
来源：http://yv.muxihuayi.cn

Ruby: class User; end
来源：http://fi.asd995.cn

C#:   class User {}
来源：http://zh.newstarts.cn

[G02] 构造函数
来源：http://jj.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://gk.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://fy.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://tq.nszjky.cn


<!-- 参考信息 -->