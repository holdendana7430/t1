代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://by.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nb.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zd.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://js.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nm.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cr.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ky.nszjky.cn

[E02] 重复字符串
来源：http://pz.szxytkj.cn

Py:   "ab" * 3
来源：http://ht.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://lv.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://qv.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://pu.gzmigu.cn

Java: "ab".repeat(3)
来源：http://gu.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://jq.newstarts.cn

Ruby: "ab" * 3
来源：http://dj.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://by.asd995.cn

[E03] 截取子串
来源：http://zk.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oj.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mz.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aj.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://pf.9csxet.cn

Java: s.substring(1, 4)
来源：http://ut.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ud.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cc.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://mz.huixiangedu.cn

[E04] 查找子串位置
来源：http://by.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://dj.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://sf.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fg.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ny.bjjhwx.cn

Java: s.indexOf("x")
来源：http://gw.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://ue.gzmigu.cn

Ruby: s.index("x")
来源：http://xb.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ku.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ve.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://md.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ah.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ei.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://px.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ao.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://be.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uz.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jr.chemitech.net.cn

[E06] 替换子串
来源：http://lc.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lv.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://xg.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oj.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ig.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jv.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tl.colortex.cn

C#:   s.Replace("a", "b")
来源：http://pr.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://up.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lz.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xv.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ql.nicolike.cn

TS:   s.split(",")
来源：http://fx.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rb.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ve.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://jy.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bg.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://ax.jctech888.com.cn

Py:   ",".join(items)
来源：http://on.shxzskj.cn

PHP:  implode(",", $items);
来源：http://wq.nicolike.cn

JS:   items.join(",")
来源：http://tp.asd995.cn

TS:   items.join(",")
来源：http://yo.nicolike.cn

Java: String.join(",", items)
来源：http://oj.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://rm.nszjky.cn

Ruby: items.join(",")
来源：http://ct.lnxyls.cn

C#:   string.Join(",", items)
来源：http://hz.newstarts.cn

[E09] 去除所有空白字符
来源：http://wq.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://co.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fy.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://sb.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://ya.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://gh.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ho.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sj.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kl.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://bq.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ng.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ps.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://xt.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://kj.huanxung.cn

Java: String.format("%03d", 7)
来源：http://rt.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mt.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://up.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://od.521024.cn

[E11] 反转字符串
来源：http://lx.szxytkj.cn

Py:   s[::-1]
来源：http://yn.nicolike.cn

PHP:  strrev($s);
来源：http://cd.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://mo.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://zs.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xq.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mb.lnxyls.cn

Ruby: s.reverse
来源：http://dj.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jp.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://sj.hnjuh.cn

Py:   s.count("a")
来源：http://xf.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://so.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://qp.colortex.cn

TS:   s.split("a").length - 1
来源：http://zm.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ek.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://dn.521024.cn

Ruby: s.count("a")
来源：http://lo.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://sc.shxzskj.cn

[E13] 逐字符遍历
来源：http://rm.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://ub.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://io.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mh.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fi.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mu.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yd.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vg.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://mq.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qp.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://az.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mm.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iv.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fx.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dq.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ch.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xj.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://xb.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kc.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://td.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jx.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://em.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bx.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aw.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mj.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uj.asd995.cn

[E16] 数字千分位
来源：http://py.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://el.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://td.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yn.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mp.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bl.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ml.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pb.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://pv.bookmarksfly.cn

[E17] 首字母大写
来源：http://tj.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bt.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://me.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dg.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pq.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ky.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ze.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://ud.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://an.521024.cn

[E18] 模板占位符替换
来源：http://lr.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pk.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ig.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ya.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ut.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wo.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fm.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hu.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cn.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://pj.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ky.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qe.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://du.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://ca.jctech888.com.cn

Java: s.lines().toList()
来源：http://kd.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://il.newstarts.cn

Ruby: s.lines
来源：http://va.asd995.cn

C#:   s.Split('\n')
来源：http://er.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://bl.nicolike.cn

Py:   if not s:
来源：http://qs.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qz.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gy.wgjwhj.cn

TS:   if (s === "") {}
来源：http://wy.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://pz.521024.cn

Go:   if s == "" {}
来源：http://pi.szxytkj.cn

Ruby: if s.empty?
来源：http://qi.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gj.asd995.cn

[E21] 超长截断加省略号
来源：http://fp.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kf.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://il.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ct.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sx.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://dy.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rl.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://um.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://wk.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pb.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ds.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ga.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eg.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wf.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bj.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://ng.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dq.huanxung.cn

================================================================================
来源：http://da.szxytkj.cn

F. 文件与目录
来源：http://vc.wgjwhj.cn

================================================================================
来源：http://sr.szsharing.cn

[F01] 读取整个文件
来源：http://uc.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uv.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://qj.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wj.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vk.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mw.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gt.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://of.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://at.szsharing.cn

[F02] 逐行读取文件
来源：http://ue.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fp.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uh.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ul.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ew.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ks.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wx.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mn.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ht.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://pu.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gr.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iw.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sz.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vw.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rk.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rh.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ak.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ac.panjiajie.cn

[F04] 追加写入文件
来源：http://st.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lg.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ng.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ep.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vy.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bu.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rv.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jn.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://io.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://vh.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sg.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://xw.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://az.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://pm.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ae.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uu.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://xg.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://yp.shxzskj.cn

[F06] 删除文件
来源：http://ax.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://yi.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://wb.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yd.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://en.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://wt.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://qh.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://fa.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://qh.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cm.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://na.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mj.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vk.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cl.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pk.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cb.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gv.shxzukj.cn

[F08] 遍历目录
来源：http://xc.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yh.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://by.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://bj.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://ru.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qk.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zv.9csxet.cn

Ruby: Dir.children("dir")
来源：http://sx.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://vg.muxihuayi.cn

[F09] 获取文件大小
来源：http://he.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://dh.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://jq.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ii.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ul.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oz.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cw.newstarts.cn

Ruby: File.size("a.txt")
来源：http://wm.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://au.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://zd.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eh.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bb.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gz.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ch.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cc.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fv.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qk.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jd.521024.cn

[F11] 复制与移动文件
来源：http://nr.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nw.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pf.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://em.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ho.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wg.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bb.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xq.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ri.gzmigu.cn

[F12] CSV 读写
来源：http://ey.huanxung.cn


<!-- 参考信息 -->