代发 wailian999

TS:   "ab".repeat(3)
来源：http://at.nszjky.cn

Java: "ab".repeat(3)
来源：http://zd.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://dr.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://vs.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mz.shxzukj.cn

[E03] 截取子串
来源：http://vl.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aw.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kp.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mn.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://lx.huanxung.cn

Java: s.substring(1, 4)
来源：http://ge.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lg.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lv.521024.cn

C#:   s.Substring(1, 3)
来源：http://bb.colortex.cn

[E04] 查找子串位置
来源：http://cv.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://nq.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://wf.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pl.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ua.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://hq.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://ag.bookmarksfly.cn

Ruby: s.index("x")
来源：http://iz.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://eb.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hs.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mw.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mh.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mf.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yl.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nk.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gt.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qt.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lt.yuexingan06.cn

[E06] 替换子串
来源：http://wg.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ez.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://xc.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gf.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://le.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bw.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aw.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xo.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://af.szxytkj.cn

[E07] 按分隔符拆分
来源：http://qc.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qb.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wi.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ea.521024.cn

TS:   s.split(",")
来源：http://rp.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zm.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pc.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://sk.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jv.521024.cn

[E08] 数组按分隔符合并
来源：http://af.nicolike.cn

Py:   ",".join(items)
来源：http://nh.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://sv.haigaiapp.cn

JS:   items.join(",")
来源：http://af.huixiangedu.cn

TS:   items.join(",")
来源：http://ht.bjjhwx.cn

Java: String.join(",", items)
来源：http://zb.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://tn.szxytkj.cn

Ruby: items.join(",")
来源：http://qf.hnjuh.cn

C#:   string.Join(",", items)
来源：http://pi.nszjky.cn

[E09] 去除所有空白字符
来源：http://tu.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://po.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hg.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://pt.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://gi.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://so.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cw.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://or.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ep.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://ls.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://th.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wf.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://is.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://qy.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://xp.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ap.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hx.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nb.haigaiapp.cn

[E11] 反转字符串
来源：http://uy.521024.cn

Py:   s[::-1]
来源：http://uv.chemitech.net.cn

PHP:  strrev($s);
来源：http://ep.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://sx.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://nw.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jk.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wk.jctech888.com.cn

Ruby: s.reverse
来源：http://mb.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ve.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://qm.szsharing.cn

Py:   s.count("a")
来源：http://jp.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://nb.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://ka.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://hv.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hi.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://kk.szxytkj.cn

Ruby: s.count("a")
来源：http://fh.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://sz.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ts.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://em.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ew.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yy.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://he.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ap.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fm.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kb.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://ub.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qm.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://se.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xq.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ja.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ob.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ei.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mf.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gi.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://uz.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gp.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nc.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mv.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ya.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ez.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gb.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ly.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ci.hahajie.cn

[E16] 数字千分位
来源：http://op.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://pc.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://hz.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yt.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zo.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ol.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://al.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://an.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://qw.shtwfgs.cn

[E17] 首字母大写
来源：http://zh.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sd.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wj.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cf.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rd.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rl.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://ui.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xf.szxytkj.cn

[E18] 模板占位符替换
来源：http://je.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bf.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rh.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hu.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tx.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ef.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://un.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mf.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://io.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://ob.shxzukj.cn

Py:   s.splitlines()
来源：http://gu.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jb.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ta.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://xv.521024.cn

Java: s.lines().toList()
来源：http://ih.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://vh.hnjuh.cn

Ruby: s.lines
来源：http://lg.wgjwhj.cn

C#:   s.Split('\n')
来源：http://gd.nszjky.cn

[E20] 判断字符串是否为空
来源：http://py.gzmigu.cn

Py:   if not s:
来源：http://xl.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ft.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kp.muxihuayi.cn

TS:   if (s === "") {}
来源：http://oe.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://rq.bookmarksfly.cn

Go:   if s == "" {}
来源：http://ba.asd995.cn

Ruby: if s.empty?
来源：http://zo.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zw.521024.cn

[E21] 超长截断加省略号
来源：http://ce.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nm.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gi.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fj.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jc.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://li.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ky.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mh.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rk.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://ii.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bw.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oj.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ty.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rt.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nf.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ni.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://ef.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://um.nicolike.cn

================================================================================
来源：http://yu.panjiajie.cn

F. 文件与目录
来源：http://hm.szxytkj.cn

================================================================================
来源：http://ek.wgjwhj.cn

[F01] 读取整个文件
来源：http://rq.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cg.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://yk.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mp.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eq.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ps.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xx.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://rw.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://pn.huixiangedu.cn

[F02] 逐行读取文件
来源：http://yd.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kw.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kg.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bi.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lz.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://os.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pu.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://im.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://og.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://sc.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://am.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vn.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tb.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qv.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mj.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rm.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://jg.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mi.asd995.cn

[F04] 追加写入文件
来源：http://ww.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zb.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pw.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://je.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ld.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gq.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://is.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bl.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fi.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://kj.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hh.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://uw.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://lr.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://tn.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gs.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lr.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://hd.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ts.colortex.cn

[F06] 删除文件
来源：http://bt.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://jk.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://go.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ts.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bv.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qs.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://zr.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://cg.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://ne.9csxet.cn

[F07] 创建目录（含多级）
来源：http://hs.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uk.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jg.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qp.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rq.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rt.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qh.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ce.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lb.wgjwhj.cn

[F08] 遍历目录
来源：http://bz.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ke.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mn.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://nc.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://bn.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://us.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://td.asd995.cn

Ruby: Dir.children("dir")
来源：http://lc.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://ea.huixiangedu.cn

[F09] 获取文件大小
来源：http://uu.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://pe.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://bl.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://om.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://cw.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rq.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bq.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://pt.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://nv.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ad.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oq.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ou.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ev.newstarts.cn

TS:   path.extname("a.txt")
来源：http://kh.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aj.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://di.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ct.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dq.panjiajie.cn

[F11] 复制与移动文件
来源：http://rb.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xw.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ti.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bp.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kt.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gr.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vz.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://si.szxytkj.cn

[F12] CSV 读写
来源：http://je.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ie.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://at.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ou.wgjwhj.cn

TS:   // 同上
来源：http://rr.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wl.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://in.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://il.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ms.shxzukj.cn

================================================================================
来源：http://yh.haigaiapp.cn

G. 面向对象
来源：http://aj.bjjhwx.cn

================================================================================
来源：http://bn.huanxung.cn

[G01] 定义类
来源：http://oy.newstarts.cn


<!-- 参考信息 -->