代发 wailian999

TS:   "ab".repeat(3)
来源：http://za.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://kj.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://gs.nicolike.cn

Ruby: "ab" * 3
来源：http://op.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://co.9csxet.cn

[E03] 截取子串
来源：http://uq.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bd.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sy.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ps.colortex.cn

TS:   s.slice(1, 4)
来源：http://gy.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://xu.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dp.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mv.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://yv.bookmarksfly.cn

[E04] 查找子串位置
来源：http://fj.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://kg.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://mz.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lg.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://yw.nszjky.cn

Java: s.indexOf("x")
来源：http://jl.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://ah.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://eu.newstarts.cn

C#:   s.IndexOf("x")
来源：http://gm.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fv.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dp.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hk.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pk.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tt.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jl.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://am.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://op.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sx.521024.cn

[E06] 替换子串
来源：http://fq.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tz.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://wt.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gd.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://jg.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gh.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sk.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ch.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://xm.hahajie.cn

[E07] 按分隔符拆分
来源：http://tq.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dh.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lh.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jj.szxytkj.cn

TS:   s.split(",")
来源：http://zp.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wx.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hf.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://ey.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tf.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://ez.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ls.nszjky.cn

PHP:  implode(",", $items);
来源：http://ng.hnjuh.cn

JS:   items.join(",")
来源：http://fc.9csxet.cn

TS:   items.join(",")
来源：http://or.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://ol.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://mu.panjiajie.cn

Ruby: items.join(",")
来源：http://gn.lnxyls.cn

C#:   string.Join(",", items)
来源：http://wo.newstarts.cn

[E09] 去除所有空白字符
来源：http://dj.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vo.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lr.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://sx.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://gf.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://gh.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jf.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qm.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://at.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://xf.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mj.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fd.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://lw.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://lf.newstarts.cn

Java: String.format("%03d", 7)
来源：http://sl.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gn.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zv.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://js.nicolike.cn

[E11] 反转字符串
来源：http://hb.huixiangedu.cn

Py:   s[::-1]
来源：http://hi.shxzskj.cn

PHP:  strrev($s);
来源：http://rj.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://ld.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://yh.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://co.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://de.nicolike.cn

Ruby: s.reverse
来源：http://bi.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ui.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://eg.colortex.cn

Py:   s.count("a")
来源：http://iv.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://fg.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://br.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://ph.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ja.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://rr.hnjuh.cn

Ruby: s.count("a")
来源：http://sa.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://er.nszjky.cn

[E13] 逐字符遍历
来源：http://gk.asd995.cn

Py:   for ch in s: print(ch)
来源：http://bk.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://so.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lh.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wu.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qq.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wr.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lz.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hk.hahajie.cn

[E14] URL 编码与 Base64
来源：http://tw.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sb.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ia.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jy.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://do.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://th.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lo.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://or.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://zn.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ya.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tx.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gy.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dq.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zx.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wp.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uk.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sh.huixinmuqiang.cn

[E16] 数字千分位
来源：http://xr.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://sk.newstarts.cn

PHP:  number_format(1234567);
来源：http://pj.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://av.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sh.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hh.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gw.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://el.9csxet.cn

[E17] 首字母大写
来源：http://fr.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qc.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vg.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qx.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tx.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tg.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dj.lnxyls.cn

Ruby: s.capitalize
来源：http://kj.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://as.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://ox.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xy.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bx.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eo.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fd.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ce.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dq.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rt.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vy.hahajie.cn

[E19] 多行文本按行拆分
来源：http://zd.szsharing.cn

Py:   s.splitlines()
来源：http://xh.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ys.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://lc.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://hi.newstarts.cn

Java: s.lines().toList()
来源：http://qt.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://vt.nicolike.cn

Ruby: s.lines
来源：http://gm.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://dl.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://xv.szsharing.cn

Py:   if not s:
来源：http://po.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ip.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rn.hahajie.cn

TS:   if (s === "") {}
来源：http://av.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://qq.huixiangedu.cn

Go:   if s == "" {}
来源：http://xp.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://bd.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fl.newstarts.cn

[E21] 超长截断加省略号
来源：http://ju.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rl.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rk.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wx.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yp.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://yh.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mg.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ke.nszjky.cn

[E22] 字节长度与字符长度
来源：http://zi.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://on.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ws.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gb.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pb.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ek.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://di.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pp.shxzskj.cn

================================================================================
来源：http://jq.asd995.cn

F. 文件与目录
来源：http://sx.nszjky.cn

================================================================================
来源：http://zf.lnxyls.cn

[F01] 读取整个文件
来源：http://xa.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yo.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://fj.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ar.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ho.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fy.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tt.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://fk.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://ht.muxihuayi.cn

[F02] 逐行读取文件
来源：http://hq.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ap.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dx.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xb.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sy.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ck.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ja.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gx.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ku.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://uu.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pv.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wc.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ws.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ih.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gt.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ag.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://ux.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bb.asd995.cn

[F04] 追加写入文件
来源：http://th.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oc.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rk.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qa.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ga.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ut.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pq.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hy.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://af.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://av.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://kz.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://wc.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://rg.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gu.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kg.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://mw.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://rn.huixinmuqiang.cn

[F06] 删除文件
来源：http://go.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://cg.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ye.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uu.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bt.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://un.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://jz.colortex.cn

Ruby: File.delete("a.txt")
来源：http://pk.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://qw.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://hv.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mq.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jg.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nk.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://su.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://be.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kv.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hm.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://px.521024.cn

[F08] 遍历目录
来源：http://ia.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://os.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tm.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://af.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://rh.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tj.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wh.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://da.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://on.hnjuh.cn

[F09] 获取文件大小
来源：http://jn.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://jt.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://xr.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://xt.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://xu.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ox.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ff.nicolike.cn

Ruby: File.size("a.txt")
来源：http://kr.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://gn.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kq.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ii.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ch.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nm.asd995.cn

TS:   path.extname("a.txt")
来源：http://kh.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rx.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ql.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cx.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://im.asd995.cn

[F11] 复制与移动文件
来源：http://sa.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wh.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://js.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ku.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qw.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xl.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hn.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gx.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qo.shxzskj.cn

[F12] CSV 读写
来源：http://id.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pr.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qk.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wk.hnjuh.cn

TS:   // 同上
来源：http://dg.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ih.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hg.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yu.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mq.newstarts.cn

================================================================================
来源：http://at.huixiangedu.cn

G. 面向对象
来源：http://ft.9csxet.cn

================================================================================
来源：http://rk.gzmigu.cn

[G01] 定义类
来源：http://xe.bjjhwx.cn


<!-- 参考信息 -->