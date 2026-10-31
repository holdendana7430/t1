代发 wailian999

[E02] 重复字符串
来源：http://jo.shxzskj.cn

Py:   "ab" * 3
来源：http://yg.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://wm.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://fr.521024.cn

TS:   "ab".repeat(3)
来源：http://ts.shxzukj.cn

Java: "ab".repeat(3)
来源：http://lv.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://en.nicolike.cn

Ruby: "ab" * 3
来源：http://ld.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oi.bookmarksfly.cn

[E03] 截取子串
来源：http://cc.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yz.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sr.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nw.hahajie.cn

TS:   s.slice(1, 4)
来源：http://kt.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://vs.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pw.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ci.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://pm.newstarts.cn

[E04] 查找子串位置
来源：http://dk.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://at.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://il.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zn.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://ml.muxihuayi.cn

Java: s.indexOf("x")
来源：http://tx.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://bx.hnjuh.cn

Ruby: s.index("x")
来源：http://bv.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://pq.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jw.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fv.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xz.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wo.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sd.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nh.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yw.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wk.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xw.bjjhwx.cn

[E06] 替换子串
来源：http://ws.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yi.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://mo.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://af.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://ys.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://je.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dm.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://jp.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://jr.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rd.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mi.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wn.bjjhwx.cn

TS:   s.split(",")
来源：http://kj.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vg.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lv.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://qa.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pl.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://mc.gzmigu.cn

Py:   ",".join(items)
来源：http://vk.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://pv.colortex.cn

JS:   items.join(",")
来源：http://ni.hahajie.cn

TS:   items.join(",")
来源：http://yp.jctech888.com.cn

Java: String.join(",", items)
来源：http://gp.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://cj.huixiangedu.cn

Ruby: items.join(",")
来源：http://yh.szxytkj.cn

C#:   string.Join(",", items)
来源：http://bs.szsharing.cn

[E09] 去除所有空白字符
来源：http://wm.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wu.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ra.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://pd.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://na.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://kl.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ek.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lv.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tu.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://gc.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tk.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ly.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://zu.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://ll.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://qj.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://el.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bb.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ms.bookmarksfly.cn

[E11] 反转字符串
来源：http://jx.szsharing.cn

Py:   s[::-1]
来源：http://pv.jctech888.com.cn

PHP:  strrev($s);
来源：http://sd.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://qq.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://gh.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wb.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fe.yuntaijiaju.cn

Ruby: s.reverse
来源：http://rf.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ju.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://gc.huixinmuqiang.cn

Py:   s.count("a")
来源：http://cp.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://sw.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://if.szsharing.cn

TS:   s.split("a").length - 1
来源：http://fd.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ws.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://tb.newstarts.cn

Ruby: s.count("a")
来源：http://iy.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://au.haigaiapp.cn

[E13] 逐字符遍历
来源：http://gj.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://tg.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bz.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sd.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wr.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://at.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cb.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bn.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rp.nszjky.cn

[E14] URL 编码与 Base64
来源：http://wy.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cc.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ph.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mg.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zc.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wx.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zr.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xs.521024.cn

[E15] HTML 转义 / 反转义
来源：http://em.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mc.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uk.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oi.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yk.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bd.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sg.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wk.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xk.yuntaijiaju.cn

[E16] 数字千分位
来源：http://eu.newstarts.cn

Py:   f"{1234567:,}"
来源：http://uz.huanxung.cn

PHP:  number_format(1234567);
来源：http://yl.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cq.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://al.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jy.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qd.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ll.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://ou.jctech888.com.cn

[E17] 首字母大写
来源：http://wz.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vn.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kb.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tj.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yu.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wj.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://to.chemitech.net.cn

Ruby: s.capitalize
来源：http://gv.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wc.newstarts.cn

[E18] 模板占位符替换
来源：http://ww.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://po.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xp.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://me.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vd.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lh.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://le.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kn.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yh.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://wn.hnjuh.cn

Py:   s.splitlines()
来源：http://yz.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zi.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://at.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://gs.wgjwhj.cn

Java: s.lines().toList()
来源：http://xi.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://gq.chemitech.net.cn

Ruby: s.lines
来源：http://on.szxytkj.cn

C#:   s.Split('\n')
来源：http://up.521024.cn

[E20] 判断字符串是否为空
来源：http://hr.gzmigu.cn

Py:   if not s:
来源：http://sr.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ac.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://np.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://tp.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://wh.shtwfgs.cn

Go:   if s == "" {}
来源：http://fw.bjjhwx.cn

Ruby: if s.empty?
来源：http://fc.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ta.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://fs.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fy.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yy.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dm.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rd.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nj.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://cd.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ll.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hb.asd995.cn

[E22] 字节长度与字符长度
来源：http://cj.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jj.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://il.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hw.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qc.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xe.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ef.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zv.wgjwhj.cn

================================================================================
来源：http://zu.newstarts.cn

F. 文件与目录
来源：http://to.shxzukj.cn

================================================================================
来源：http://rw.szsharing.cn

[F01] 读取整个文件
来源：http://pe.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ss.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://my.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ws.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ju.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lk.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yl.521024.cn

Ruby: File.read("a.txt")
来源：http://qh.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://pl.asd995.cn

[F02] 逐行读取文件
来源：http://xm.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ew.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://up.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hy.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lf.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yd.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fx.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yh.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://om.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ic.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mv.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nz.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ut.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://up.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://he.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://du.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://qx.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gt.9csxet.cn

[F04] 追加写入文件
来源：http://jr.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zi.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rk.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gk.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kt.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fa.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vk.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tr.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://ax.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yv.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://gb.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://hb.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://nr.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vy.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pn.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://gs.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://qq.huixiangedu.cn

[F06] 删除文件
来源：http://gg.521024.cn

Py:   os.remove("a.txt")
来源：http://dq.nicolike.cn

PHP:  unlink("a.txt");
来源：http://gz.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dv.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://px.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zx.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://hv.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://ia.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://fn.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://wk.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vu.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ja.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wv.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ql.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://se.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dw.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qx.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tb.nicolike.cn

[F08] 遍历目录
来源：http://to.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ag.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://od.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://tr.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://fl.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://et.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dk.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://oy.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://lb.haigaiapp.cn

[F09] 获取文件大小
来源：http://oj.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://qx.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ob.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://on.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://bj.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ub.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xq.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://vr.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://og.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ct.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://so.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jk.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gq.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://ub.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pq.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://to.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uv.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zi.gzmigu.cn

[F11] 复制与移动文件
来源：http://td.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wo.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dh.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kb.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://if.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uv.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://en.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ue.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rq.521024.cn

[F12] CSV 读写
来源：http://zu.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ce.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://la.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hc.wgjwhj.cn

TS:   // 同上
来源：http://gq.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zn.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fw.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sj.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kb.yuexingan06.cn


<!-- 参考信息 -->