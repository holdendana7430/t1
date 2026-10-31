代发 wailian999

TS:   "ab".repeat(3)
来源：http://xg.asd995.cn

Java: "ab".repeat(3)
来源：http://ly.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://mo.haigaiapp.cn

Ruby: "ab" * 3
来源：http://xk.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gk.huixiangedu.cn

[E03] 截取子串
来源：http://rd.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qq.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nu.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ro.521024.cn

TS:   s.slice(1, 4)
来源：http://ga.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://xa.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mu.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mb.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ni.muxihuayi.cn

[E04] 查找子串位置
来源：http://xe.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://rh.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://rs.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jp.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://ll.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://ig.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://ta.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://cx.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://qg.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fl.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hj.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cn.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bj.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://as.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kw.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tj.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zn.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ge.shxzukj.cn

[E06] 替换子串
来源：http://sd.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kl.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vj.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sg.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://ix.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xl.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fh.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zh.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://ov.gzmigu.cn

[E07] 按分隔符拆分
来源：http://td.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xn.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yc.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ss.bjjhwx.cn

TS:   s.split(",")
来源：http://wm.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hy.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pb.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://tc.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cu.colortex.cn

[E08] 数组按分隔符合并
来源：http://qo.bjjhwx.cn

Py:   ",".join(items)
来源：http://lk.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://tl.huixinmuqiang.cn

JS:   items.join(",")
来源：http://jp.newstarts.cn

TS:   items.join(",")
来源：http://of.asd995.cn

Java: String.join(",", items)
来源：http://ze.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://tr.9csxet.cn

Ruby: items.join(",")
来源：http://dk.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://sp.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://xf.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ki.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zm.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://rd.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://gm.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://ww.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wa.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eu.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sw.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://uv.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cr.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bd.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://us.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://vt.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://vh.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hm.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iq.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nl.hahajie.cn

[E11] 反转字符串
来源：http://hh.nicolike.cn

Py:   s[::-1]
来源：http://ok.lnxyls.cn

PHP:  strrev($s);
来源：http://gz.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://vy.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://tv.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dq.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eh.9csxet.cn

Ruby: s.reverse
来源：http://qu.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fc.9csxet.cn

[E12] 统计某字符出现次数
来源：http://db.muxihuayi.cn

Py:   s.count("a")
来源：http://as.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://xa.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://ux.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://yg.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ny.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://so.shxzukj.cn

Ruby: s.count("a")
来源：http://xk.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://rg.gzmigu.cn

[E13] 逐字符遍历
来源：http://oy.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://yq.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fx.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://in.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qg.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://du.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hr.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wt.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sf.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ie.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://js.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yq.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pp.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rd.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://js.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zd.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qu.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://pu.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xs.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zt.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sh.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bx.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hh.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sb.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wa.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rx.yuexingan06.cn

[E16] 数字千分位
来源：http://wx.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://ml.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://kj.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tz.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gv.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oa.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lf.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qk.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://sm.jianghongdianzi.cn

[E17] 首字母大写
来源：http://qe.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qu.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vm.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qj.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://la.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zg.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bw.szxytkj.cn

Ruby: s.capitalize
来源：http://yx.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pl.chemitech.net.cn

[E18] 模板占位符替换
来源：http://mz.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://me.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fs.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wo.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://br.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zd.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iq.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ut.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aq.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://wi.chemitech.net.cn

Py:   s.splitlines()
来源：http://bc.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mp.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://xe.521024.cn

TS:   s.split(/\r?\n/)
来源：http://rw.asd995.cn

Java: s.lines().toList()
来源：http://xc.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://zb.wgjwhj.cn

Ruby: s.lines
来源：http://co.yuexingan06.cn

C#:   s.Split('\n')
来源：http://pe.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://rp.nicolike.cn

Py:   if not s:
来源：http://xe.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xj.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yd.muxihuayi.cn

TS:   if (s === "") {}
来源：http://pn.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ms.yuexingan06.cn

Go:   if s == "" {}
来源：http://br.bookmarksfly.cn

Ruby: if s.empty?
来源：http://lj.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gr.asd995.cn

[E21] 超长截断加省略号
来源：http://pr.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fu.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://os.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yr.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ah.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fp.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ow.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jv.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hs.asd995.cn

[E22] 字节长度与字符长度
来源：http://vr.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gh.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tj.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://no.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lb.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://az.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://df.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://xn.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fs.chemitech.net.cn

================================================================================
来源：http://if.muxihuayi.cn

F. 文件与目录
来源：http://vf.bjjhwx.cn

================================================================================
来源：http://ut.huixiangedu.cn

[F01] 读取整个文件
来源：http://nj.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fk.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://lk.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bf.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hq.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jr.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://js.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://wp.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://hn.hahajie.cn

[F02] 逐行读取文件
来源：http://ll.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yk.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vk.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wq.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bl.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gm.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://os.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ey.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fm.colortex.cn

[F03] 写入文件（覆盖）
来源：http://lq.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sk.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kj.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jd.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fb.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uw.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gr.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gn.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://rk.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://co.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oz.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ha.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dw.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zf.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lo.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ii.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iq.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://bo.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lo.asd995.cn

PHP:  file_exists("a.txt");
来源：http://qs.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://he.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://yn.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://si.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://al.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://dz.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://xn.hnjuh.cn

[F06] 删除文件
来源：http://jg.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://od.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://re.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ka.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jv.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pi.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://gv.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://nd.asd995.cn

C#:   File.Delete("a.txt");
来源：http://bj.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://gb.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pk.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ed.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kb.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fn.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ra.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yi.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hn.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ce.muxihuayi.cn

[F08] 遍历目录
来源：http://fd.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://li.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lg.521024.cn

JS:   fs.readdirSync("dir")
来源：http://zh.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://pd.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sm.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dg.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://yt.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://gw.yuexingan06.cn

[F09] 获取文件大小
来源：http://dd.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://nw.colortex.cn

PHP:  filesize("a.txt");
来源：http://mc.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://vd.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://sy.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ss.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gd.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://za.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://dh.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://qp.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://er.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://so.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://zn.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://se.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hs.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://of.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xy.haigaiapp.cn

[F11] 复制与移动文件
来源：http://kt.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ie.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wg.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xw.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://px.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ex.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qu.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yz.newstarts.cn

[F12] CSV 读写
来源：http://uh.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://om.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cz.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ka.shxzukj.cn

TS:   // 同上
来源：http://ny.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hy.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://la.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qf.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://px.yuntaijiaju.cn

================================================================================
来源：http://pq.szxytkj.cn

G. 面向对象
来源：http://tx.gzmigu.cn

================================================================================
来源：http://dx.szxytkj.cn

[G01] 定义类
来源：http://pn.asd995.cn


<!-- 参考信息 -->