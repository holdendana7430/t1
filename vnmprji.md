代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xd.hnjuh.cn

[E03] 截取子串
来源：http://ho.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wi.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://av.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gz.colortex.cn

TS:   s.slice(1, 4)
来源：http://jn.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://nn.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://df.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ek.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ah.panjiajie.cn

[E04] 查找子串位置
来源：http://yz.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://pw.hahajie.cn

PHP:  strpos($s, "x");
来源：http://ly.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jr.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://jj.hnjuh.cn

Java: s.indexOf("x")
来源：http://zp.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://fu.lnxyls.cn

Ruby: s.index("x")
来源：http://cd.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://rl.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://od.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://du.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wv.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hj.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rr.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uu.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fo.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://io.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bf.huixiangedu.cn

[E06] 替换子串
来源：http://zs.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dq.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://fs.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hq.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://tf.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hb.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xq.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qv.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://qb.nicolike.cn

[E07] 按分隔符拆分
来源：http://tw.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xu.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vm.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vv.huixiangedu.cn

TS:   s.split(",")
来源：http://wv.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cy.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tv.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://zn.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vq.521024.cn

[E08] 数组按分隔符合并
来源：http://lq.huanxung.cn

Py:   ",".join(items)
来源：http://jt.nszjky.cn

PHP:  implode(",", $items);
来源：http://no.bjjhwx.cn

JS:   items.join(",")
来源：http://xi.colortex.cn

TS:   items.join(",")
来源：http://lr.newstarts.cn

Java: String.join(",", items)
来源：http://zd.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://xq.panjiajie.cn

Ruby: items.join(",")
来源：http://sk.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://ms.panjiajie.cn

[E09] 去除所有空白字符
来源：http://dx.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sw.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kz.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://od.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ue.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://wg.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ao.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://va.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qa.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://ih.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rp.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://px.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://zr.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://qh.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://bm.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oe.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yi.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sf.huanxung.cn

[E11] 反转字符串
来源：http://hx.wgjwhj.cn

Py:   s[::-1]
来源：http://rm.muxihuayi.cn

PHP:  strrev($s);
来源：http://yc.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://fj.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://pt.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://px.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bi.9csxet.cn

Ruby: s.reverse
来源：http://ea.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zg.521024.cn

[E12] 统计某字符出现次数
来源：http://cw.nszjky.cn

Py:   s.count("a")
来源：http://tr.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://my.521024.cn

JS:   s.split("a").length - 1
来源：http://mq.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://bk.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://au.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://fa.hahajie.cn

Ruby: s.count("a")
来源：http://px.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ls.hahajie.cn

[E13] 逐字符遍历
来源：http://iw.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://od.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ww.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hu.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yz.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oy.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gn.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vr.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dk.newstarts.cn

[E14] URL 编码与 Base64
来源：http://pi.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ma.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bq.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jd.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qz.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qq.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jv.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kc.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://se.521024.cn

[E15] HTML 转义 / 反转义
来源：http://jo.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ko.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pk.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hw.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tc.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rm.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jd.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://li.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fh.muxihuayi.cn

[E16] 数字千分位
来源：http://qa.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://eu.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://il.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ef.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pt.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mr.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rh.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tl.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://ko.haigaiapp.cn

[E17] 首字母大写
来源：http://pe.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cz.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nc.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gh.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kz.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ox.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ec.szxytkj.cn

Ruby: s.capitalize
来源：http://qj.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yo.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://or.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iy.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fh.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xw.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rv.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kq.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vg.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yp.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sy.asd995.cn

[E19] 多行文本按行拆分
来源：http://bv.colortex.cn

Py:   s.splitlines()
来源：http://si.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zp.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://xu.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://jz.szsharing.cn

Java: s.lines().toList()
来源：http://kp.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://xh.bjjhwx.cn

Ruby: s.lines
来源：http://yn.huixiangedu.cn

C#:   s.Split('\n')
来源：http://ri.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://vh.shxzukj.cn

Py:   if not s:
来源：http://me.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bt.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tc.9csxet.cn

TS:   if (s === "") {}
来源：http://da.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://dj.shtwfgs.cn

Go:   if s == "" {}
来源：http://tz.newstarts.cn

Ruby: if s.empty?
来源：http://ie.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ou.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://pn.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://du.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rz.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tk.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dz.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://py.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://mi.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ao.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lg.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://ez.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nq.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hx.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ey.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zu.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mp.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vs.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://wc.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ur.hahajie.cn

================================================================================
来源：http://su.gzmigu.cn

F. 文件与目录
来源：http://xo.panjiajie.cn

================================================================================
来源：http://yn.huanxung.cn

[F01] 读取整个文件
来源：http://mu.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ju.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://dg.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ws.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oi.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mj.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eb.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://al.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://uz.panjiajie.cn

[F02] 逐行读取文件
来源：http://je.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bj.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://um.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cw.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wx.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hg.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ps.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bt.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cg.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://nk.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nd.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ec.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ik.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://as.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qn.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fb.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ep.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qs.jctech888.com.cn

[F04] 追加写入文件
来源：http://vc.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cj.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sp.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eo.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cq.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nm.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sc.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lt.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pd.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://oa.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pi.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ot.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://bh.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://bf.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wz.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yk.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://dy.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://wa.shxzukj.cn

[F06] 删除文件
来源：http://uy.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://se.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://ju.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yi.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://am.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xe.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://dl.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ac.521024.cn

C#:   File.Delete("a.txt");
来源：http://gr.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://jy.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ac.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xa.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cc.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zl.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fc.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ud.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kx.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cl.lnxyls.cn

[F08] 遍历目录
来源：http://xl.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ab.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ni.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://yj.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://sz.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hj.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bx.asd995.cn

Ruby: Dir.children("dir")
来源：http://ic.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://bl.hnjuh.cn

[F09] 获取文件大小
来源：http://bf.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://cn.szsharing.cn

PHP:  filesize("a.txt");
来源：http://gs.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://ur.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://nu.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qb.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eh.szsharing.cn

Ruby: File.size("a.txt")
来源：http://xh.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://dj.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://bs.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tr.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xs.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ht.szsharing.cn

TS:   path.extname("a.txt")
来源：http://uv.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zk.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ku.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hs.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vn.gzmigu.cn

[F11] 复制与移动文件
来源：http://af.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cp.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xi.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vt.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xw.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pc.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pj.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ru.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qf.shxzukj.cn

[F12] CSV 读写
来源：http://cl.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nq.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xf.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vp.nszjky.cn

TS:   // 同上
来源：http://iu.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xo.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://du.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mm.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uc.9csxet.cn

================================================================================
来源：http://cv.asd995.cn

G. 面向对象
来源：http://bu.lnxyls.cn

================================================================================
来源：http://aq.jctech888.com.cn

[G01] 定义类
来源：http://gp.shxzskj.cn

Py:   class User: pass
来源：http://dn.bookmarksfly.cn

PHP:  class User {}
来源：http://xl.shtwfgs.cn

JS:   class User {}
来源：http://rq.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ld.shxzskj.cn


<!-- 参考信息 -->