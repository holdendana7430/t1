代发 wailian999

Java: String.join(", ", list)
来源：http://fu.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://be.9csxet.cn

Ruby: arr.join(", ")
来源：http://qg.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://cc.muxihuayi.cn

================================================================================
来源：http://vi.yuntaijiaju.cn

E. 字符串处理
来源：http://cy.jctech888.com.cn

================================================================================
来源：http://mx.chemitech.net.cn

[E01] 拼接字符串
来源：http://dz.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yp.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ot.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ul.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://at.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uw.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yy.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fx.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mf.huanxung.cn

[E02] 重复字符串
来源：http://pu.jctech888.com.cn

Py:   "ab" * 3
来源：http://zs.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://vk.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://db.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://ma.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://wm.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://if.9csxet.cn

Ruby: "ab" * 3
来源：http://so.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nt.muxihuayi.cn

[E03] 截取子串
来源：http://qm.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ez.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aq.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jn.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://ze.asd995.cn

Java: s.substring(1, 4)
来源：http://vw.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mn.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cb.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://xj.haigaiapp.cn

[E04] 查找子串位置
来源：http://jq.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://bp.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://bs.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tt.9csxet.cn

TS:   s.indexOf("x")
来源：http://bl.hahajie.cn

Java: s.indexOf("x")
来源：http://hq.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://zz.jctech888.com.cn

Ruby: s.index("x")
来源：http://bc.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://au.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sb.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gm.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hy.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uu.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cz.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://te.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dr.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rw.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rq.hahajie.cn

[E06] 替换子串
来源：http://ja.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ay.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://zw.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yk.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://cv.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ze.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wz.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ds.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://lw.9csxet.cn

[E07] 按分隔符拆分
来源：http://jv.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kj.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fg.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uo.lnxyls.cn

TS:   s.split(",")
来源：http://mf.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qk.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kd.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://rh.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bh.521024.cn

[E08] 数组按分隔符合并
来源：http://vu.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://uh.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://qe.shtwfgs.cn

JS:   items.join(",")
来源：http://ug.wgjwhj.cn

TS:   items.join(",")
来源：http://ur.bjjhwx.cn

Java: String.join(",", items)
来源：http://ye.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://tj.muxihuayi.cn

Ruby: items.join(",")
来源：http://iv.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://be.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://ns.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://te.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cn.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://zk.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ah.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://zf.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eg.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ga.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oy.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://gd.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ls.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ev.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://cb.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://yx.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://lq.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jc.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jk.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nl.9csxet.cn

[E11] 反转字符串
来源：http://zg.9csxet.cn

Py:   s[::-1]
来源：http://im.nicolike.cn

PHP:  strrev($s);
来源：http://rt.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://jq.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://tp.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bh.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hs.bookmarksfly.cn

Ruby: s.reverse
来源：http://ox.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xo.huanxung.cn

[E12] 统计某字符出现次数
来源：http://np.muxihuayi.cn

Py:   s.count("a")
来源：http://ts.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://ls.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://ab.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ti.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pn.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://ko.colortex.cn

Ruby: s.count("a")
来源：http://lu.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://qu.shxzskj.cn

[E13] 逐字符遍历
来源：http://gy.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://zq.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://do.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xt.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ru.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sd.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fj.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ov.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cq.9csxet.cn

[E14] URL 编码与 Base64
来源：http://ef.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ag.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bc.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nd.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yj.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aa.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ot.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wy.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lf.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://yt.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ka.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hx.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lz.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wp.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yz.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zq.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mm.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ar.szxytkj.cn

[E16] 数字千分位
来源：http://eg.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://ym.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://lo.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://us.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iu.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xk.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ns.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://um.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://jn.muxihuayi.cn

[E17] 首字母大写
来源：http://ql.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kd.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xh.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zd.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fb.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cd.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bu.szxytkj.cn

Ruby: s.capitalize
来源：http://rc.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ug.shxzskj.cn

[E18] 模板占位符替换
来源：http://yz.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dz.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gb.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ga.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://af.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://in.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dh.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xl.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qa.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://ov.huixiangedu.cn

Py:   s.splitlines()
来源：http://eo.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ve.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ld.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://vv.asd995.cn

Java: s.lines().toList()
来源：http://jb.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://hs.lnxyls.cn

Ruby: s.lines
来源：http://qn.9csxet.cn

C#:   s.Split('\n')
来源：http://iv.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://kz.szxytkj.cn

Py:   if not s:
来源：http://tx.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wr.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fq.nszjky.cn

TS:   if (s === "") {}
来源：http://iy.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://yh.nicolike.cn

Go:   if s == "" {}
来源：http://qg.muxihuayi.cn

Ruby: if s.empty?
来源：http://cp.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tg.szsharing.cn

[E21] 超长截断加省略号
来源：http://vw.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qs.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mr.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ee.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fc.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cl.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://zh.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://le.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fk.9csxet.cn

[E22] 字节长度与字符长度
来源：http://lq.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wu.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uq.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uq.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gq.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ck.521024.cn

Ruby: s.bytesize;  s.length
来源：http://up.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zh.lnxyls.cn

================================================================================
来源：http://ti.nszjky.cn

F. 文件与目录
来源：http://nl.nicolike.cn

================================================================================
来源：http://vz.muxihuayi.cn

[F01] 读取整个文件
来源：http://kp.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fz.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://ef.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://es.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vb.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ob.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ur.521024.cn

Ruby: File.read("a.txt")
来源：http://pl.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://cc.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://gt.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nb.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jb.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xb.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sl.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://js.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oc.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://no.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hp.521024.cn

[F03] 写入文件（覆盖）
来源：http://vc.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uy.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://on.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jj.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vf.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fv.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ku.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://jb.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uq.shxzukj.cn

[F04] 追加写入文件
来源：http://qv.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fx.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ah.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sr.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://op.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dk.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ry.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gn.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://zl.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://bn.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://lt.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ov.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ou.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gk.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://fi.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://ix.yuntaijiaju.cn

[F06] 删除文件
来源：http://hs.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://jw.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://iq.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ll.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ld.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pm.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://il.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://mp.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ng.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://sb.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ql.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ir.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ip.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ov.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tx.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ur.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gh.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lt.szsharing.cn

[F08] 遍历目录
来源：http://yh.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kd.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xh.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://jp.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://uw.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pn.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sl.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://mo.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ui.chemitech.net.cn

[F09] 获取文件大小
来源：http://gd.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ta.hahajie.cn

PHP:  filesize("a.txt");
来源：http://xy.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://fw.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://zl.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fq.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pt.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://ou.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://se.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://bl.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jd.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://au.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cf.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://wu.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wg.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ez.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jz.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://od.panjiajie.cn

[F11] 复制与移动文件
来源：http://va.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wl.hnjuh.cn


<!-- 参考信息 -->