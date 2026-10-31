代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jd.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ws.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fc.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ew.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fx.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vi.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dn.panjiajie.cn

[E02] 重复字符串
来源：http://ee.huanxung.cn

Py:   "ab" * 3
来源：http://vo.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://xu.9csxet.cn

JS:   "ab".repeat(3)
来源：http://xr.asd995.cn

TS:   "ab".repeat(3)
来源：http://kq.lnxyls.cn

Java: "ab".repeat(3)
来源：http://eb.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://xz.shxzukj.cn

Ruby: "ab" * 3
来源：http://sy.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ql.hnjuh.cn

[E03] 截取子串
来源：http://sq.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sk.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eu.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iw.nszjky.cn

TS:   s.slice(1, 4)
来源：http://cf.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ar.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zb.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gw.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://mi.yuexingan06.cn

[E04] 查找子串位置
来源：http://ul.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://qy.szsharing.cn

PHP:  strpos($s, "x");
来源：http://kw.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xl.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://wu.9csxet.cn

Java: s.indexOf("x")
来源：http://qj.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://bi.hnjuh.cn

Ruby: s.index("x")
来源：http://ss.huanxung.cn

C#:   s.IndexOf("x")
来源：http://tz.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://so.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ej.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nr.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ad.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pw.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yn.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nx.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://un.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ta.bookmarksfly.cn

[E06] 替换子串
来源：http://ni.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lo.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://yw.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tk.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://vr.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jj.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ew.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uh.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://wh.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ns.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wg.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nt.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gm.szxytkj.cn

TS:   s.split(",")
来源：http://uc.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jo.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qn.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://uq.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://di.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://kz.9csxet.cn

Py:   ",".join(items)
来源：http://tr.szsharing.cn

PHP:  implode(",", $items);
来源：http://zv.huanxung.cn

JS:   items.join(",")
来源：http://rq.shxzukj.cn

TS:   items.join(",")
来源：http://jj.newstarts.cn

Java: String.join(",", items)
来源：http://rj.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://lq.bjjhwx.cn

Ruby: items.join(",")
来源：http://rs.521024.cn

C#:   string.Join(",", items)
来源：http://dp.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://vc.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jx.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://el.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://vw.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://xb.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://kr.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hr.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wi.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gs.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ft.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kw.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jm.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://pm.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://xy.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://uq.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dh.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oa.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qg.bjjhwx.cn

[E11] 反转字符串
来源：http://fv.nicolike.cn

Py:   s[::-1]
来源：http://lh.asd995.cn

PHP:  strrev($s);
来源：http://rq.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://ip.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://as.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rw.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zb.nicolike.cn

Ruby: s.reverse
来源：http://ig.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wb.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://pr.shxzukj.cn

Py:   s.count("a")
来源：http://ix.colortex.cn

PHP:  substr_count($s, "a");
来源：http://qr.hahajie.cn

JS:   s.split("a").length - 1
来源：http://se.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://dt.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hf.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://jt.shxzskj.cn

Ruby: s.count("a")
来源：http://pu.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://tf.9csxet.cn

[E13] 逐字符遍历
来源：http://lj.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://cu.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iq.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rx.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fg.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://if.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pv.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hk.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ht.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://kv.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ze.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bk.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qt.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ra.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://px.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wu.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fi.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://dz.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zu.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ib.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yb.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uo.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tv.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ih.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vg.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nz.newstarts.cn

[E16] 数字千分位
来源：http://lb.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://sj.newstarts.cn

PHP:  number_format(1234567);
来源：http://eg.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://td.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jn.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qg.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dl.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ea.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://ak.9csxet.cn

[E17] 首字母大写
来源：http://tx.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mc.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tc.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wx.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hs.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kt.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bg.nicolike.cn

Ruby: s.capitalize
来源：http://sx.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ee.chemitech.net.cn

[E18] 模板占位符替换
来源：http://hh.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bq.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zn.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ce.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tb.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://in.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qh.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oz.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fu.521024.cn

[E19] 多行文本按行拆分
来源：http://fa.panjiajie.cn

Py:   s.splitlines()
来源：http://zs.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nr.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://eo.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://oq.bjjhwx.cn

Java: s.lines().toList()
来源：http://mt.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://jk.huixinmuqiang.cn

Ruby: s.lines
来源：http://il.shtwfgs.cn

C#:   s.Split('\n')
来源：http://lh.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ju.shxzskj.cn

Py:   if not s:
来源：http://ig.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tj.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pa.521024.cn

TS:   if (s === "") {}
来源：http://sv.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://ly.lnxyls.cn

Go:   if s == "" {}
来源：http://wj.huanxung.cn

Ruby: if s.empty?
来源：http://os.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kl.colortex.cn

[E21] 超长截断加省略号
来源：http://cj.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ii.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lk.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bx.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://op.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ll.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gl.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vp.szsharing.cn

[E22] 字节长度与字符长度
来源：http://wy.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uo.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rv.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lr.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tc.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qj.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cs.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://mj.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://je.lnxyls.cn

================================================================================
来源：http://hx.bjjhwx.cn

F. 文件与目录
来源：http://ag.jianghongdianzi.cn

================================================================================
来源：http://tk.yuexingan06.cn

[F01] 读取整个文件
来源：http://ye.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gb.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://jm.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ng.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zb.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pi.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://if.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://bk.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://mz.9csxet.cn

[F02] 逐行读取文件
来源：http://fv.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fc.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://it.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lf.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vd.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kd.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qa.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qk.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pp.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://sh.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gl.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qo.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qp.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gn.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zw.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ld.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rf.shtwfgs.cn

[F04] 追加写入文件
来源：http://tj.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://df.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://di.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ky.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oz.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nc.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://no.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xo.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://wi.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://av.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://rq.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://gx.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://es.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pc.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cg.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://lc.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://gy.nicolike.cn

[F06] 删除文件
来源：http://af.asd995.cn

Py:   os.remove("a.txt")
来源：http://kh.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://kp.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gv.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cy.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kj.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://io.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://rq.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://bz.newstarts.cn

[F07] 创建目录（含多级）
来源：http://wk.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ws.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qu.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vo.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tg.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jf.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ei.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sa.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gz.szxytkj.cn

[F08] 遍历目录
来源：http://xl.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nt.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kc.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://lw.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://cb.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dk.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://io.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://fi.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://hq.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://mr.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://hs.hahajie.cn

PHP:  filesize("a.txt");
来源：http://qg.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://eu.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://yo.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://we.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hq.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://sy.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://rj.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://qa.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xw.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pl.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://in.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://qb.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pr.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ay.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gc.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bs.colortex.cn

[F11] 复制与移动文件
来源：http://bd.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tl.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yx.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vl.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tu.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fw.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pc.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pm.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mp.huixinmuqiang.cn

[F12] CSV 读写
来源：http://fk.wgjwhj.cn


<!-- 参考信息 -->