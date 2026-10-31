代发 wailian999

[E02] 重复字符串
来源：http://lh.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ic.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://dv.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://uc.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://fu.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://lz.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://es.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ef.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wy.haigaiapp.cn

[E03] 截取子串
来源：http://au.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zp.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ti.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jj.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://gx.panjiajie.cn

Java: s.substring(1, 4)
来源：http://nh.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ce.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jo.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ah.newstarts.cn

[E04] 查找子串位置
来源：http://gu.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://cx.szsharing.cn

PHP:  strpos($s, "x");
来源：http://rd.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zq.lnxyls.cn

TS:   s.indexOf("x")
来源：http://on.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ub.colortex.cn

Go:   strings.Index(s, "x")
来源：http://fk.haigaiapp.cn

Ruby: s.index("x")
来源：http://ml.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://cc.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xz.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ie.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qy.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pj.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qz.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gt.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pb.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ul.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ge.shxzskj.cn

[E06] 替换子串
来源：http://dj.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pz.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ha.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tc.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://gp.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ew.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kr.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jl.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://fp.gzmigu.cn

[E07] 按分隔符拆分
来源：http://wk.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ij.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rr.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wa.huixiangedu.cn

TS:   s.split(",")
来源：http://oe.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vy.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vn.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://fi.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rf.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ic.colortex.cn

Py:   ",".join(items)
来源：http://gh.9csxet.cn

PHP:  implode(",", $items);
来源：http://lm.521024.cn

JS:   items.join(",")
来源：http://op.nszjky.cn

TS:   items.join(",")
来源：http://mp.lnxyls.cn

Java: String.join(",", items)
来源：http://xj.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://xy.jctech888.com.cn

Ruby: items.join(",")
来源：http://jm.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://nm.huanxung.cn

[E09] 去除所有空白字符
来源：http://oj.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vt.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://al.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://gr.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://od.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://xd.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ma.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jj.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bg.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://hg.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pz.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ro.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://kd.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://fd.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://ma.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jb.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sk.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bv.chemitech.net.cn

[E11] 反转字符串
来源：http://be.bookmarksfly.cn

Py:   s[::-1]
来源：http://ai.szsharing.cn

PHP:  strrev($s);
来源：http://wu.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://lf.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://jx.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zc.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ub.muxihuayi.cn

Ruby: s.reverse
来源：http://zs.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gq.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://gy.haigaiapp.cn

Py:   s.count("a")
来源：http://xa.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ah.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://bk.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://xr.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ch.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://kb.huanxung.cn

Ruby: s.count("a")
来源：http://ux.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ph.szsharing.cn

[E13] 逐字符遍历
来源：http://pz.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://nf.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aj.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ek.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yi.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gf.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://af.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tn.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lb.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://yg.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sr.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xb.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fm.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://im.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ns.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ep.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zp.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lk.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://bk.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rq.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xh.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ot.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iz.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://an.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sr.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://li.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xx.szsharing.cn

[E16] 数字千分位
来源：http://ji.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://jo.gzmigu.cn

PHP:  number_format(1234567);
来源：http://wl.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://er.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gg.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ju.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://op.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://az.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ib.muxihuayi.cn

[E17] 首字母大写
来源：http://js.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ao.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gh.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uh.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jz.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rw.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aj.bjjhwx.cn

Ruby: s.capitalize
来源：http://zl.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qv.shxzukj.cn

[E18] 模板占位符替换
来源：http://yy.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hr.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vp.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mx.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rx.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ne.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ng.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yy.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lt.nicolike.cn

[E19] 多行文本按行拆分
来源：http://mg.huixiangedu.cn

Py:   s.splitlines()
来源：http://dx.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pt.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://qx.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://lh.hnjuh.cn

Java: s.lines().toList()
来源：http://dt.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://sw.hnjuh.cn

Ruby: s.lines
来源：http://fw.newstarts.cn

C#:   s.Split('\n')
来源：http://nk.newstarts.cn

[E20] 判断字符串是否为空
来源：http://iq.nicolike.cn

Py:   if not s:
来源：http://xu.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ov.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ti.nszjky.cn

TS:   if (s === "") {}
来源：http://wj.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://el.huanxung.cn

Go:   if s == "" {}
来源：http://nf.9csxet.cn

Ruby: if s.empty?
来源：http://kn.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://do.521024.cn

[E21] 超长截断加省略号
来源：http://ob.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ye.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yx.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pe.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://os.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://ia.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zr.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yn.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://at.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ry.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yu.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qq.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hq.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kx.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sj.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ud.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ys.szxytkj.cn

================================================================================
来源：http://lr.huixiangedu.cn

F. 文件与目录
来源：http://le.hnjuh.cn

================================================================================
来源：http://cg.bookmarksfly.cn

[F01] 读取整个文件
来源：http://sp.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ad.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://up.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fd.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ok.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hy.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wn.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://tp.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://et.shxzukj.cn

[F02] 逐行读取文件
来源：http://qi.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jy.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vg.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dz.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fk.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cl.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aw.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lw.colortex.cn

[F03] 写入文件（覆盖）
来源：http://kz.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vb.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bw.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jw.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jm.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hx.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oc.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://qs.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mu.newstarts.cn

[F04] 追加写入文件
来源：http://fm.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ax.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hu.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qm.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rl.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dt.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zu.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ep.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wb.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://ig.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lf.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://bb.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://tf.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://nm.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yb.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rt.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://xq.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://du.jctech888.com.cn

[F06] 删除文件
来源：http://vp.asd995.cn

Py:   os.remove("a.txt")
来源：http://wb.newstarts.cn

PHP:  unlink("a.txt");
来源：http://tm.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ie.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jv.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://li.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://lk.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://jy.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://je.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://vj.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uy.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ab.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wh.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uw.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pi.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nj.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aw.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pi.bjjhwx.cn

[F08] 遍历目录
来源：http://fu.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://to.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://og.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://mc.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://qk.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yq.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bv.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://ue.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://pw.colortex.cn

[F09] 获取文件大小
来源：http://wy.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://yu.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://vt.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://vl.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://rk.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oe.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zj.9csxet.cn

Ruby: File.size("a.txt")
来源：http://ac.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://jl.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://nt.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cq.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ow.9csxet.cn

TS:   path.extname("a.txt")
来源：http://eu.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ip.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://an.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ec.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pj.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://rj.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nw.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://js.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tb.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ch.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vx.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tz.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sl.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fd.bookmarksfly.cn

[F12] CSV 读写
来源：http://uw.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://it.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cs.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uq.szxytkj.cn

TS:   // 同上
来源：http://ap.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ne.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hp.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eo.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kd.wgjwhj.cn


<!-- 参考信息 -->