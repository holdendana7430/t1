代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://ki.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://dx.hnjuh.cn

JS:   arr.join(", ")
来源：http://az.shtwfgs.cn

TS:   arr.join(", ")
来源：http://gi.yuexingan06.cn

Java: String.join(", ", list)
来源：http://nj.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://rn.nszjky.cn

Ruby: arr.join(", ")
来源：http://ou.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://it.lnxyls.cn

================================================================================
来源：http://fh.panjiajie.cn

E. 字符串处理
来源：http://lo.huixiangedu.cn

================================================================================
来源：http://qi.jctech888.com.cn

[E01] 拼接字符串
来源：http://em.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tm.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://el.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qt.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nz.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nr.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yh.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dq.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fx.muxihuayi.cn

[E02] 重复字符串
来源：http://je.muxihuayi.cn

Py:   "ab" * 3
来源：http://dr.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://qx.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://aw.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://ek.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://cb.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://sf.jctech888.com.cn

Ruby: "ab" * 3
来源：http://db.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xl.jctech888.com.cn

[E03] 截取子串
来源：http://gc.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://og.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hc.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ky.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://tr.gzmigu.cn

Java: s.substring(1, 4)
来源：http://bt.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rd.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fu.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://yj.muxihuayi.cn

[E04] 查找子串位置
来源：http://vp.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ea.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://lq.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ts.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://nz.shxzskj.cn

Java: s.indexOf("x")
来源：http://mj.asd995.cn

Go:   strings.Index(s, "x")
来源：http://oa.szsharing.cn

Ruby: s.index("x")
来源：http://ev.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://rg.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jm.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qb.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nj.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ky.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bu.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dl.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xs.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kw.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mh.haigaiapp.cn

[E06] 替换子串
来源：http://ef.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jo.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://qq.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ru.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://ka.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://se.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jh.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aj.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://uu.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://rl.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cz.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gz.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xa.huixiangedu.cn

TS:   s.split(",")
来源：http://gz.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ez.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://op.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://it.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tk.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://oo.yuexingan06.cn

Py:   ",".join(items)
来源：http://mz.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://ur.wgjwhj.cn

JS:   items.join(",")
来源：http://uz.muxihuayi.cn

TS:   items.join(",")
来源：http://uf.asd995.cn

Java: String.join(",", items)
来源：http://iq.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://zm.haigaiapp.cn

Ruby: items.join(",")
来源：http://eu.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://mk.nicolike.cn

[E09] 去除所有空白字符
来源：http://gh.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dt.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bh.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ue.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://wz.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://oz.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://it.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sp.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jh.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://tr.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ik.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ba.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://af.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ul.521024.cn

Java: String.format("%03d", 7)
来源：http://xk.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hu.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lu.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wu.lnxyls.cn

[E11] 反转字符串
来源：http://hd.hnjuh.cn

Py:   s[::-1]
来源：http://qp.bjjhwx.cn

PHP:  strrev($s);
来源：http://ct.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://ly.521024.cn

TS:   [...s].reverse().join("")
来源：http://vf.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rl.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cc.9csxet.cn

Ruby: s.reverse
来源：http://rl.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zz.nszjky.cn

[E12] 统计某字符出现次数
来源：http://rb.huixiangedu.cn

Py:   s.count("a")
来源：http://at.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://rm.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://lx.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ko.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ko.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://tp.9csxet.cn

Ruby: s.count("a")
来源：http://gv.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://vf.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://eu.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://ty.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pp.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gj.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vk.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gc.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ii.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dt.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lp.asd995.cn

[E14] URL 编码与 Base64
来源：http://gb.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pi.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iw.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xe.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fo.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bo.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fl.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kh.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://go.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://zd.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xz.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://au.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qk.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hy.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uy.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kl.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wk.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ru.9csxet.cn

[E16] 数字千分位
来源：http://ir.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ms.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://hq.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pi.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bf.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ij.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zu.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jf.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://pi.shxzskj.cn

[E17] 首字母大写
来源：http://ys.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dj.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fq.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xl.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rf.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zt.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vf.hnjuh.cn

Ruby: s.capitalize
来源：http://ea.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bh.yuexingan06.cn

[E18] 模板占位符替换
来源：http://pc.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vx.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mo.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sx.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://le.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tu.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://du.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://da.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zc.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://dj.nicolike.cn

Py:   s.splitlines()
来源：http://di.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sa.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://oc.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://oj.hahajie.cn

Java: s.lines().toList()
来源：http://yx.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://my.newstarts.cn

Ruby: s.lines
来源：http://hp.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://rg.huanxung.cn

[E20] 判断字符串是否为空
来源：http://ap.521024.cn

Py:   if not s:
来源：http://hi.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pn.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bn.521024.cn

TS:   if (s === "") {}
来源：http://qy.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://lq.szsharing.cn

Go:   if s == "" {}
来源：http://eu.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://dk.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ol.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://dh.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kj.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ja.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nx.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uq.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wg.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://go.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cs.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kg.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://uf.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nu.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://id.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cj.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yp.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kt.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ff.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ym.haigaiapp.cn

================================================================================
来源：http://hs.huanxung.cn

F. 文件与目录
来源：http://gr.panjiajie.cn

================================================================================
来源：http://at.jctech888.com.cn

[F01] 读取整个文件
来源：http://wi.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ti.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://nn.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mt.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ur.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://au.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rf.newstarts.cn

Ruby: File.read("a.txt")
来源：http://gh.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://lo.nicolike.cn

[F02] 逐行读取文件
来源：http://uj.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gm.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oh.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hg.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gb.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cw.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rq.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bz.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xn.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://cg.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cj.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tp.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yq.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yu.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vq.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ei.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://fy.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ih.9csxet.cn

[F04] 追加写入文件
来源：http://ty.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://co.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cm.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bi.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vm.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yb.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pq.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mu.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://ju.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xy.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://kq.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://kh.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://wk.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qm.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ug.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://sa.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://vx.9csxet.cn

[F06] 删除文件
来源：http://sl.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://do.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://vn.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bx.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ff.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fy.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://ba.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://vo.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://zh.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://mr.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xo.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sb.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zg.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ri.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dq.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ed.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ui.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ed.szxytkj.cn

[F08] 遍历目录
来源：http://ww.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xn.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sv.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://yh.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://hv.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qu.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ff.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://oz.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://gr.haigaiapp.cn

[F09] 获取文件大小
来源：http://yn.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://td.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://bs.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://oc.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://zr.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zm.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ca.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://jh.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://az.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://hq.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ox.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://od.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://qi.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vr.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://de.newstarts.cn


<!-- 参考信息 -->