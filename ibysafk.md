代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ug.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pm.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://er.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tm.colortex.cn

[E02] 重复字符串
来源：http://vp.huanxung.cn

Py:   "ab" * 3
来源：http://nm.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://bh.szsharing.cn

JS:   "ab".repeat(3)
来源：http://kn.hahajie.cn

TS:   "ab".repeat(3)
来源：http://ps.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://gw.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://is.nicolike.cn

Ruby: "ab" * 3
来源：http://fb.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ti.bookmarksfly.cn

[E03] 截取子串
来源：http://gx.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://np.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oc.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uk.szsharing.cn

TS:   s.slice(1, 4)
来源：http://qc.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://gh.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ct.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zd.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://wq.jctech888.com.cn

[E04] 查找子串位置
来源：http://qy.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://oq.nicolike.cn

PHP:  strpos($s, "x");
来源：http://sm.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pv.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://cs.huixiangedu.cn

Java: s.indexOf("x")
来源：http://qt.colortex.cn

Go:   strings.Index(s, "x")
来源：http://zl.bookmarksfly.cn

Ruby: s.index("x")
来源：http://oe.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://cc.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cx.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ko.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://by.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dx.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xo.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vy.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qd.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sf.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ly.lnxyls.cn

[E06] 替换子串
来源：http://qj.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tf.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://fz.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kv.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://fa.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wf.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mt.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://af.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://ir.panjiajie.cn

[E07] 按分隔符拆分
来源：http://xv.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ct.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xv.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://so.szxytkj.cn

TS:   s.split(",")
来源：http://sh.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://or.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dc.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://mr.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iu.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://bu.asd995.cn

Py:   ",".join(items)
来源：http://er.szxytkj.cn

PHP:  implode(",", $items);
来源：http://mz.newstarts.cn

JS:   items.join(",")
来源：http://nw.panjiajie.cn

TS:   items.join(",")
来源：http://wd.wgjwhj.cn

Java: String.join(",", items)
来源：http://pc.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://qh.bookmarksfly.cn

Ruby: items.join(",")
来源：http://lw.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://oh.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://ph.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xm.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lr.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://py.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://sc.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://fk.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nx.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nz.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oq.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://xp.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gn.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fz.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ga.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://ez.521024.cn

Java: String.format("%03d", 7)
来源：http://gb.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zx.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uu.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qp.panjiajie.cn

[E11] 反转字符串
来源：http://ya.jianghongdianzi.cn

Py:   s[::-1]
来源：http://bq.shxzukj.cn

PHP:  strrev($s);
来源：http://zd.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://bf.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://gx.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xn.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uc.wgjwhj.cn

Ruby: s.reverse
来源：http://hi.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cv.521024.cn

[E12] 统计某字符出现次数
来源：http://ng.asd995.cn

Py:   s.count("a")
来源：http://lk.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://zb.nszjky.cn

JS:   s.split("a").length - 1
来源：http://ie.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://wx.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://go.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ec.jctech888.com.cn

Ruby: s.count("a")
来源：http://og.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://xa.shtwfgs.cn

[E13] 逐字符遍历
来源：http://ss.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://qe.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wg.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://te.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gc.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zk.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qc.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zx.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zj.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://rx.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lr.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ea.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hm.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xa.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ga.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jc.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vi.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aa.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://eb.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tr.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lo.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jv.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ea.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gk.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eq.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wh.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://if.chemitech.net.cn

[E16] 数字千分位
来源：http://ce.huanxung.cn

Py:   f"{1234567:,}"
来源：http://gq.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ks.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hh.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cx.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ld.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yp.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aq.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://wz.gzmigu.cn

[E17] 首字母大写
来源：http://qf.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xr.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lc.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xm.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hi.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ns.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iw.muxihuayi.cn

Ruby: s.capitalize
来源：http://ru.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nb.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://gc.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uc.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yt.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ii.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jk.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cd.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ay.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ig.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vs.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://yc.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://du.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://at.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://nk.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://dv.shtwfgs.cn

Java: s.lines().toList()
来源：http://cg.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://za.gzmigu.cn

Ruby: s.lines
来源：http://gv.9csxet.cn

C#:   s.Split('\n')
来源：http://rj.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://jv.haigaiapp.cn

Py:   if not s:
来源：http://xl.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dn.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fn.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ih.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://yr.gzmigu.cn

Go:   if s == "" {}
来源：http://ka.hnjuh.cn

Ruby: if s.empty?
来源：http://bf.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qb.9csxet.cn

[E21] 超长截断加省略号
来源：http://un.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zh.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lb.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ky.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jq.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ra.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ti.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cp.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sk.nicolike.cn

[E22] 字节长度与字符长度
来源：http://kp.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gf.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xw.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://to.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ow.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ub.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xw.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://mi.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://up.muxihuayi.cn

================================================================================
来源：http://lr.asd995.cn

F. 文件与目录
来源：http://jk.asd995.cn

================================================================================
来源：http://oi.lnxyls.cn

[F01] 读取整个文件
来源：http://hp.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://do.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ro.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sz.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://es.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hg.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://us.9csxet.cn

Ruby: File.read("a.txt")
来源：http://wt.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://ie.bjjhwx.cn

[F02] 逐行读取文件
来源：http://rn.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ay.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gi.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cv.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yq.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nh.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qx.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oa.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gc.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ba.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yc.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://os.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mj.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://td.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rz.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nr.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://uy.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gq.jctech888.com.cn

[F04] 追加写入文件
来源：http://ar.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jj.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://br.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sv.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tu.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eo.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sz.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tl.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kc.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://fl.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://du.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://oj.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://xj.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://ty.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hw.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cx.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://vh.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://oy.jctech888.com.cn

[F06] 删除文件
来源：http://ah.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://bj.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://ge.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://px.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://du.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fe.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://fc.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://hp.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://bs.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://jf.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ah.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://up.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vw.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ou.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fn.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fh.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jg.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oa.shxzskj.cn

[F08] 遍历目录
来源：http://oi.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ut.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aw.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://lr.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://ic.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kq.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://da.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://tn.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://ax.gzmigu.cn

[F09] 获取文件大小
来源：http://kf.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://gc.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://or.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://jh.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://fz.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://or.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oz.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://ub.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://il.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ke.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jl.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wv.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ac.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://sl.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dl.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ph.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oq.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oc.colortex.cn

[F11] 复制与移动文件
来源：http://tv.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kn.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qm.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uo.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cc.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hh.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://by.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mv.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qf.huixinmuqiang.cn

[F12] CSV 读写
来源：http://wn.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ws.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sg.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vg.wgjwhj.cn

TS:   // 同上
来源：http://on.szsharing.cn


<!-- 参考信息 -->