代发 wailian999

================================================================================
来源：http://je.521024.cn

E. 字符串处理
来源：http://zm.shxzukj.cn

================================================================================
来源：http://de.colortex.cn

[E01] 拼接字符串
来源：http://br.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://br.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fd.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gp.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jn.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pj.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gr.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qa.colortex.cn

[E02] 重复字符串
来源：http://kn.muxihuayi.cn

Py:   "ab" * 3
来源：http://io.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://vj.huanxung.cn

JS:   "ab".repeat(3)
来源：http://rr.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://pv.lnxyls.cn

Java: "ab".repeat(3)
来源：http://py.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://zd.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://ed.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rc.wgjwhj.cn

[E03] 截取子串
来源：http://lr.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pd.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ds.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://td.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://vv.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://hu.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yi.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kj.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://ya.huixiangedu.cn

[E04] 查找子串位置
来源：http://rv.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://yv.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://si.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ow.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://wt.shxzskj.cn

Java: s.indexOf("x")
来源：http://pg.colortex.cn

Go:   strings.Index(s, "x")
来源：http://vd.haigaiapp.cn

Ruby: s.index("x")
来源：http://vq.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://uy.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lj.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kc.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lg.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zc.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cu.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yu.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eh.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cb.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oa.huixiangedu.cn

[E06] 替换子串
来源：http://ik.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rx.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://zi.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yg.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://by.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rq.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jt.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dm.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://gd.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://no.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gv.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aq.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://un.bookmarksfly.cn

TS:   s.split(",")
来源：http://jx.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pn.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gd.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://ua.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yn.szsharing.cn

[E08] 数组按分隔符合并
来源：http://jl.lnxyls.cn

Py:   ",".join(items)
来源：http://rq.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://fl.shtwfgs.cn

JS:   items.join(",")
来源：http://iq.shxzskj.cn

TS:   items.join(",")
来源：http://zl.wgjwhj.cn

Java: String.join(",", items)
来源：http://rk.colortex.cn

Go:   strings.Join(items, ",")
来源：http://rf.szxytkj.cn

Ruby: items.join(",")
来源：http://uw.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ey.hnjuh.cn

[E09] 去除所有空白字符
来源：http://zr.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hy.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xi.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://fj.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://nf.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://np.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zl.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nx.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gm.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://xc.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dg.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vr.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://zt.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://oj.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://ma.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bp.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dt.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bh.wgjwhj.cn

[E11] 反转字符串
来源：http://rx.shxzskj.cn

Py:   s[::-1]
来源：http://ok.gzmigu.cn

PHP:  strrev($s);
来源：http://tx.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ho.521024.cn

TS:   [...s].reverse().join("")
来源：http://gn.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zc.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://du.nszjky.cn

Ruby: s.reverse
来源：http://nx.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ut.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://rt.huanxung.cn

Py:   s.count("a")
来源：http://eb.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://ck.521024.cn

JS:   s.split("a").length - 1
来源：http://rb.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://pb.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dd.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://zn.bookmarksfly.cn

Ruby: s.count("a")
来源：http://hl.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://rm.szsharing.cn

[E13] 逐字符遍历
来源：http://wh.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://cw.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bg.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://si.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sc.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fu.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jb.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ic.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cu.asd995.cn

[E14] URL 编码与 Base64
来源：http://ih.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dx.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bp.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://in.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ke.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ut.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://us.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lm.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oo.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://fz.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gy.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://br.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://in.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oy.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wl.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qv.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mb.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ha.newstarts.cn

[E16] 数字千分位
来源：http://xv.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://of.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://ft.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ov.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ik.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://je.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ko.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hi.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://an.szxytkj.cn

[E17] 首字母大写
来源：http://sm.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://od.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hm.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pk.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://co.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ew.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wp.asd995.cn

Ruby: s.capitalize
来源：http://no.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fj.shtwfgs.cn

[E18] 模板占位符替换
来源：http://zr.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nn.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qz.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://om.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yo.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yt.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ln.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ql.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zs.9csxet.cn

[E19] 多行文本按行拆分
来源：http://by.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://gj.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cx.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://oo.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://xt.lnxyls.cn

Java: s.lines().toList()
来源：http://ub.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://dt.9csxet.cn

Ruby: s.lines
来源：http://hd.huanxung.cn

C#:   s.Split('\n')
来源：http://nd.521024.cn

[E20] 判断字符串是否为空
来源：http://it.nszjky.cn

Py:   if not s:
来源：http://wj.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cp.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ya.shxzskj.cn

TS:   if (s === "") {}
来源：http://tt.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://hm.hahajie.cn

Go:   if s == "" {}
来源：http://ns.9csxet.cn

Ruby: if s.empty?
来源：http://hq.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gw.colortex.cn

[E21] 超长截断加省略号
来源：http://cr.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gx.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lm.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gp.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rj.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hn.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://yq.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qu.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ma.huanxung.cn

[E22] 字节长度与字符长度
来源：http://go.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ya.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sw.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hb.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mm.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oy.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pl.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://fz.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ig.jianghongdianzi.cn

================================================================================
来源：http://xc.9csxet.cn

F. 文件与目录
来源：http://ah.muxihuayi.cn

================================================================================
来源：http://ip.colortex.cn

[F01] 读取整个文件
来源：http://mo.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ai.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://iu.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dg.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cq.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qo.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lb.521024.cn

Ruby: File.read("a.txt")
来源：http://wn.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ck.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://lm.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mx.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uo.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cx.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mg.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ub.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bw.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rj.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lo.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://bz.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vv.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ou.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pd.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yr.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ub.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hh.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://va.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gk.gzmigu.cn

[F04] 追加写入文件
来源：http://pm.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hg.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ug.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uh.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aw.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://do.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sv.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cc.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vp.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ng.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ol.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://ty.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://va.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://pp.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ww.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zr.shtwfgs.cn

Ruby: File.exist?("a.txt")
来源：http://hk.521024.cn

C#:   File.Exists("a.txt")
来源：http://hk.muxihuayi.cn

[F06] 删除文件
来源：http://ey.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://de.newstarts.cn

PHP:  unlink("a.txt");
来源：http://oh.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lx.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ie.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kf.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://cc.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://pg.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://je.huanxung.cn

[F07] 创建目录（含多级）
来源：http://fi.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tf.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qz.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sl.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://in.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aw.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gn.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ry.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uu.wgjwhj.cn

[F08] 遍历目录
来源：http://fc.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kk.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ss.521024.cn

JS:   fs.readdirSync("dir")
来源：http://jq.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://hb.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kb.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wv.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://jx.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://nt.szxytkj.cn

[F09] 获取文件大小
来源：http://pv.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ip.newstarts.cn

PHP:  filesize("a.txt");
来源：http://iq.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://cj.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://wx.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tp.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ln.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://ym.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://qi.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://gv.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ap.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://th.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gm.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://zg.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zp.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kj.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ir.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jf.shxzskj.cn

[F11] 复制与移动文件
来源：http://ty.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kv.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ys.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ec.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yp.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cy.gzmigu.cn


<!-- 参考信息 -->