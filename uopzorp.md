代发 wailian999

TS:   "ab".repeat(3)
来源：http://mc.szxytkj.cn

Java: "ab".repeat(3)
来源：http://cr.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://wh.muxihuayi.cn

Ruby: "ab" * 3
来源：http://tp.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zy.huixiangedu.cn

[E03] 截取子串
来源：http://dq.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vy.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pj.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hw.huanxung.cn

TS:   s.slice(1, 4)
来源：http://cg.asd995.cn

Java: s.substring(1, 4)
来源：http://iq.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ok.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vs.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://hy.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ug.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://cr.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://fr.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://od.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://pe.shxzskj.cn

Java: s.indexOf("x")
来源：http://pf.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://cq.nicolike.cn

Ruby: s.index("x")
来源：http://hz.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://ff.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qj.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://so.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pg.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sb.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://os.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dd.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tr.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wr.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://we.nicolike.cn

[E06] 替换子串
来源：http://kt.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://al.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://sv.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qk.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://wz.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xg.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hp.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://af.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://gl.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://wy.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ar.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nr.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qn.yuexingan06.cn

TS:   s.split(",")
来源：http://ad.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eh.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ck.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://yk.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vn.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://dj.huanxung.cn

Py:   ",".join(items)
来源：http://gn.asd995.cn

PHP:  implode(",", $items);
来源：http://vi.panjiajie.cn

JS:   items.join(",")
来源：http://gn.panjiajie.cn

TS:   items.join(",")
来源：http://nh.newstarts.cn

Java: String.join(",", items)
来源：http://eo.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://cz.wgjwhj.cn

Ruby: items.join(",")
来源：http://dx.lnxyls.cn

C#:   string.Join(",", items)
来源：http://qh.szsharing.cn

[E09] 去除所有空白字符
来源：http://va.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fk.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gq.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://dc.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://dc.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://xd.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pm.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fs.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lb.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://qz.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ty.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cp.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://rn.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://je.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://wq.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cb.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://db.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uu.jctech888.com.cn

[E11] 反转字符串
来源：http://uc.lnxyls.cn

Py:   s[::-1]
来源：http://wm.hahajie.cn

PHP:  strrev($s);
来源：http://tr.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://lb.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ar.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qx.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wo.nszjky.cn

Ruby: s.reverse
来源：http://ez.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kn.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://xr.bookmarksfly.cn

Py:   s.count("a")
来源：http://sk.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://nx.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://fs.9csxet.cn

TS:   s.split("a").length - 1
来源：http://ro.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fr.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://vr.shxzukj.cn

Ruby: s.count("a")
来源：http://ve.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://yy.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://we.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://kl.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fm.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xg.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lj.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wy.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://be.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pw.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rh.newstarts.cn

[E14] URL 编码与 Base64
来源：http://jm.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tw.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qz.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lx.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://km.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yc.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ri.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vp.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lt.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://fe.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ig.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ck.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yp.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pu.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uo.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tk.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xf.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ko.huixiangedu.cn

[E16] 数字千分位
来源：http://dd.nszjky.cn

Py:   f"{1234567:,}"
来源：http://lf.shxzukj.cn

PHP:  number_format(1234567);
来源：http://wm.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fc.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zp.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dd.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vd.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ag.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://bg.huanxung.cn

[E17] 首字母大写
来源：http://ip.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://on.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kj.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eo.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jf.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tw.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://by.huixiangedu.cn

Ruby: s.capitalize
来源：http://fy.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ta.chemitech.net.cn

[E18] 模板占位符替换
来源：http://kq.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kw.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ej.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ty.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hh.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lx.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ns.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qw.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vn.hahajie.cn

[E19] 多行文本按行拆分
来源：http://bt.panjiajie.cn

Py:   s.splitlines()
来源：http://ky.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yd.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://ta.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://cb.colortex.cn

Java: s.lines().toList()
来源：http://wp.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://zb.asd995.cn

Ruby: s.lines
来源：http://hn.haigaiapp.cn

C#:   s.Split('\n')
来源：http://xk.nicolike.cn

[E20] 判断字符串是否为空
来源：http://iw.gzmigu.cn

Py:   if not s:
来源：http://rd.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kx.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jp.huixiangedu.cn

TS:   if (s === "") {}
来源：http://xx.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://db.huanxung.cn

Go:   if s == "" {}
来源：http://du.lnxyls.cn

Ruby: if s.empty?
来源：http://dm.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ou.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://wj.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://za.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ny.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pu.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://al.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wy.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://lt.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nv.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dj.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://no.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nq.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qs.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tm.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://el.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qv.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fn.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://su.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uf.hnjuh.cn

================================================================================
来源：http://pu.haigaiapp.cn

F. 文件与目录
来源：http://nb.asd995.cn

================================================================================
来源：http://ud.nszjky.cn

[F01] 读取整个文件
来源：http://vi.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wd.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://xp.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ta.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qy.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zl.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://co.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://xn.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://mi.szsharing.cn

[F02] 逐行读取文件
来源：http://by.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kj.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rc.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://et.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wz.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qw.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://or.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ul.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jp.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://ai.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mt.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mo.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lr.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jo.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wp.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://en.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://tv.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xf.521024.cn

[F04] 追加写入文件
来源：http://hh.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rh.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lk.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://um.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rc.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ea.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zj.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mi.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iy.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://gl.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xp.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://je.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ar.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://dw.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ei.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dq.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://gy.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://uo.lnxyls.cn

[F06] 删除文件
来源：http://sx.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://mc.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://nb.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://es.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mo.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mq.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://pw.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://oo.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://wq.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://xx.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wi.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://on.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sc.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wx.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hr.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uh.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wp.wgjwhj.cn

[F08] 遍历目录
来源：http://tn.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uj.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gw.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://bn.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ig.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://si.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jf.asd995.cn

Ruby: Dir.children("dir")
来源：http://ty.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://kw.bookmarksfly.cn

[F09] 获取文件大小
来源：http://bc.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ca.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://ch.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://qk.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://hz.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pp.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hf.asd995.cn

Ruby: File.size("a.txt")
来源：http://rk.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://bo.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lz.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mm.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nt.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xh.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://eo.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://do.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hr.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wm.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wx.jctech888.com.cn

[F11] 复制与移动文件
来源：http://xk.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rj.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pz.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dz.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bm.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bw.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zm.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://da.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yl.hahajie.cn

[F12] CSV 读写
来源：http://fb.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xx.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sd.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nu.hnjuh.cn

TS:   // 同上
来源：http://mp.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zq.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dl.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lx.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gb.yuntaijiaju.cn

================================================================================
来源：http://gl.muxihuayi.cn

G. 面向对象
来源：http://qo.chemitech.net.cn

================================================================================
来源：http://ev.bjjhwx.cn

[G01] 定义类
来源：http://ua.gzmigu.cn


<!-- 参考信息 -->