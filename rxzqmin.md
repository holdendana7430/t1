代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xb.9csxet.cn

TS:   s.slice(1, 4)
来源：http://cy.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://kb.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ys.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pz.521024.cn

C#:   s.Substring(1, 3)
来源：http://du.huanxung.cn

[E04] 查找子串位置
来源：http://bz.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://kc.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://hb.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cy.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://qa.jctech888.com.cn

Java: s.indexOf("x")
来源：http://yf.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://uz.shtwfgs.cn

Ruby: s.index("x")
来源：http://lz.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://mi.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oc.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oe.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fg.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://la.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xu.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yf.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ie.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zv.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ji.huanxung.cn

[E06] 替换子串
来源：http://mt.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pc.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://su.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://el.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://zk.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://or.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xw.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pb.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://iy.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ut.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://th.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oj.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zf.shxzskj.cn

TS:   s.split(",")
来源：http://rc.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zj.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dn.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://lp.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://no.hahajie.cn

[E08] 数组按分隔符合并
来源：http://dx.nszjky.cn

Py:   ",".join(items)
来源：http://iw.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://ml.newstarts.cn

JS:   items.join(",")
来源：http://ks.lnxyls.cn

TS:   items.join(",")
来源：http://tc.shxzukj.cn

Java: String.join(",", items)
来源：http://fu.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://yy.colortex.cn

Ruby: items.join(",")
来源：http://bs.gzmigu.cn

C#:   string.Join(",", items)
来源：http://cr.newstarts.cn

[E09] 去除所有空白字符
来源：http://dn.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://no.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yk.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://ao.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://de.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://yl.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pq.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ob.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pn.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://nd.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mf.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ui.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://bz.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://mo.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://vb.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hq.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ly.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ye.chemitech.net.cn

[E11] 反转字符串
来源：http://ue.haigaiapp.cn

Py:   s[::-1]
来源：http://ce.szsharing.cn

PHP:  strrev($s);
来源：http://st.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://nd.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://uj.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bv.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nt.nszjky.cn

Ruby: s.reverse
来源：http://ml.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vf.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://ob.shtwfgs.cn

Py:   s.count("a")
来源：http://bo.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://di.asd995.cn

JS:   s.split("a").length - 1
来源：http://en.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://ta.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yx.asd995.cn

Go:   strings.Count(s, "a")
来源：http://jn.bjjhwx.cn

Ruby: s.count("a")
来源：http://vw.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://eg.huanxung.cn

[E13] 逐字符遍历
来源：http://iw.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://zs.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qu.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yo.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xx.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wq.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://me.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yr.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ii.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://vr.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://la.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sv.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eg.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rj.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ct.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ub.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uu.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gh.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://bo.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ll.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tl.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ts.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nd.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ya.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://th.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ov.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qb.lnxyls.cn

[E16] 数字千分位
来源：http://nb.colortex.cn

Py:   f"{1234567:,}"
来源：http://iv.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://ke.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kg.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fz.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qb.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zk.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ez.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://jj.nicolike.cn

[E17] 首字母大写
来源：http://cr.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cj.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qr.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ce.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iz.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eg.gzmigu.cn

Ruby: s.capitalize
来源：http://tv.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jh.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://cj.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://av.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lh.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lh.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://us.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ix.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dp.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wg.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sm.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://vn.szsharing.cn

Py:   s.splitlines()
来源：http://aa.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://to.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://hr.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://hm.shxzskj.cn

Java: s.lines().toList()
来源：http://li.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://ca.huanxung.cn

Ruby: s.lines
来源：http://jz.colortex.cn

C#:   s.Split('\n')
来源：http://qy.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://ge.jctech888.com.cn

Py:   if not s:
来源：http://uv.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vj.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oz.shtwfgs.cn

TS:   if (s === "") {}
来源：http://rr.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://wb.szsharing.cn

Go:   if s == "" {}
来源：http://ci.colortex.cn

Ruby: if s.empty?
来源：http://hq.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lz.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://fo.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tg.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dm.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uj.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cm.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://by.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://vj.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uw.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://je.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://mq.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qk.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://av.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://my.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hq.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uc.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://ea.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yh.huixiangedu.cn

================================================================================
来源：http://zv.huanxung.cn

F. 文件与目录
来源：http://jv.bjjhwx.cn

================================================================================
来源：http://ob.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://mp.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://un.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://cl.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dx.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vy.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lu.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ql.nicolike.cn

Ruby: File.read("a.txt")
来源：http://tw.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://fg.newstarts.cn

[F02] 逐行读取文件
来源：http://pt.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vh.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ob.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vc.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uc.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://js.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ga.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ct.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://sk.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ys.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vs.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sq.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pb.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ap.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rm.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://yh.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lb.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://yp.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yo.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xv.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sp.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hh.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gd.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ed.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yv.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://hz.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ox.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://iy.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://yr.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://bo.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zs.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tv.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://pq.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://or.szxytkj.cn

[F06] 删除文件
来源：http://uq.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://zs.newstarts.cn

PHP:  unlink("a.txt");
来源：http://xb.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ag.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ps.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cf.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://ng.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://oa.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://dq.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://jv.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://py.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qp.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oc.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aw.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://te.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hg.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vp.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zx.asd995.cn

[F08] 遍历目录
来源：http://tx.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ar.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lq.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://hz.521024.cn

TS:   fs.readdirSync("dir")
来源：http://gy.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tx.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://la.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://bo.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://bo.shxzskj.cn

[F09] 获取文件大小
来源：http://ev.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://bm.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://uy.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://bz.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://pz.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ow.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ld.521024.cn

Ruby: File.size("a.txt")
来源：http://tt.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qf.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://mk.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://py.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ek.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fz.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://te.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://to.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tl.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fq.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xc.yuexingan06.cn

[F11] 复制与移动文件
来源：http://zl.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mb.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jt.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ee.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ej.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qi.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mr.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zi.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wf.jianghongdianzi.cn

[F12] CSV 读写
来源：http://bn.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nu.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wz.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ov.hahajie.cn

TS:   // 同上
来源：http://fy.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jt.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sa.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://my.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ab.shxzskj.cn

================================================================================
来源：http://xp.nicolike.cn

G. 面向对象
来源：http://hd.chemitech.net.cn

================================================================================
来源：http://ac.haigaiapp.cn

[G01] 定义类
来源：http://ok.521024.cn

Py:   class User: pass
来源：http://bn.nicolike.cn

PHP:  class User {}
来源：http://jo.haigaiapp.cn

JS:   class User {}
来源：http://dk.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://qi.huanxung.cn

Java: class User {}
来源：http://cd.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://qt.colortex.cn

Ruby: class User; end
来源：http://sz.shtwfgs.cn

C#:   class User {}
来源：http://ca.huixinmuqiang.cn


<!-- 参考信息 -->