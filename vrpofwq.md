代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vr.newstarts.cn

[E03] 截取子串
来源：http://mj.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jv.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wf.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yk.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://tm.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://ez.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ib.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ws.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ze.hahajie.cn

[E04] 查找子串位置
来源：http://th.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://jq.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://os.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uw.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ob.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ps.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://le.9csxet.cn

Ruby: s.index("x")
来源：http://gq.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://pb.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vl.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ab.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hr.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cu.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mq.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://me.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gf.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lh.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ri.bjjhwx.cn

[E06] 替换子串
来源：http://bt.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://to.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://yw.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ld.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://gm.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vy.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://di.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pq.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://mg.521024.cn

[E07] 按分隔符拆分
来源：http://pl.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dy.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://be.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://do.yuntaijiaju.cn

TS:   s.split(",")
来源：http://vj.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uc.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://av.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://bn.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zw.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ek.wgjwhj.cn

Py:   ",".join(items)
来源：http://vg.newstarts.cn

PHP:  implode(",", $items);
来源：http://ll.shtwfgs.cn

JS:   items.join(",")
来源：http://lq.9csxet.cn

TS:   items.join(",")
来源：http://kz.chemitech.net.cn

Java: String.join(",", items)
来源：http://yt.colortex.cn

Go:   strings.Join(items, ",")
来源：http://kd.chemitech.net.cn

Ruby: items.join(",")
来源：http://oy.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://cm.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://xb.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zx.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ac.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fq.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ls.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://uu.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://np.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zt.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wc.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://jd.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dt.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fx.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://id.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://dy.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://vf.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://td.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bf.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vr.huanxung.cn

[E11] 反转字符串
来源：http://ii.shtwfgs.cn

Py:   s[::-1]
来源：http://dn.shxzukj.cn

PHP:  strrev($s);
来源：http://qr.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://yv.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://kk.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vh.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nt.huixiangedu.cn

Ruby: s.reverse
来源：http://tb.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yk.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ud.yuexingan06.cn

Py:   s.count("a")
来源：http://yu.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://sd.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://cz.9csxet.cn

TS:   s.split("a").length - 1
来源：http://sn.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lw.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://ha.asd995.cn

Ruby: s.count("a")
来源：http://kn.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://lo.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://ne.colortex.cn

Py:   for ch in s: print(ch)
来源：http://hm.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eb.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://li.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eo.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mg.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ru.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hr.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://if.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://rr.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ag.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ql.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cm.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lr.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ju.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sd.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wx.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gw.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://wg.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://un.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ou.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bo.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rr.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zo.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tf.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ni.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ku.jianghongdianzi.cn

[E16] 数字千分位
来源：http://lk.colortex.cn

Py:   f"{1234567:,}"
来源：http://qc.colortex.cn

PHP:  number_format(1234567);
来源：http://ws.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zl.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fw.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rw.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vp.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lz.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://nh.9csxet.cn

[E17] 首字母大写
来源：http://fz.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://de.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ut.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kh.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kw.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nf.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sx.lnxyls.cn

Ruby: s.capitalize
来源：http://jb.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ez.wgjwhj.cn

[E18] 模板占位符替换
来源：http://uq.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nz.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bl.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://so.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tb.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wf.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ae.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wh.huanxung.cn

[E19] 多行文本按行拆分
来源：http://sc.szsharing.cn

Py:   s.splitlines()
来源：http://bz.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xi.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ei.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://sn.shxzukj.cn

Java: s.lines().toList()
来源：http://xn.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://im.lnxyls.cn

Ruby: s.lines
来源：http://fm.szxytkj.cn

C#:   s.Split('\n')
来源：http://ho.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://ou.521024.cn

Py:   if not s:
来源：http://eb.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hl.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nu.asd995.cn

TS:   if (s === "") {}
来源：http://fe.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://pi.panjiajie.cn

Go:   if s == "" {}
来源：http://dx.gzmigu.cn

Ruby: if s.empty?
来源：http://kx.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pp.gzmigu.cn

[E21] 超长截断加省略号
来源：http://jk.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ao.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ee.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dm.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dg.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dl.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://xz.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qk.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jc.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://ts.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lc.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ft.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ws.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zz.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ha.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qe.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ia.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qp.haigaiapp.cn

================================================================================
来源：http://oq.shxzskj.cn

F. 文件与目录
来源：http://hw.jctech888.com.cn

================================================================================
来源：http://zg.newstarts.cn

[F01] 读取整个文件
来源：http://ty.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qx.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://gh.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rd.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tw.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xi.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nl.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://ap.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://je.colortex.cn

[F02] 逐行读取文件
来源：http://ei.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://it.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fz.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ye.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dp.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hv.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://md.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cy.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ug.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://cy.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uz.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aw.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oh.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yz.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fg.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fk.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://tw.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fo.haigaiapp.cn

[F04] 追加写入文件
来源：http://qu.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eq.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uh.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://no.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://be.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qm.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gh.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pi.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://za.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://kr.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dw.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ri.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://qf.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://th.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ln.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zf.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://kb.521024.cn

C#:   File.Exists("a.txt")
来源：http://va.nszjky.cn

[F06] 删除文件
来源：http://bc.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://fa.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://rh.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gk.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wv.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hb.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://sn.colortex.cn

Ruby: File.delete("a.txt")
来源：http://fm.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://cc.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://tl.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ga.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cp.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gl.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gv.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yr.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nl.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xh.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://px.huixinmuqiang.cn

[F08] 遍历目录
来源：http://fy.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zj.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tb.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://si.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://be.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ps.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ia.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://kg.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://mc.asd995.cn

[F09] 获取文件大小
来源：http://cy.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://lv.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://ci.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://pl.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://hs.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kl.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jp.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://ix.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://ne.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://wf.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wh.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vt.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vm.nszjky.cn

TS:   path.extname("a.txt")
来源：http://em.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eh.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ub.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bs.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ei.521024.cn

[F11] 复制与移动文件
来源：http://fb.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fo.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rr.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://em.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oy.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ar.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oz.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xx.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ak.shxzukj.cn

[F12] CSV 读写
来源：http://it.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wo.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ac.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jl.yuexingan06.cn

TS:   // 同上
来源：http://rx.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jk.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zz.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oq.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lu.shxzukj.cn

================================================================================
来源：http://iz.panjiajie.cn

G. 面向对象
来源：http://rv.lnxyls.cn

================================================================================
来源：http://ti.panjiajie.cn

[G01] 定义类
来源：http://da.panjiajie.cn

Py:   class User: pass
来源：http://yr.szxytkj.cn

PHP:  class User {}
来源：http://ez.jctech888.com.cn

JS:   class User {}
来源：http://pn.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://oy.gzmigu.cn


<!-- 参考信息 -->