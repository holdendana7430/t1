代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bs.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fo.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://py.muxihuayi.cn

[D26] 数组转字符串
来源：http://hd.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://uj.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://tz.colortex.cn

JS:   arr.join(", ")
来源：http://rb.521024.cn

TS:   arr.join(", ")
来源：http://ax.nicolike.cn

Java: String.join(", ", list)
来源：http://eq.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://tm.szsharing.cn

Ruby: arr.join(", ")
来源：http://gw.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://yx.bjjhwx.cn

================================================================================
来源：http://pz.huixinmuqiang.cn

E. 字符串处理
来源：http://zs.shxzskj.cn

================================================================================
来源：http://cp.9csxet.cn

[E01] 拼接字符串
来源：http://wy.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jc.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://st.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sf.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mg.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gs.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ky.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yk.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lk.chemitech.net.cn

[E02] 重复字符串
来源：http://pd.gzmigu.cn

Py:   "ab" * 3
来源：http://wu.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://nd.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://xo.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://mr.hahajie.cn

Java: "ab".repeat(3)
来源：http://rn.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://uk.szsharing.cn

Ruby: "ab" * 3
来源：http://em.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fx.hnjuh.cn

[E03] 截取子串
来源：http://xo.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lv.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ue.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wx.huanxung.cn

TS:   s.slice(1, 4)
来源：http://xj.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://rn.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iv.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gw.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://fi.wgjwhj.cn

[E04] 查找子串位置
来源：http://nw.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ly.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://vm.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hd.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://rf.szsharing.cn

Java: s.indexOf("x")
来源：http://am.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ij.haigaiapp.cn

Ruby: s.index("x")
来源：http://ta.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://li.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ur.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://db.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://df.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://go.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fx.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lb.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xh.chemitech.net.cn

[E06] 替换子串
来源：http://vt.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wt.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://vc.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://qi.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vi.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vu.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://la.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://vq.asd995.cn

[E07] 按分隔符拆分
来源：http://vc.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hn.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://db.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ce.jianghongdianzi.cn

TS:   s.split(",")
来源：http://qw.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://by.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fo.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://vg.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yb.nicolike.cn

[E08] 数组按分隔符合并
来源：http://cb.shtwfgs.cn

Py:   ",".join(items)
来源：http://vm.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://ea.szxytkj.cn

JS:   items.join(",")
来源：http://kh.hahajie.cn

TS:   items.join(",")
来源：http://nj.hahajie.cn

Java: String.join(",", items)
来源：http://ka.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://dw.haigaiapp.cn

Ruby: items.join(",")
来源：http://kk.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://ru.nszjky.cn

[E09] 去除所有空白字符
来源：http://cs.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ce.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://st.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://zh.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://tv.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://mk.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ap.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gf.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vv.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ty.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wk.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pr.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://pt.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://mq.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://pe.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://al.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nl.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mx.nicolike.cn

[E11] 反转字符串
来源：http://we.wgjwhj.cn

Py:   s[::-1]
来源：http://am.hahajie.cn

PHP:  strrev($s);
来源：http://fo.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://qh.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://dk.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vl.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://js.newstarts.cn

Ruby: s.reverse
来源：http://kv.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zq.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://nh.huixinmuqiang.cn

Py:   s.count("a")
来源：http://vf.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://za.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://yx.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://ly.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jg.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://nq.bookmarksfly.cn

Ruby: s.count("a")
来源：http://gz.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://fs.asd995.cn

[E13] 逐字符遍历
来源：http://mc.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://pf.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ho.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://de.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wr.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nl.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zs.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rs.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bn.nicolike.cn

[E14] URL 编码与 Base64
来源：http://lv.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ex.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tu.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wh.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cd.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ef.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hx.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lm.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zv.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://na.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://si.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kf.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cs.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://le.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rb.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vy.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mf.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gp.newstarts.cn

[E16] 数字千分位
来源：http://jf.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://oq.hnjuh.cn

PHP:  number_format(1234567);
来源：http://bi.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gg.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mx.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://az.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rc.colortex.cn

C#:   1234567.ToString("N0")
来源：http://uf.lnxyls.cn

[E17] 首字母大写
来源：http://hm.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ux.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ea.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hc.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uv.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fq.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hn.lnxyls.cn

Ruby: s.capitalize
来源：http://wu.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cr.hahajie.cn

[E18] 模板占位符替换
来源：http://oh.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wf.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fm.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hu.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fy.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mw.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eg.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nw.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gu.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://wv.lnxyls.cn

Py:   s.splitlines()
来源：http://tc.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dz.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://or.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ll.szsharing.cn

Java: s.lines().toList()
来源：http://er.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://ry.szxytkj.cn

Ruby: s.lines
来源：http://ky.nszjky.cn

C#:   s.Split('\n')
来源：http://bt.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://hh.huixinmuqiang.cn

Py:   if not s:
来源：http://na.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yy.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fs.shtwfgs.cn

TS:   if (s === "") {}
来源：http://zm.521024.cn

Java: if (s.isEmpty()) {}
来源：http://ul.huanxung.cn

Go:   if s == "" {}
来源：http://aw.9csxet.cn

Ruby: if s.empty?
来源：http://pm.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yp.lnxyls.cn

[E21] 超长截断加省略号
来源：http://od.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ic.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tj.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vy.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eb.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cz.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://yy.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jk.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iz.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://wu.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vi.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ui.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pk.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lm.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ut.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://la.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ov.lnxyls.cn

================================================================================
来源：http://pf.huixiangedu.cn

F. 文件与目录
来源：http://mi.nicolike.cn

================================================================================
来源：http://gu.hahajie.cn

[F01] 读取整个文件
来源：http://rn.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qr.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://zp.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kb.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ff.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gf.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kt.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://di.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://mh.bjjhwx.cn

[F02] 逐行读取文件
来源：http://rb.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gn.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bk.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hp.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ho.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oc.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vg.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ya.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fb.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://av.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://he.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zk.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://du.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rl.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gx.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dq.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://jx.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bw.bookmarksfly.cn

[F04] 追加写入文件
来源：http://gs.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wv.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jn.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ur.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nz.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rl.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hi.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fj.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sp.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://mx.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bi.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://fl.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://dd.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://xr.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://em.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jx.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://sl.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://zn.panjiajie.cn

[F06] 删除文件
来源：http://wa.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://uj.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://qw.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cy.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rh.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gx.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://jr.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://be.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://xh.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://sb.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uv.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pw.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ym.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wg.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ru.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wq.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ol.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gx.nszjky.cn

[F08] 遍历目录
来源：http://dh.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ao.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tn.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://hi.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://mw.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ai.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fh.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://fw.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://wj.szxytkj.cn

[F09] 获取文件大小
来源：http://gs.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://db.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://yi.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://wu.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://nj.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ob.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oc.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://cm.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://fx.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://xu.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gk.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uk.szxytkj.cn


<!-- 参考信息 -->