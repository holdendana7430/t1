代发 wailian999

Java: String.join(", ", list)
来源：http://nv.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://en.panjiajie.cn

Ruby: arr.join(", ")
来源：http://kt.nszjky.cn

C#:   string.Join(", ", list)
来源：http://mn.bjjhwx.cn

================================================================================
来源：http://vu.hnjuh.cn

E. 字符串处理
来源：http://ir.shtwfgs.cn

================================================================================
来源：http://fs.hnjuh.cn

[E01] 拼接字符串
来源：http://ax.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vk.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://om.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kb.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lg.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tb.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nt.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ik.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nd.shxzukj.cn

[E02] 重复字符串
来源：http://zn.asd995.cn

Py:   "ab" * 3
来源：http://ny.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://io.colortex.cn

JS:   "ab".repeat(3)
来源：http://rm.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://kz.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://lh.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://fm.asd995.cn

Ruby: "ab" * 3
来源：http://nw.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gk.shxzukj.cn

[E03] 截取子串
来源：http://fs.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dm.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tg.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bi.nszjky.cn

TS:   s.slice(1, 4)
来源：http://me.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://dy.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zv.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ok.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://qf.newstarts.cn

[E04] 查找子串位置
来源：http://kj.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://rr.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://ih.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ie.asd995.cn

TS:   s.indexOf("x")
来源：http://zu.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://vo.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://ey.shxzskj.cn

Ruby: s.index("x")
来源：http://tw.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://wt.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uu.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ai.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gs.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kh.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://od.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wz.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://le.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kk.colortex.cn

[E06] 替换子串
来源：http://ul.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gg.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://xj.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ab.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://zt.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://od.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://af.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://an.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://qp.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://cs.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vi.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fa.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tp.wgjwhj.cn

TS:   s.split(",")
来源：http://zl.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gt.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ti.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://fb.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cl.521024.cn

[E08] 数组按分隔符合并
来源：http://vz.huixiangedu.cn

Py:   ",".join(items)
来源：http://so.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://tz.shxzskj.cn

JS:   items.join(",")
来源：http://qo.shtwfgs.cn

TS:   items.join(",")
来源：http://ug.panjiajie.cn

Java: String.join(",", items)
来源：http://ot.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://pf.hahajie.cn

Ruby: items.join(",")
来源：http://cv.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://vw.gzmigu.cn

[E09] 去除所有空白字符
来源：http://hj.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://er.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qn.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://xj.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://kf.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ad.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fz.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bl.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zs.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://xq.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://np.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mx.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://bd.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://si.nszjky.cn

Java: String.format("%03d", 7)
来源：http://yc.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mn.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://as.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://be.lnxyls.cn

[E11] 反转字符串
来源：http://vg.huanxung.cn

Py:   s[::-1]
来源：http://do.shtwfgs.cn

PHP:  strrev($s);
来源：http://zx.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://dw.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://by.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ua.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ei.bookmarksfly.cn

Ruby: s.reverse
来源：http://fg.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yp.hahajie.cn

[E12] 统计某字符出现次数
来源：http://yj.chemitech.net.cn

Py:   s.count("a")
来源：http://ca.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://as.9csxet.cn

JS:   s.split("a").length - 1
来源：http://ea.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://nt.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yu.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://ut.shxzukj.cn

Ruby: s.count("a")
来源：http://ue.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://zx.shxzskj.cn

[E13] 逐字符遍历
来源：http://lh.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://po.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gg.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jv.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ix.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vr.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ib.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cf.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yn.szsharing.cn

[E14] URL 编码与 Base64
来源：http://ew.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qx.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hp.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wh.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gb.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vz.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fq.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rt.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xu.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://px.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iv.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://da.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zb.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://br.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lq.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lp.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ut.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bh.bjjhwx.cn

[E16] 数字千分位
来源：http://bw.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://hx.shxzskj.cn

PHP:  number_format(1234567);
来源：http://nx.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dg.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pu.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ja.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qe.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ti.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://aa.shxzskj.cn

[E17] 首字母大写
来源：http://cz.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://un.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xx.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://za.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://va.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wv.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qw.huixiangedu.cn

Ruby: s.capitalize
来源：http://hl.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://au.shtwfgs.cn

[E18] 模板占位符替换
来源：http://cy.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ge.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jr.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ay.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://an.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://er.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ub.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vi.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ol.9csxet.cn

[E19] 多行文本按行拆分
来源：http://jr.haigaiapp.cn

Py:   s.splitlines()
来源：http://es.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lx.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://oo.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://pq.nszjky.cn

Java: s.lines().toList()
来源：http://wb.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://bf.newstarts.cn

Ruby: s.lines
来源：http://zo.huanxung.cn

C#:   s.Split('\n')
来源：http://qi.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://qu.jctech888.com.cn

Py:   if not s:
来源：http://xb.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yh.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ot.szsharing.cn

TS:   if (s === "") {}
来源：http://kx.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://gp.lnxyls.cn

Go:   if s == "" {}
来源：http://vm.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://ex.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ud.nicolike.cn

[E21] 超长截断加省略号
来源：http://ck.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tz.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rg.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xw.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xv.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://iw.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vz.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://he.newstarts.cn

[E22] 字节长度与字符长度
来源：http://fi.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vp.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lj.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vh.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tx.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://so.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ak.lnxyls.cn

================================================================================
来源：http://nn.colortex.cn

F. 文件与目录
来源：http://ka.lnxyls.cn

================================================================================
来源：http://kw.shxzukj.cn

[F01] 读取整个文件
来源：http://pd.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cp.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://cu.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pz.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://db.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bz.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ya.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://vn.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ki.521024.cn

[F02] 逐行读取文件
来源：http://rm.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rf.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wu.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yi.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uc.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zf.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xc.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ub.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gg.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://ao.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oi.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nk.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bo.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nk.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ut.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ra.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://qq.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://do.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://vr.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zo.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ru.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dr.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iy.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ql.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ps.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tr.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ny.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://fe.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yk.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://uq.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://nh.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://iq.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tj.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cs.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://yn.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ou.hahajie.cn

[F06] 删除文件
来源：http://sk.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://bx.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://rz.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vy.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sr.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ja.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ec.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://zz.asd995.cn

C#:   File.Delete("a.txt");
来源：http://ue.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://er.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uu.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aq.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lx.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jc.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lp.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://is.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kz.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wp.jctech888.com.cn

[F08] 遍历目录
来源：http://js.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mp.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gv.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://as.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://mk.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rm.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bm.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://tw.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://mr.haigaiapp.cn

[F09] 获取文件大小
来源：http://ub.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ga.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://zt.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://yc.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://iu.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kc.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tu.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://uf.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://cc.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://uh.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pj.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pf.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lp.szsharing.cn

TS:   path.extname("a.txt")
来源：http://xz.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wm.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ei.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fq.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://as.nszjky.cn

[F11] 复制与移动文件
来源：http://av.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uo.yuntaijiaju.cn


<!-- 参考信息 -->