代发 wailian999

Java: String.join(", ", list)
来源：http://wp.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://pg.hnjuh.cn

Ruby: arr.join(", ")
来源：http://tp.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://ld.9csxet.cn

================================================================================
来源：http://gm.nszjky.cn

E. 字符串处理
来源：http://mj.newstarts.cn

================================================================================
来源：http://dj.haigaiapp.cn

[E01] 拼接字符串
来源：http://cf.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gs.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bf.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nm.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bd.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sm.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yr.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tl.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vc.wgjwhj.cn

[E02] 重复字符串
来源：http://lw.jctech888.com.cn

Py:   "ab" * 3
来源：http://ez.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ti.nszjky.cn

JS:   "ab".repeat(3)
来源：http://te.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://si.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ci.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://en.szxytkj.cn

Ruby: "ab" * 3
来源：http://cg.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jf.wgjwhj.cn

[E03] 截取子串
来源：http://bf.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wu.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wo.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rd.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://ki.lnxyls.cn

Java: s.substring(1, 4)
来源：http://sb.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yp.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://as.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://my.shxzskj.cn

[E04] 查找子串位置
来源：http://nj.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://lo.521024.cn

PHP:  strpos($s, "x");
来源：http://zd.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jx.lnxyls.cn

TS:   s.indexOf("x")
来源：http://my.nicolike.cn

Java: s.indexOf("x")
来源：http://rg.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://ps.huanxung.cn

Ruby: s.index("x")
来源：http://pc.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://cd.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nv.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zy.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://th.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dz.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ex.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cb.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ma.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fp.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ln.haigaiapp.cn

[E06] 替换子串
来源：http://im.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kg.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://rg.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://by.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://ik.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tp.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qk.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tq.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://sd.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://qj.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xi.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://up.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qn.lnxyls.cn

TS:   s.split(",")
来源：http://om.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fn.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cx.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://pv.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pp.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://dx.shxzukj.cn

Py:   ",".join(items)
来源：http://hi.hnjuh.cn

PHP:  implode(",", $items);
来源：http://dj.haigaiapp.cn

JS:   items.join(",")
来源：http://rf.panjiajie.cn

TS:   items.join(",")
来源：http://mb.panjiajie.cn

Java: String.join(",", items)
来源：http://xm.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://id.hnjuh.cn

Ruby: items.join(",")
来源：http://om.lnxyls.cn

C#:   string.Join(",", items)
来源：http://ne.nicolike.cn

[E09] 去除所有空白字符
来源：http://kz.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pl.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ss.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://cv.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://tg.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://kb.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yd.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lc.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mo.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://vm.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vq.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wc.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://bs.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ic.szsharing.cn

Java: String.format("%03d", 7)
来源：http://xf.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://da.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fh.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jd.muxihuayi.cn

[E11] 反转字符串
来源：http://bc.chemitech.net.cn

Py:   s[::-1]
来源：http://do.huanxung.cn

PHP:  strrev($s);
来源：http://vq.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://df.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://kj.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tp.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kc.521024.cn

Ruby: s.reverse
来源：http://cl.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wu.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ys.panjiajie.cn

Py:   s.count("a")
来源：http://wf.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://qg.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://np.521024.cn

TS:   s.split("a").length - 1
来源：http://cf.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dk.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://uf.shxzukj.cn

Ruby: s.count("a")
来源：http://nc.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://wy.yuexingan06.cn

[E13] 逐字符遍历
来源：http://ki.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://eb.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fk.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://es.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yv.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ft.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uo.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xa.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bj.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://lq.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://du.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jp.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tv.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cd.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vn.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nq.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yt.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ap.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://kw.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uj.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bn.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pb.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qe.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://og.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wx.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tq.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yl.newstarts.cn

[E16] 数字千分位
来源：http://me.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://fl.hnjuh.cn

PHP:  number_format(1234567);
来源：http://km.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nn.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ta.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ku.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mq.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bf.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://gr.jianghongdianzi.cn

[E17] 首字母大写
来源：http://wi.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rk.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uo.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sf.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wv.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mb.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ru.chemitech.net.cn

Ruby: s.capitalize
来源：http://nn.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ub.muxihuayi.cn

[E18] 模板占位符替换
来源：http://gk.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://je.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://au.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bo.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ua.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vx.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mc.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lk.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yp.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://eo.nicolike.cn

Py:   s.splitlines()
来源：http://hb.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ls.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://nr.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://ht.9csxet.cn

Java: s.lines().toList()
来源：http://cu.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://mx.lnxyls.cn

Ruby: s.lines
来源：http://rg.9csxet.cn

C#:   s.Split('\n')
来源：http://fw.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ov.szsharing.cn

Py:   if not s:
来源：http://sv.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tf.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oy.newstarts.cn

TS:   if (s === "") {}
来源：http://lf.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://go.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://xi.521024.cn

Ruby: if s.empty?
来源：http://eg.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gn.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://gp.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dq.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nu.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qd.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tw.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qg.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ag.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://te.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://td.asd995.cn

[E22] 字节长度与字符长度
来源：http://gy.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yx.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jc.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://of.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kx.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lg.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ed.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://yo.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gv.9csxet.cn

================================================================================
来源：http://wk.jctech888.com.cn

F. 文件与目录
来源：http://kc.bookmarksfly.cn

================================================================================
来源：http://af.huixiangedu.cn

[F01] 读取整个文件
来源：http://dz.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pv.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://jf.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lt.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lx.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fb.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bz.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://od.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wa.haigaiapp.cn

[F02] 逐行读取文件
来源：http://ie.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ka.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tg.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bh.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ch.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kh.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bw.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uc.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kv.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ts.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mt.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cl.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bl.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ob.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ei.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zq.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://mj.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zj.bookmarksfly.cn

[F04] 追加写入文件
来源：http://nh.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ok.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yt.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lq.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fg.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://da.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mz.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gy.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yn.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://en.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hs.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://lb.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://no.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://tt.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://li.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rf.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://br.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://im.nszjky.cn

[F06] 删除文件
来源：http://wj.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://xd.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://jr.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tp.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ki.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zv.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://yg.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://sc.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://qm.nszjky.cn

[F07] 创建目录（含多级）
来源：http://lw.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://db.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ya.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wu.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ze.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dy.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hf.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ve.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qe.huixinmuqiang.cn

[F08] 遍历目录
来源：http://or.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kf.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kj.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://dl.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://im.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hd.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lw.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://bo.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://vw.huanxung.cn

[F09] 获取文件大小
来源：http://aj.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://du.nicolike.cn

PHP:  filesize("a.txt");
来源：http://fn.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ao.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://cp.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qh.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://la.nicolike.cn

Ruby: File.size("a.txt")
来源：http://mu.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://hd.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rn.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://os.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ck.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hq.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://ou.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fh.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sb.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://po.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iq.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://jt.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ra.lnxyls.cn


<!-- 参考信息 -->