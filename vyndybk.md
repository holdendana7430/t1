代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://md.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://qs.lnxyls.cn

JS:   arr.join(", ")
来源：http://ww.gzmigu.cn

TS:   arr.join(", ")
来源：http://ww.9csxet.cn

Java: String.join(", ", list)
来源：http://vo.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://ou.asd995.cn

Ruby: arr.join(", ")
来源：http://xr.521024.cn

C#:   string.Join(", ", list)
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://do.szxytkj.cn

E. 字符串处理
来源：http://ib.jianghongdianzi.cn

================================================================================
来源：http://sg.hnjuh.cn

[E01] 拼接字符串
来源：http://tu.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dv.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rf.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iu.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ya.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://me.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cm.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fu.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oi.bjjhwx.cn

[E02] 重复字符串
来源：http://po.colortex.cn

Py:   "ab" * 3
来源：http://zq.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://nt.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://pa.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://ax.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://rt.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://cu.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://je.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nv.muxihuayi.cn

[E03] 截取子串
来源：http://tp.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hy.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nt.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iq.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://py.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://rs.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dy.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ba.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ar.huanxung.cn

[E04] 查找子串位置
来源：http://wj.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ui.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://ta.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ta.gzmigu.cn

TS:   s.indexOf("x")
来源：http://dn.lnxyls.cn

Java: s.indexOf("x")
来源：http://eu.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://uw.jctech888.com.cn

Ruby: s.index("x")
来源：http://ba.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://lo.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xg.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zn.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bz.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://td.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hg.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fa.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://im.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fz.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dv.shxzskj.cn

[E06] 替换子串
来源：http://ts.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://le.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://id.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zs.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://vj.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lg.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://og.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ei.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://hu.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://hw.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uy.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qq.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ph.newstarts.cn

TS:   s.split(",")
来源：http://vk.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lm.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zp.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://eq.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sp.huanxung.cn

[E08] 数组按分隔符合并
来源：http://dp.chemitech.net.cn

Py:   ",".join(items)
来源：http://gs.521024.cn

PHP:  implode(",", $items);
来源：http://bl.panjiajie.cn

JS:   items.join(",")
来源：http://bn.gzmigu.cn

TS:   items.join(",")
来源：http://ge.yuexingan06.cn

Java: String.join(",", items)
来源：http://oi.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://dx.asd995.cn

Ruby: items.join(",")
来源：http://fh.szsharing.cn

C#:   string.Join(",", items)
来源：http://gf.9csxet.cn

[E09] 去除所有空白字符
来源：http://vv.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gh.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cb.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ws.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://jg.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://me.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kb.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qz.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bv.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://xn.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gm.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ns.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ti.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ij.asd995.cn

Java: String.format("%03d", 7)
来源：http://ug.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hy.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gd.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://da.nszjky.cn

[E11] 反转字符串
来源：http://hi.yuntaijiaju.cn

Py:   s[::-1]
来源：http://bd.bookmarksfly.cn

PHP:  strrev($s);
来源：http://pv.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://oo.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://sz.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cl.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dr.nicolike.cn

Ruby: s.reverse
来源：http://vv.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vk.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://af.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ki.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://fp.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ld.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ti.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sx.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://ss.hahajie.cn

Ruby: s.count("a")
来源：http://gz.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://kq.newstarts.cn

[E13] 逐字符遍历
来源：http://ww.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://bi.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cw.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gx.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qd.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://um.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ve.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vv.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://js.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://zm.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ps.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rk.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mj.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xn.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ky.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wf.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://or.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gs.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://xh.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cp.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ex.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ds.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vw.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bf.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fz.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://it.huanxung.cn

[E16] 数字千分位
来源：http://qq.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://we.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://zu.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://el.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://am.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cj.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ek.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ta.colortex.cn

C#:   1234567.ToString("N0")
来源：http://ia.yuntaijiaju.cn

[E17] 首字母大写
来源：http://zb.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fm.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ge.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kx.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vk.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://du.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pv.huanxung.cn

Ruby: s.capitalize
来源：http://kt.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://af.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://fb.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sm.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zz.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lx.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lw.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fk.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kg.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cb.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bz.asd995.cn

[E19] 多行文本按行拆分
来源：http://jt.huixiangedu.cn

Py:   s.splitlines()
来源：http://tu.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hk.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://cv.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://nc.chemitech.net.cn

Java: s.lines().toList()
来源：http://ts.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ez.szsharing.cn

Ruby: s.lines
来源：http://ol.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ib.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://pm.shxzukj.cn

Py:   if not s:
来源：http://al.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sy.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://je.muxihuayi.cn

TS:   if (s === "") {}
来源：http://tq.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://zn.huixiangedu.cn

Go:   if s == "" {}
来源：http://tn.lnxyls.cn

Ruby: if s.empty?
来源：http://xu.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rq.newstarts.cn

[E21] 超长截断加省略号
来源：http://rn.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yd.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ib.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fx.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qf.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oy.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nj.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ll.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://id.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://jr.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mn.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://be.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ur.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ul.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sz.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://vb.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://db.shtwfgs.cn

================================================================================
来源：http://xf.szxytkj.cn

F. 文件与目录
来源：http://zd.haigaiapp.cn

================================================================================
来源：http://sc.chemitech.net.cn

[F01] 读取整个文件
来源：http://mj.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ax.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://wr.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vd.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jk.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zh.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://af.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://dh.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://xm.gzmigu.cn

[F02] 逐行读取文件
来源：http://zp.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ux.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ys.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dq.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ff.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xo.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kh.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wq.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zp.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://kn.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xh.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wx.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lk.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zq.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://og.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gr.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://zg.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://su.hahajie.cn

[F04] 追加写入文件
来源：http://id.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ic.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ih.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cb.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ft.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xp.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bm.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wf.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vo.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ac.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xz.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://jq.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://zv.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://ek.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sy.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eo.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://sd.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://fg.nszjky.cn

[F06] 删除文件
来源：http://pq.nszjky.cn

Py:   os.remove("a.txt")
来源：http://qv.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://qu.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tw.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fc.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vr.521024.cn

Go:   os.Remove("a.txt")
来源：http://hf.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://lu.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://fz.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://hd.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lm.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sh.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://le.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ot.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uu.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ri.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pk.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dl.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ff.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lr.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ib.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://zi.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://lr.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aa.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hm.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://ct.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://hn.shtwfgs.cn

[F09] 获取文件大小
来源：http://ee.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://nn.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://zg.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://kk.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://dz.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rt.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bs.newstarts.cn

Ruby: File.size("a.txt")
来源：http://mq.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ix.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://pg.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cb.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dz.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://al.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://py.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ob.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hg.nicolike.cn


<!-- 参考信息 -->