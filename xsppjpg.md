代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ns.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sw.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ap.yuexingan06.cn

[D26] 数组转字符串
来源：http://xk.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://fy.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://rw.nszjky.cn

JS:   arr.join(", ")
来源：http://kk.huanxung.cn

TS:   arr.join(", ")
来源：http://vb.9csxet.cn

Java: String.join(", ", list)
来源：http://hj.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://bs.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://zu.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://yq.newstarts.cn

================================================================================
来源：http://nk.yuexingan06.cn

E. 字符串处理
来源：http://ip.newstarts.cn

================================================================================
来源：http://vl.9csxet.cn

[E01] 拼接字符串
来源：http://wz.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ub.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fp.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ry.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dv.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wp.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://us.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ed.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xo.chemitech.net.cn

[E02] 重复字符串
来源：http://df.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://sw.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://rl.521024.cn

JS:   "ab".repeat(3)
来源：http://qx.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://yd.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://nr.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hp.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://ya.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://br.9csxet.cn

[E03] 截取子串
来源：http://yb.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qt.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xu.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gt.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://cs.lnxyls.cn

Java: s.substring(1, 4)
来源：http://if.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cy.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pp.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://el.shxzukj.cn

[E04] 查找子串位置
来源：http://ot.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://mm.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://pe.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bw.nicolike.cn

TS:   s.indexOf("x")
来源：http://cz.huixiangedu.cn

Java: s.indexOf("x")
来源：http://if.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://ok.hahajie.cn

Ruby: s.index("x")
来源：http://gx.521024.cn

C#:   s.IndexOf("x")
来源：http://ek.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wi.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rq.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bs.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nx.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pl.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jz.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gp.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://il.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dd.wgjwhj.cn

[E06] 替换子串
来源：http://aj.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ml.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://zr.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://up.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://ml.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wh.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lz.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://gz.shxzukj.cn

[E07] 按分隔符拆分
来源：http://lc.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ik.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://na.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bx.nicolike.cn

TS:   s.split(",")
来源：http://lh.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ke.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vt.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://od.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gp.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://mq.haigaiapp.cn

Py:   ",".join(items)
来源：http://qr.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://eb.panjiajie.cn

JS:   items.join(",")
来源：http://oq.9csxet.cn

TS:   items.join(",")
来源：http://us.huanxung.cn

Java: String.join(",", items)
来源：http://jm.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://cp.wgjwhj.cn

Ruby: items.join(",")
来源：http://lu.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://rz.nszjky.cn

[E09] 去除所有空白字符
来源：http://np.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fu.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xa.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://kl.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://xk.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://ym.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nc.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ni.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bl.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://mw.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://si.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wz.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://ga.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://xk.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://fu.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dz.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zb.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bl.huanxung.cn

[E11] 反转字符串
来源：http://so.szsharing.cn

Py:   s[::-1]
来源：http://cb.gzmigu.cn

PHP:  strrev($s);
来源：http://ps.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://io.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://dd.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gh.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qx.shtwfgs.cn

Ruby: s.reverse
来源：http://pd.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bh.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ve.colortex.cn

Py:   s.count("a")
来源：http://zx.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://ix.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://cb.nszjky.cn

TS:   s.split("a").length - 1
来源：http://qh.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://is.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://pp.newstarts.cn

Ruby: s.count("a")
来源：http://rz.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://cs.shtwfgs.cn

[E13] 逐字符遍历
来源：http://bh.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://hr.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mk.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xe.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://un.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lc.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mw.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xb.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xl.nicolike.cn

[E14] URL 编码与 Base64
来源：http://mk.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dp.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rw.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://df.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zk.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cf.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gu.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ta.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qa.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://oz.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ve.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wt.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://us.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cf.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cy.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pa.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lv.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ib.szxytkj.cn

[E16] 数字千分位
来源：http://ud.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://xd.shxzskj.cn

PHP:  number_format(1234567);
来源：http://pn.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fu.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dp.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gg.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zs.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tn.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://lm.panjiajie.cn

[E17] 首字母大写
来源：http://pl.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cd.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fb.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pu.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bd.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cu.nszjky.cn

Ruby: s.capitalize
来源：http://qi.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cx.9csxet.cn

[E18] 模板占位符替换
来源：http://zy.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mk.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tr.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rv.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kw.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cl.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uy.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pj.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kx.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ht.hahajie.cn

Py:   s.splitlines()
来源：http://sd.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://um.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://ha.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ab.chemitech.net.cn

Java: s.lines().toList()
来源：http://fn.521024.cn

Go:   strings.Split(s, "\n")
来源：http://wd.521024.cn

Ruby: s.lines
来源：http://yv.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://af.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://qh.521024.cn

Py:   if not s:
来源：http://jn.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qt.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kb.yuexingan06.cn

TS:   if (s === "") {}
来源：http://ps.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://rf.hahajie.cn

Go:   if s == "" {}
来源：http://dn.shxzskj.cn

Ruby: if s.empty?
来源：http://ol.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dk.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://nf.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bd.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dl.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fp.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pl.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ol.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ow.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ji.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nj.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://el.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qb.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ko.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sb.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eo.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mt.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xb.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://rq.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ze.shtwfgs.cn

================================================================================
来源：http://oa.yuntaijiaju.cn

F. 文件与目录
来源：http://lm.lnxyls.cn

================================================================================
来源：http://oa.gzmigu.cn

[F01] 读取整个文件
来源：http://yz.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gj.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://pd.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://in.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qt.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jq.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ca.521024.cn

Ruby: File.read("a.txt")
来源：http://ra.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://en.colortex.cn

[F02] 逐行读取文件
来源：http://zl.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qe.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xw.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bd.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nj.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hb.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://el.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jh.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mv.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://zx.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wu.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://le.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hm.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fv.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lu.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sv.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://qy.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pp.hnjuh.cn

[F04] 追加写入文件
来源：http://cu.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://la.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xz.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ry.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fh.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kt.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cy.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ly.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://he.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://jl.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vg.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://zx.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://nb.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://wn.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nz.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ka.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://oy.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://co.colortex.cn

[F06] 删除文件
来源：http://yj.nszjky.cn

Py:   os.remove("a.txt")
来源：http://qg.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://eh.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lb.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://es.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bo.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://tr.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://qm.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://be.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://bn.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bw.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sh.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hu.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zf.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://en.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ii.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nm.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zc.huixiangedu.cn

[F08] 遍历目录
来源：http://co.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ks.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ij.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ez.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://bm.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kg.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ns.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://to.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://qu.gzmigu.cn

[F09] 获取文件大小
来源：http://pk.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://et.newstarts.cn

PHP:  filesize("a.txt");
来源：http://gx.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://ng.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://xi.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bi.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://km.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://jh.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://rl.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://el.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xw.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ox.newstarts.cn


<!-- 参考信息 -->