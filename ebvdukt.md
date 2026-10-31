代发 wailian999

Java: String.join(", ", list)
来源：http://lt.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://nr.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://kv.521024.cn

C#:   string.Join(", ", list)
来源：http://fh.bjjhwx.cn

================================================================================
来源：http://hl.yuntaijiaju.cn

E. 字符串处理
来源：http://so.bjjhwx.cn

================================================================================
来源：http://qe.bjjhwx.cn

[E01] 拼接字符串
来源：http://oa.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zb.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ka.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fz.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qk.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sa.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://po.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pk.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uq.gzmigu.cn

[E02] 重复字符串
来源：http://ih.9csxet.cn

Py:   "ab" * 3
来源：http://pz.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://zj.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://jv.newstarts.cn

TS:   "ab".repeat(3)
来源：http://vk.colortex.cn

Java: "ab".repeat(3)
来源：http://xk.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://vm.haigaiapp.cn

Ruby: "ab" * 3
来源：http://zg.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gb.haigaiapp.cn

[E03] 截取子串
来源：http://cg.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ul.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bp.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://on.nicolike.cn

TS:   s.slice(1, 4)
来源：http://vq.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://xg.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oe.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yf.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://qz.jctech888.com.cn

[E04] 查找子串位置
来源：http://rw.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://yw.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://dn.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://st.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://qa.asd995.cn

Java: s.indexOf("x")
来源：http://tf.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://kj.lnxyls.cn

Ruby: s.index("x")
来源：http://dk.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://vx.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iw.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cl.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bv.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pu.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kq.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ws.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://os.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wu.szxytkj.cn

[E06] 替换子串
来源：http://gp.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dq.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://og.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jd.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://dg.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yn.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qs.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wt.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ne.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://rg.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ui.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dx.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nm.9csxet.cn

TS:   s.split(",")
来源：http://rv.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rl.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ai.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://fb.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yz.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://dg.newstarts.cn

Py:   ",".join(items)
来源：http://na.nszjky.cn

PHP:  implode(",", $items);
来源：http://pz.bjjhwx.cn

JS:   items.join(",")
来源：http://zz.newstarts.cn

TS:   items.join(",")
来源：http://hi.nicolike.cn

Java: String.join(",", items)
来源：http://re.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://zp.panjiajie.cn

Ruby: items.join(",")
来源：http://ku.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://vf.hahajie.cn

[E09] 去除所有空白字符
来源：http://kw.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nf.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qc.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://sv.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://rd.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://yx.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://th.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://no.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sv.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://ki.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qu.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ni.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://qz.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://vv.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://sm.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kr.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yf.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dv.bookmarksfly.cn

[E11] 反转字符串
来源：http://yl.wgjwhj.cn

Py:   s[::-1]
来源：http://sz.szsharing.cn

PHP:  strrev($s);
来源：http://tz.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://cv.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://yt.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://op.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pi.huanxung.cn

Ruby: s.reverse
来源：http://rv.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bx.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://sz.wgjwhj.cn

Py:   s.count("a")
来源：http://hw.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://ho.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://br.521024.cn

TS:   s.split("a").length - 1
来源：http://tz.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sd.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://oc.asd995.cn

Ruby: s.count("a")
来源：http://hw.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://dm.lnxyls.cn

[E13] 逐字符遍历
来源：http://gu.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://xx.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rv.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iy.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qe.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jw.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://st.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uf.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ae.colortex.cn

[E14] URL 编码与 Base64
来源：http://og.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://li.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ro.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jb.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rp.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vr.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mu.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gu.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://an.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ec.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oc.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xg.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tn.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cp.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mp.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fz.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vy.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tp.jctech888.com.cn

[E16] 数字千分位
来源：http://lg.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://sf.lnxyls.cn

PHP:  number_format(1234567);
来源：http://hx.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qh.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rr.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qj.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vm.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rd.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://tf.newstarts.cn

[E17] 首字母大写
来源：http://sz.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://td.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ep.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dr.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iq.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://en.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ua.lnxyls.cn

Ruby: s.capitalize
来源：http://lo.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ze.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ok.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vq.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rg.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wb.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gc.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gh.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vj.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gm.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aq.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://ub.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ab.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gs.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://da.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://jq.panjiajie.cn

Java: s.lines().toList()
来源：http://ov.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://vd.shxzskj.cn

Ruby: s.lines
来源：http://bu.hahajie.cn

C#:   s.Split('\n')
来源：http://vt.9csxet.cn

[E20] 判断字符串是否为空
来源：http://xv.newstarts.cn

Py:   if not s:
来源：http://ve.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ja.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://am.hahajie.cn

TS:   if (s === "") {}
来源：http://aa.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://fn.wgjwhj.cn

Go:   if s == "" {}
来源：http://lp.haigaiapp.cn

Ruby: if s.empty?
来源：http://xs.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kg.hnjuh.cn

[E21] 超长截断加省略号
来源：http://oe.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lk.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ue.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ff.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hn.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://us.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://lg.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kk.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://el.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://fa.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cc.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hx.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ga.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mx.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xv.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ro.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://mi.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yx.bookmarksfly.cn

================================================================================
来源：http://ze.szsharing.cn

F. 文件与目录
来源：http://pr.hnjuh.cn

================================================================================
来源：http://im.lnxyls.cn

[F01] 读取整个文件
来源：http://bc.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dw.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://th.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dc.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lh.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ej.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sz.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://vo.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://oc.shtwfgs.cn

[F02] 逐行读取文件
来源：http://to.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ud.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vz.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://io.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fz.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hr.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fl.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wc.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ro.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ml.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zh.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jo.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jq.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ym.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ld.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rq.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://jz.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hu.colortex.cn

[F04] 追加写入文件
来源：http://jb.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bv.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eq.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ha.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zy.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ah.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ul.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uz.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vh.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://er.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kf.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://es.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://qb.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://rb.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ol.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ks.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://di.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://ux.hahajie.cn

[F06] 删除文件
来源：http://uk.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://ce.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://bx.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fa.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yk.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hu.521024.cn

Go:   os.Remove("a.txt")
来源：http://iv.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://lz.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://dj.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://qv.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ci.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kj.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kx.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lv.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fx.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ri.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zd.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ba.szxytkj.cn

[F08] 遍历目录
来源：http://da.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ps.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fb.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://ds.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://jm.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iz.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ii.asd995.cn

Ruby: Dir.children("dir")
来源：http://nm.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://bq.szxytkj.cn

[F09] 获取文件大小
来源：http://mf.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://rj.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://vc.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://fy.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://ny.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jr.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yg.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://dm.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://wt.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://qr.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hc.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xr.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zb.colortex.cn

TS:   path.extname("a.txt")
来源：http://fp.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mz.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dv.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fr.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qe.hnjuh.cn

[F11] 复制与移动文件
来源：http://cd.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fq.colortex.cn


<!-- 参考信息 -->