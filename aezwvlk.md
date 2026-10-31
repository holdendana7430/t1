代发 wailian999

Java: String.join(", ", list)
来源：http://mc.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://mu.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://gz.asd995.cn

C#:   string.Join(", ", list)
来源：http://em.bookmarksfly.cn

================================================================================
来源：http://ie.szsharing.cn

E. 字符串处理
来源：http://qf.gzmigu.cn

================================================================================
来源：http://pk.chemitech.net.cn

[E01] 拼接字符串
来源：http://dz.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kj.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zk.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iv.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dq.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yf.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fm.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fz.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fb.bjjhwx.cn

[E02] 重复字符串
来源：http://os.lnxyls.cn

Py:   "ab" * 3
来源：http://fi.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://kc.newstarts.cn

JS:   "ab".repeat(3)
来源：http://xu.nszjky.cn

TS:   "ab".repeat(3)
来源：http://pd.newstarts.cn

Java: "ab".repeat(3)
来源：http://zm.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://we.yuexingan06.cn

Ruby: "ab" * 3
来源：http://hv.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fz.asd995.cn

[E03] 截取子串
来源：http://iv.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://je.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xk.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ja.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://vx.shxzskj.cn

Java: s.substring(1, 4)
来源：http://pw.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ji.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hg.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://og.shxzukj.cn

[E04] 查找子串位置
来源：http://uf.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ow.huanxung.cn

PHP:  strpos($s, "x");
来源：http://ms.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yb.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ze.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://jx.521024.cn

Go:   strings.Index(s, "x")
来源：http://to.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://jy.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://wi.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://re.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ea.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yz.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bz.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yc.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dq.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sd.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wo.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fs.colortex.cn

[E06] 替换子串
来源：http://tl.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jm.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://ls.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://np.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://od.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tj.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fw.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qe.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://rd.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://nj.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yc.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yb.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qr.yuntaijiaju.cn

TS:   s.split(",")
来源：http://ta.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xw.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ev.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://yq.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hm.newstarts.cn

[E08] 数组按分隔符合并
来源：http://ub.haigaiapp.cn

Py:   ",".join(items)
来源：http://bz.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://sz.lnxyls.cn

JS:   items.join(",")
来源：http://fy.huixinmuqiang.cn

TS:   items.join(",")
来源：http://gz.shtwfgs.cn

Java: String.join(",", items)
来源：http://li.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://fu.haigaiapp.cn

Ruby: items.join(",")
来源：http://vk.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://nv.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://rw.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ji.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ub.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://cg.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wr.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://wl.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jy.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pq.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://pz.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yu.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ox.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://om.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://vo.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://zt.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://co.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ik.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ls.asd995.cn

[E11] 反转字符串
来源：http://lb.jctech888.com.cn

Py:   s[::-1]
来源：http://gs.shxzukj.cn

PHP:  strrev($s);
来源：http://bz.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://zk.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://lo.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://da.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yb.nszjky.cn

Ruby: s.reverse
来源：http://mb.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ll.521024.cn

[E12] 统计某字符出现次数
来源：http://ny.asd995.cn

Py:   s.count("a")
来源：http://cg.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://pz.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://yl.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://rl.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tg.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://lm.nszjky.cn

Ruby: s.count("a")
来源：http://by.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://cx.hahajie.cn

[E13] 逐字符遍历
来源：http://bm.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://yz.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ju.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qa.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hv.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jq.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mt.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bh.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kw.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://wr.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vn.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dt.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eq.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://om.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vj.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tp.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aj.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ma.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ok.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yj.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://if.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mh.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xc.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fb.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nk.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nh.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kx.colortex.cn

[E16] 数字千分位
来源：http://ow.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://ss.9csxet.cn

PHP:  number_format(1234567);
来源：http://om.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fk.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hc.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://li.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wj.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ga.asd995.cn

C#:   1234567.ToString("N0")
来源：http://xr.gzmigu.cn

[E17] 首字母大写
来源：http://ld.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rq.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qd.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zl.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lf.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://um.asd995.cn

Ruby: s.capitalize
来源：http://ll.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rd.nszjky.cn

[E18] 模板占位符替换
来源：http://qj.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kx.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cu.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oi.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rx.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aw.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bf.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zl.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vg.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://hn.gzmigu.cn

Py:   s.splitlines()
来源：http://nj.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qx.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://hm.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://ve.chemitech.net.cn

Java: s.lines().toList()
来源：http://qg.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://tk.hnjuh.cn

Ruby: s.lines
来源：http://mj.wgjwhj.cn

C#:   s.Split('\n')
来源：http://uf.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://iw.muxihuayi.cn

Py:   if not s:
来源：http://lz.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ff.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jr.shxzukj.cn

TS:   if (s === "") {}
来源：http://vj.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://sk.bjjhwx.cn

Go:   if s == "" {}
来源：http://wl.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://tt.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rx.hahajie.cn

[E21] 超长截断加省略号
来源：http://ii.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bx.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://to.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ut.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gn.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ij.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ns.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bt.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lw.521024.cn

[E22] 字节长度与字符长度
来源：http://vx.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aq.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nb.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qx.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ms.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jp.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ep.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yy.huixiangedu.cn

================================================================================
来源：http://ud.szsharing.cn

F. 文件与目录
来源：http://yz.szxytkj.cn

================================================================================
来源：http://cd.newstarts.cn

[F01] 读取整个文件
来源：http://mi.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ji.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://hr.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ve.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ss.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qj.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pv.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://oz.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://sn.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://gl.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ju.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ww.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fv.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://om.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hl.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ke.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://va.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://db.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://sk.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rf.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://an.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hb.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ko.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dj.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://ap.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jq.shtwfgs.cn

[F04] 追加写入文件
来源：http://tk.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kf.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jy.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rq.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wu.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ti.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ig.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wv.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://ri.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dy.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://sj.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://zy.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://wz.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jr.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ch.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://zq.521024.cn

C#:   File.Exists("a.txt")
来源：http://lh.szsharing.cn

[F06] 删除文件
来源：http://zo.nszjky.cn

Py:   os.remove("a.txt")
来源：http://af.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://ko.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uy.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gp.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sj.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://qs.colortex.cn

Ruby: File.delete("a.txt")
来源：http://sd.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ye.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://hg.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ip.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gv.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ho.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ux.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qf.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://af.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rm.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lc.haigaiapp.cn

[F08] 遍历目录
来源：http://pz.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dz.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://di.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://mo.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://ig.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xv.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vg.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://nm.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://on.bookmarksfly.cn

[F09] 获取文件大小
来源：http://bx.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://hc.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://lo.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://pj.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://bs.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hs.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dm.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://vm.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://jb.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://lh.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ku.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yi.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zu.colortex.cn

TS:   path.extname("a.txt")
来源：http://nh.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fb.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wy.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://af.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ta.hahajie.cn

[F11] 复制与移动文件
来源：http://zw.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.huixinmuqiang.cn


<!-- 参考信息 -->