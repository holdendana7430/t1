代发 wailian999

PHP:  strpos($s, "x");
来源：http://hc.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ub.hnjuh.cn

TS:   s.indexOf("x")
来源：http://xm.hahajie.cn

Java: s.indexOf("x")
来源：http://bs.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://gl.huixiangedu.cn

Ruby: s.index("x")
来源：http://jn.nszjky.cn

C#:   s.IndexOf("x")
来源：http://qp.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ll.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bd.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mb.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://my.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qr.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nk.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ge.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sq.nicolike.cn

[E06] 替换子串
来源：http://pc.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://or.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://pf.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://na.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oj.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vb.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ff.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://di.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ez.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ip.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mw.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oa.huanxung.cn

TS:   s.split(",")
来源：http://el.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xw.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ix.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://qi.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dd.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://wf.nszjky.cn

Py:   ",".join(items)
来源：http://pm.hnjuh.cn

PHP:  implode(",", $items);
来源：http://ki.hahajie.cn

JS:   items.join(",")
来源：http://pe.haigaiapp.cn

TS:   items.join(",")
来源：http://ah.szsharing.cn

Java: String.join(",", items)
来源：http://at.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ba.wgjwhj.cn

Ruby: items.join(",")
来源：http://iw.shxzukj.cn

C#:   string.Join(",", items)
来源：http://qb.shxzskj.cn

[E09] 去除所有空白字符
来源：http://kr.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ca.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yo.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://rx.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://ad.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://hx.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xa.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vm.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hx.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://np.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eo.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rc.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://lj.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://vo.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://tp.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mw.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ob.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wc.shxzukj.cn

[E11] 反转字符串
来源：http://mp.asd995.cn

Py:   s[::-1]
来源：http://ag.bookmarksfly.cn

PHP:  strrev($s);
来源：http://bh.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://pn.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://xv.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wz.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rd.shxzukj.cn

Ruby: s.reverse
来源：http://ag.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ns.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ix.haigaiapp.cn

Py:   s.count("a")
来源：http://pc.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://da.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://qb.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://dn.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fm.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://bd.muxihuayi.cn

Ruby: s.count("a")
来源：http://gu.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://jx.huanxung.cn

[E13] 逐字符遍历
来源：http://bo.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://iw.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xj.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kr.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ww.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://te.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tg.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ba.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ve.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://de.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lp.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ct.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ve.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pp.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://to.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ss.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gi.521024.cn

[E15] HTML 转义 / 反转义
来源：http://ub.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kk.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rm.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nz.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qw.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gg.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qv.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://up.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jy.jianghongdianzi.cn

[E16] 数字千分位
来源：http://uy.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://xq.521024.cn

PHP:  number_format(1234567);
来源：http://ua.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mi.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sz.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wg.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uy.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://du.521024.cn

C#:   1234567.ToString("N0")
来源：http://us.szxytkj.cn

[E17] 首字母大写
来源：http://nr.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nr.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tt.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://so.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xm.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mn.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://co.jctech888.com.cn

Ruby: s.capitalize
来源：http://cy.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kv.newstarts.cn

[E18] 模板占位符替换
来源：http://cp.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sl.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pc.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uk.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://do.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rn.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://so.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cu.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mf.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://xf.shxzskj.cn

Py:   s.splitlines()
来源：http://yw.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ul.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://ac.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ok.gzmigu.cn

Java: s.lines().toList()
来源：http://ux.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://gl.jianghongdianzi.cn

Ruby: s.lines
来源：http://sq.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ia.9csxet.cn

[E20] 判断字符串是否为空
来源：http://yi.huixiangedu.cn

Py:   if not s:
来源：http://pw.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://az.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tb.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://ua.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://wu.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://ur.colortex.cn

Ruby: if s.empty?
来源：http://mu.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://om.nicolike.cn

[E21] 超长截断加省略号
来源：http://md.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ql.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://il.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hk.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zq.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bk.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://qx.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://to.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kg.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://iq.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vw.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oe.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tt.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nt.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hp.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qy.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ix.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xq.shxzskj.cn

================================================================================
来源：http://lu.gzmigu.cn

F. 文件与目录
来源：http://fu.nicolike.cn

================================================================================
来源：http://hj.colortex.cn

[F01] 读取整个文件
来源：http://di.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mo.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://mp.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qb.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bj.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rj.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://di.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://nh.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://de.nicolike.cn

[F02] 逐行读取文件
来源：http://xw.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://am.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yz.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mp.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pz.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bw.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://um.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pi.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eh.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ni.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rc.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mf.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yj.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://at.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cw.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ey.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ge.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rs.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://cv.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ci.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qq.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://se.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hi.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zk.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bf.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bi.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://nj.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ht.asd995.cn

PHP:  file_exists("a.txt");
来源：http://mw.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://rf.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://ki.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://di.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nz.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ht.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://xm.nicolike.cn

[F06] 删除文件
来源：http://cu.szsharing.cn

Py:   os.remove("a.txt")
来源：http://dv.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://nl.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vt.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vv.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mk.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://zw.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://vf.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://fq.szsharing.cn

[F07] 创建目录（含多级）
来源：http://jp.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rb.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tc.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rm.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://al.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://co.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mm.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ar.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bf.shtwfgs.cn

[F08] 遍历目录
来源：http://li.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vi.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iz.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://xw.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://ml.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rc.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ga.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://vz.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://gp.muxihuayi.cn

[F09] 获取文件大小
来源：http://mc.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://dc.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ae.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://ok.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://nb.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nw.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nt.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://uj.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://dx.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://vr.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://py.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bk.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://to.9csxet.cn

TS:   path.extname("a.txt")
来源：http://ye.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ct.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kn.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gl.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tl.9csxet.cn

[F11] 复制与移动文件
来源：http://ht.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sy.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zz.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://es.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ax.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pd.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fi.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://im.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ie.shtwfgs.cn

[F12] CSV 读写
来源：http://vc.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ve.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tz.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kg.yuntaijiaju.cn

TS:   // 同上
来源：http://aj.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://if.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qm.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jv.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ql.haigaiapp.cn

================================================================================
来源：http://ln.hahajie.cn

G. 面向对象
来源：http://jp.jctech888.com.cn

================================================================================
来源：http://yy.hahajie.cn

[G01] 定义类
来源：http://cu.muxihuayi.cn

Py:   class User: pass
来源：http://kr.newstarts.cn

PHP:  class User {}
来源：http://li.bjjhwx.cn

JS:   class User {}
来源：http://os.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://uk.jianghongdianzi.cn

Java: class User {}
来源：http://te.9csxet.cn

Go:   type User struct { Name string }
来源：http://uj.jctech888.com.cn

Ruby: class User; end
来源：http://sh.szxytkj.cn

C#:   class User {}
来源：http://st.gzmigu.cn

[G02] 构造函数
来源：http://yk.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://dt.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://rq.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ra.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ka.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ty.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ir.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://kn.nszjky.cn


<!-- 参考信息 -->