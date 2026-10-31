代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dx.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ie.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://we.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ov.shtwfgs.cn

[E02] 重复字符串
来源：http://pg.shxzskj.cn

Py:   "ab" * 3
来源：http://zv.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://xs.hahajie.cn

JS:   "ab".repeat(3)
来源：http://pf.nicolike.cn

TS:   "ab".repeat(3)
来源：http://wg.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://fe.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://qc.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://lw.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fe.chemitech.net.cn

[E03] 截取子串
来源：http://hj.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ke.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dj.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pp.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://rl.shxzskj.cn

Java: s.substring(1, 4)
来源：http://nq.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bl.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://my.521024.cn

C#:   s.Substring(1, 3)
来源：http://vn.yuexingan06.cn

[E04] 查找子串位置
来源：http://df.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://lr.szsharing.cn

PHP:  strpos($s, "x");
来源：http://ta.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fa.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://mf.szxytkj.cn

Java: s.indexOf("x")
来源：http://gl.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://up.asd995.cn

Ruby: s.index("x")
来源：http://iv.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://od.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oo.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iu.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nl.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tk.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dl.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://er.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://on.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hy.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mm.nicolike.cn

[E06] 替换子串
来源：http://pp.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tf.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://kj.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zd.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://lf.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nn.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vq.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lq.colortex.cn

C#:   s.Replace("a", "b")
来源：http://lw.nszjky.cn

[E07] 按分隔符拆分
来源：http://og.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pq.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ut.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sz.muxihuayi.cn

TS:   s.split(",")
来源：http://il.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gg.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fn.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://qf.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sy.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://rv.szxytkj.cn

Py:   ",".join(items)
来源：http://pi.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://cx.shxzukj.cn

JS:   items.join(",")
来源：http://kr.panjiajie.cn

TS:   items.join(",")
来源：http://co.nicolike.cn

Java: String.join(",", items)
来源：http://gb.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://wc.521024.cn

Ruby: items.join(",")
来源：http://tr.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://ue.521024.cn

[E09] 去除所有空白字符
来源：http://yj.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gw.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hi.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://ot.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://pr.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://tq.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wc.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pg.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hu.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://ul.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bn.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://al.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://mz.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://mp.9csxet.cn

Java: String.format("%03d", 7)
来源：http://vs.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iq.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ti.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cn.521024.cn

[E11] 反转字符串
来源：http://as.muxihuayi.cn

Py:   s[::-1]
来源：http://pp.newstarts.cn

PHP:  strrev($s);
来源：http://wc.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://td.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://wz.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ze.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wx.gzmigu.cn

Ruby: s.reverse
来源：http://ei.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://az.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ad.521024.cn

Py:   s.count("a")
来源：http://cc.colortex.cn

PHP:  substr_count($s, "a");
来源：http://nx.9csxet.cn

JS:   s.split("a").length - 1
来源：http://ea.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://tg.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ev.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://ii.jctech888.com.cn

Ruby: s.count("a")
来源：http://wa.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://tf.panjiajie.cn

[E13] 逐字符遍历
来源：http://jq.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://kl.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eq.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pm.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gm.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ia.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jl.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vu.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://tu.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bc.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kp.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fo.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bn.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mf.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://io.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gi.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xv.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://zr.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://co.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vo.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cv.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tg.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mq.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mv.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://an.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://an.huixiangedu.cn

[E16] 数字千分位
来源：http://rf.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://zn.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://qx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nh.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ot.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ue.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hj.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://je.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://qz.muxihuayi.cn

[E17] 首字母大写
来源：http://xa.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xj.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bt.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oz.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oj.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fd.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qo.chemitech.net.cn

Ruby: s.capitalize
来源：http://kg.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ta.haigaiapp.cn

[E18] 模板占位符替换
来源：http://zr.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ei.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yf.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bv.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kp.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ro.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ew.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xb.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://du.nicolike.cn

[E19] 多行文本按行拆分
来源：http://cq.colortex.cn

Py:   s.splitlines()
来源：http://pr.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ei.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://vl.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://qx.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://my.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://ku.huanxung.cn

Ruby: s.lines
来源：http://ry.9csxet.cn

C#:   s.Split('\n')
来源：http://cw.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://uz.shtwfgs.cn

Py:   if not s:
来源：http://qg.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ir.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gi.jctech888.com.cn

TS:   if (s === "") {}
来源：http://cw.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://eb.521024.cn

Go:   if s == "" {}
来源：http://rm.jctech888.com.cn

Ruby: if s.empty?
来源：http://vm.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nw.9csxet.cn

[E21] 超长截断加省略号
来源：http://zk.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hw.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zy.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xb.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ma.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://lr.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oi.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kn.521024.cn

[E22] 字节长度与字符长度
来源：http://si.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oq.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vq.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ij.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bv.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ii.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zr.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://fm.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ay.asd995.cn

================================================================================
来源：http://fl.521024.cn

F. 文件与目录
来源：http://rf.wgjwhj.cn

================================================================================
来源：http://te.panjiajie.cn

[F01] 读取整个文件
来源：http://uc.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xg.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ms.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cu.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vz.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jn.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yt.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://vn.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://uo.szsharing.cn

[F02] 逐行读取文件
来源：http://lc.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uo.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kj.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vo.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pl.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hj.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vg.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://tl.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sx.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sp.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rr.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pl.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lv.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oa.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://ef.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wc.nicolike.cn

[F04] 追加写入文件
来源：http://ak.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lh.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://le.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rb.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mn.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tt.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jw.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jh.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gg.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ev.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wk.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://cg.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://gy.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://be.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ph.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ju.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://pd.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://dx.yuntaijiaju.cn

[F06] 删除文件
来源：http://qu.szsharing.cn

Py:   os.remove("a.txt")
来源：http://fl.nszjky.cn

PHP:  unlink("a.txt");
来源：http://fy.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kq.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hx.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zi.521024.cn

Go:   os.Remove("a.txt")
来源：http://fi.asd995.cn

Ruby: File.delete("a.txt")
来源：http://pz.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://zs.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://gq.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ot.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kr.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zj.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pw.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nu.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jt.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kr.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eb.szsharing.cn

[F08] 遍历目录
来源：http://jv.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://im.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fy.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://ah.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://on.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ib.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gv.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://kk.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://qb.shxzukj.cn

[F09] 获取文件大小
来源：http://yx.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://vn.521024.cn

PHP:  filesize("a.txt");
来源：http://cb.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://ui.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://mv.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iy.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mk.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://zd.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://hp.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://dn.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://za.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ib.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mq.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://mu.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fj.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tm.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qc.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gm.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://gl.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pc.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ey.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dc.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hw.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nm.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sz.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://if.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gc.nicolike.cn

[F12] CSV 读写
来源：http://lp.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sa.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://um.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wc.gzmigu.cn

TS:   // 同上
来源：http://qw.bookmarksfly.cn


<!-- 参考信息 -->