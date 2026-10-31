代发 wailian999

Java: String.join(", ", list)
来源：http://al.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://mg.huanxung.cn

Ruby: arr.join(", ")
来源：http://pc.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://by.nicolike.cn

================================================================================
来源：http://ir.9csxet.cn

E. 字符串处理
来源：http://yt.huanxung.cn

================================================================================
来源：http://zl.gzmigu.cn

[E01] 拼接字符串
来源：http://qi.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://so.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ri.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fp.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fx.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mv.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lb.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://to.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sj.huixinmuqiang.cn

[E02] 重复字符串
来源：http://za.bjjhwx.cn

Py:   "ab" * 3
来源：http://mp.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://zh.nicolike.cn

JS:   "ab".repeat(3)
来源：http://qg.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://bn.shxzskj.cn

Java: "ab".repeat(3)
来源：http://bx.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://iy.asd995.cn

Ruby: "ab" * 3
来源：http://uc.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://de.jianghongdianzi.cn

[E03] 截取子串
来源：http://gb.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ro.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sd.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gi.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://hn.gzmigu.cn

Java: s.substring(1, 4)
来源：http://dc.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jk.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qr.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://op.shxzukj.cn

[E04] 查找子串位置
来源：http://jk.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://iw.colortex.cn

PHP:  strpos($s, "x");
来源：http://vs.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hw.521024.cn

TS:   s.indexOf("x")
来源：http://zl.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ia.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://kk.shtwfgs.cn

Ruby: s.index("x")
来源：http://vm.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ar.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hx.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nl.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fm.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gt.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ys.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wt.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mw.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://js.bookmarksfly.cn

[E06] 替换子串
来源：http://ho.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sw.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://wo.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yr.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://xa.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bw.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nq.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tl.colortex.cn

C#:   s.Replace("a", "b")
来源：http://be.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://oc.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://te.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ma.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mv.hnjuh.cn

TS:   s.split(",")
来源：http://hy.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yu.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bh.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://nl.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ln.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://wz.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://em.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://jx.asd995.cn

JS:   items.join(",")
来源：http://fe.huixiangedu.cn

TS:   items.join(",")
来源：http://nu.nicolike.cn

Java: String.join(",", items)
来源：http://sk.colortex.cn

Go:   strings.Join(items, ",")
来源：http://og.jctech888.com.cn

Ruby: items.join(",")
来源：http://as.gzmigu.cn

C#:   string.Join(",", items)
来源：http://we.newstarts.cn

[E09] 去除所有空白字符
来源：http://cc.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dr.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://te.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://lb.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://to.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://kf.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sb.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mz.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://me.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://yj.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yp.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cd.521024.cn

JS:   "7".padStart(3, "0")
来源：http://bf.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://dk.colortex.cn

Java: String.format("%03d", 7)
来源：http://pr.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://du.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://si.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oo.chemitech.net.cn

[E11] 反转字符串
来源：http://nc.hahajie.cn

Py:   s[::-1]
来源：http://ks.yuexingan06.cn

PHP:  strrev($s);
来源：http://vc.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://sg.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://ah.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nr.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://el.huanxung.cn

Ruby: s.reverse
来源：http://ds.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://me.colortex.cn

[E12] 统计某字符出现次数
来源：http://hv.bookmarksfly.cn

Py:   s.count("a")
来源：http://ev.521024.cn

PHP:  substr_count($s, "a");
来源：http://ci.9csxet.cn

JS:   s.split("a").length - 1
来源：http://em.hahajie.cn

TS:   s.split("a").length - 1
来源：http://pm.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xn.colortex.cn

Go:   strings.Count(s, "a")
来源：http://ds.hnjuh.cn

Ruby: s.count("a")
来源：http://dm.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://sr.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://aq.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://zd.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ct.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ux.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mw.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vt.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tt.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cx.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lq.huanxung.cn

[E14] URL 编码与 Base64
来源：http://hg.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://np.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iu.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uq.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vl.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vg.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pf.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cs.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xd.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://mx.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hw.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gk.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pi.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uu.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vq.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://io.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pd.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kr.hahajie.cn

[E16] 数字千分位
来源：http://hg.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://dl.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://sh.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://to.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://as.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://re.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ob.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wo.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://lc.nicolike.cn

[E17] 首字母大写
来源：http://ro.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fz.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ql.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ff.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ou.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://db.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hv.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ky.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gj.521024.cn

[E18] 模板占位符替换
来源：http://zs.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oa.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ex.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ar.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nd.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fq.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ls.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://au.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mv.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://yy.shxzskj.cn

Py:   s.splitlines()
来源：http://kq.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vo.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://rh.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://tq.bjjhwx.cn

Java: s.lines().toList()
来源：http://od.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://gu.nicolike.cn

Ruby: s.lines
来源：http://wj.muxihuayi.cn

C#:   s.Split('\n')
来源：http://pr.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://nm.gzmigu.cn

Py:   if not s:
来源：http://rv.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hy.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wk.nicolike.cn

TS:   if (s === "") {}
来源：http://yr.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://jp.szsharing.cn

Go:   if s == "" {}
来源：http://ds.haigaiapp.cn

Ruby: if s.empty?
来源：http://bq.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tt.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://yj.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aw.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hg.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wa.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tt.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sj.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jn.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fh.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://qy.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wq.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://er.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pj.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://md.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ps.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ry.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://jo.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xi.chemitech.net.cn

================================================================================
来源：http://ex.hnjuh.cn

F. 文件与目录
来源：http://bd.yuntaijiaju.cn

================================================================================
来源：http://xi.szxytkj.cn

[F01] 读取整个文件
来源：http://ze.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ty.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://nt.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://np.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xv.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eu.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jo.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://xl.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://og.yuexingan06.cn

[F02] 逐行读取文件
来源：http://uq.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yz.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mn.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eg.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zj.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ds.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ac.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lv.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ca.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://dg.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bc.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fk.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://os.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jb.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xa.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bg.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://aa.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jn.muxihuayi.cn

[F04] 追加写入文件
来源：http://rm.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wl.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nu.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gp.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uo.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uj.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zc.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xo.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://ns.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fs.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://cl.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://vp.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://zj.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kr.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fb.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://pj.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ek.bjjhwx.cn

[F06] 删除文件
来源：http://ix.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://kd.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://hj.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vh.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oj.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ah.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://kv.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://xm.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://nn.newstarts.cn

[F07] 创建目录（含多级）
来源：http://eo.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wm.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pb.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ic.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mi.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kk.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gr.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xx.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xe.panjiajie.cn

[F08] 遍历目录
来源：http://ja.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fw.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ec.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://be.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://xi.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yr.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wk.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://jt.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://yw.nicolike.cn

[F09] 获取文件大小
来源：http://yo.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://cc.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://jc.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://xk.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://rt.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://te.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vo.colortex.cn

Ruby: File.size("a.txt")
来源：http://ow.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://zf.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ye.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://th.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ng.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ae.szsharing.cn

TS:   path.extname("a.txt")
来源：http://hn.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qs.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ry.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kn.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ww.lnxyls.cn

[F11] 复制与移动文件
来源：http://lp.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yz.asd995.cn


<!-- 参考信息 -->