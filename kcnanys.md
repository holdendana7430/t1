代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ak.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://pg.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://qg.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ca.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oc.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://uy.szsharing.cn

[E04] 查找子串位置
来源：http://de.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://tz.szsharing.cn

PHP:  strpos($s, "x");
来源：http://kp.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://js.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://sr.nszjky.cn

Java: s.indexOf("x")
来源：http://ig.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://vp.shtwfgs.cn

Ruby: s.index("x")
来源：http://qr.nicolike.cn

C#:   s.IndexOf("x")
来源：http://jq.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ip.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ad.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wu.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sb.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iz.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xs.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://se.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fh.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cp.hnjuh.cn

[E06] 替换子串
来源：http://us.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://on.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://vl.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sc.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://ve.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zy.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ed.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ej.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://qn.hahajie.cn

[E07] 按分隔符拆分
来源：http://ho.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ml.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rw.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://do.521024.cn

TS:   s.split(",")
来源：http://rl.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zo.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mc.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ch.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dl.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://hu.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://zq.hnjuh.cn

PHP:  implode(",", $items);
来源：http://ey.shxzukj.cn

JS:   items.join(",")
来源：http://oz.wgjwhj.cn

TS:   items.join(",")
来源：http://di.nicolike.cn

Java: String.join(",", items)
来源：http://qu.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://zk.521024.cn

Ruby: items.join(",")
来源：http://jx.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://cy.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://uc.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fl.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zp.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://ky.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ys.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://nn.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tk.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wg.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iq.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://pd.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kh.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xc.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://dh.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://zg.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://sm.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wg.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pm.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yq.hnjuh.cn

[E11] 反转字符串
来源：http://au.shxzskj.cn

Py:   s[::-1]
来源：http://jr.hnjuh.cn

PHP:  strrev($s);
来源：http://ak.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ss.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://hy.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ry.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ex.colortex.cn

Ruby: s.reverse
来源：http://tb.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xl.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://uf.chemitech.net.cn

Py:   s.count("a")
来源：http://hj.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://bs.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://ou.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://qk.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dd.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://tv.yuexingan06.cn

Ruby: s.count("a")
来源：http://ya.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://qc.shxzskj.cn

[E13] 逐字符遍历
来源：http://cq.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://ae.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aa.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://me.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dl.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xs.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mh.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tm.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ie.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://fm.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iq.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aq.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ch.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tg.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://my.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xx.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yk.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ha.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://qi.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qv.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jk.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dw.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xa.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hu.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ah.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jy.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lq.szsharing.cn

[E16] 数字千分位
来源：http://mq.newstarts.cn

Py:   f"{1234567:,}"
来源：http://nf.nszjky.cn

PHP:  number_format(1234567);
来源：http://gq.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uo.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zz.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vv.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ct.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tl.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://lk.521024.cn

[E17] 首字母大写
来源：http://wu.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://se.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tx.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oq.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ir.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ci.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ww.jctech888.com.cn

Ruby: s.capitalize
来源：http://ux.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://is.shxzskj.cn

[E18] 模板占位符替换
来源：http://fc.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pq.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yd.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xc.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ob.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://py.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zz.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yj.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yk.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://qo.szxytkj.cn

Py:   s.splitlines()
来源：http://be.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gt.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://qo.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://ly.chemitech.net.cn

Java: s.lines().toList()
来源：http://pn.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://uf.colortex.cn

Ruby: s.lines
来源：http://bn.huanxung.cn

C#:   s.Split('\n')
来源：http://jw.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://ue.shtwfgs.cn

Py:   if not s:
来源：http://nw.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ts.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wm.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://by.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://uc.shxzukj.cn

Go:   if s == "" {}
来源：http://hw.colortex.cn

Ruby: if s.empty?
来源：http://ok.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zz.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://aq.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gh.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mi.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ac.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jj.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://az.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ws.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gx.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://pr.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lh.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tg.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ww.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lq.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qt.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://wz.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://te.colortex.cn

================================================================================
来源：http://bv.yuexingan06.cn

F. 文件与目录
来源：http://bg.panjiajie.cn

================================================================================
来源：http://ku.9csxet.cn

[F01] 读取整个文件
来源：http://dr.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fu.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://ut.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wp.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pl.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sb.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vk.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://yy.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://hd.shtwfgs.cn

[F02] 逐行读取文件
来源：http://gi.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fq.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fi.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uq.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pq.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sx.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ga.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ff.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://up.asd995.cn

[F03] 写入文件（覆盖）
来源：http://wl.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vf.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mm.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://td.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yo.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kj.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://je.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://vu.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sb.asd995.cn

[F04] 追加写入文件
来源：http://rj.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ww.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gf.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gm.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xm.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bv.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://le.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zl.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ad.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://al.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://hl.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://wj.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://yg.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fd.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kp.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://cl.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://rt.wgjwhj.cn

[F06] 删除文件
来源：http://mj.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://uu.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://rq.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uj.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lu.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jw.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ug.asd995.cn

Ruby: File.delete("a.txt")
来源：http://za.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://rz.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://ng.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wk.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nf.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pw.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sq.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aa.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nq.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iv.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gr.szxytkj.cn

[F08] 遍历目录
来源：http://wx.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wu.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cz.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://lp.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://yk.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yr.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vi.szsharing.cn

Ruby: Dir.children("dir")
来源：http://sl.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://fl.szsharing.cn

[F09] 获取文件大小
来源：http://mr.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://uq.asd995.cn

PHP:  filesize("a.txt");
来源：http://fc.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://hm.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://zo.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mf.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gl.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://mu.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://zd.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://op.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fu.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pq.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tb.huanxung.cn

TS:   path.extname("a.txt")
来源：http://al.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wg.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ev.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zf.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jo.newstarts.cn

[F11] 复制与移动文件
来源：http://xz.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nh.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ac.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lj.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wc.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ol.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pl.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wq.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hi.hahajie.cn

[F12] CSV 读写
来源：http://yg.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://my.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://et.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yj.jianghongdianzi.cn

TS:   // 同上
来源：http://va.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dq.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pq.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cq.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://av.gzmigu.cn

================================================================================
来源：http://hd.shxzskj.cn

G. 面向对象
来源：http://lt.jctech888.com.cn

================================================================================
来源：http://ss.panjiajie.cn

[G01] 定义类
来源：http://zk.huixinmuqiang.cn

Py:   class User: pass
来源：http://ya.shtwfgs.cn

PHP:  class User {}
来源：http://yv.wgjwhj.cn

JS:   class User {}
来源：http://wt.asd995.cn

TS:   class User { name: string = ""; }
来源：http://mi.hahajie.cn

Java: class User {}
来源：http://zc.szsharing.cn

Go:   type User struct { Name string }
来源：http://tm.9csxet.cn

Ruby: class User; end
来源：http://rf.shxzskj.cn

C#:   class User {}
来源：http://dn.9csxet.cn


<!-- 参考信息 -->