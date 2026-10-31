代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://sm.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://xi.huanxung.cn

JS:   arr.join(", ")
来源：http://sr.shxzukj.cn

TS:   arr.join(", ")
来源：http://fm.521024.cn

Java: String.join(", ", list)
来源：http://hd.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://rv.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://kn.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://jy.colortex.cn

================================================================================
来源：http://gv.szxytkj.cn

E. 字符串处理
来源：http://zo.yuntaijiaju.cn

================================================================================
来源：http://eo.nszjky.cn

[E01] 拼接字符串
来源：http://xh.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bo.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pg.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fc.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://id.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lf.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kk.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cr.521024.cn

[E02] 重复字符串
来源：http://kz.gzmigu.cn

Py:   "ab" * 3
来源：http://wd.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://lc.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://mu.asd995.cn

TS:   "ab".repeat(3)
来源：http://ik.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://cj.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://of.521024.cn

Ruby: "ab" * 3
来源：http://yn.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jq.szxytkj.cn

[E03] 截取子串
来源：http://uk.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vs.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sp.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cs.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://km.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://fs.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://to.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ph.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://rw.gzmigu.cn

[E04] 查找子串位置
来源：http://fo.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://pc.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://vi.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jb.colortex.cn

TS:   s.indexOf("x")
来源：http://rb.nszjky.cn

Java: s.indexOf("x")
来源：http://wj.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://up.szsharing.cn

Ruby: s.index("x")
来源：http://af.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://gn.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://va.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fb.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tg.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rh.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fo.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cz.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hi.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oz.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://um.521024.cn

[E06] 替换子串
来源：http://gu.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uj.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://tn.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vr.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://bs.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://di.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yd.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ti.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://cj.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://qs.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pe.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mq.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aj.muxihuayi.cn

TS:   s.split(",")
来源：http://cm.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eu.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mb.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://av.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vl.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ck.colortex.cn

Py:   ",".join(items)
来源：http://lk.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://yj.panjiajie.cn

JS:   items.join(",")
来源：http://vw.shxzskj.cn

TS:   items.join(",")
来源：http://pe.colortex.cn

Java: String.join(",", items)
来源：http://en.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://fu.haigaiapp.cn

Ruby: items.join(",")
来源：http://xq.panjiajie.cn

C#:   string.Join(",", items)
来源：http://fp.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://rf.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ff.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zx.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://rw.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://eh.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://pc.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://me.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ef.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ef.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://to.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mo.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rk.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://th.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://tn.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://ix.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vk.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wv.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yr.521024.cn

[E11] 反转字符串
来源：http://wy.shxzskj.cn

Py:   s[::-1]
来源：http://sk.hnjuh.cn

PHP:  strrev($s);
来源：http://co.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://it.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://ro.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xi.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zm.nszjky.cn

Ruby: s.reverse
来源：http://ut.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ri.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://nd.hahajie.cn

Py:   s.count("a")
来源：http://zw.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://sp.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://ls.9csxet.cn

TS:   s.split("a").length - 1
来源：http://nr.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eu.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://vw.chemitech.net.cn

Ruby: s.count("a")
来源：http://dn.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://qw.shtwfgs.cn

[E13] 逐字符遍历
来源：http://wq.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://yl.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ba.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://js.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zx.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ml.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vr.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hk.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hf.nszjky.cn

[E14] URL 编码与 Base64
来源：http://tf.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://il.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qu.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kj.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ur.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ra.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bu.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://er.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uc.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://zq.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mg.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sg.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xc.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eo.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yh.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://od.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lp.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://db.jianghongdianzi.cn

[E16] 数字千分位
来源：http://qd.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://km.colortex.cn

PHP:  number_format(1234567);
来源：http://nf.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vg.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nk.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ck.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hu.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sr.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://gx.colortex.cn

[E17] 首字母大写
来源：http://vh.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sv.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gd.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://md.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wh.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dy.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jo.haigaiapp.cn

Ruby: s.capitalize
来源：http://vx.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ls.asd995.cn

[E18] 模板占位符替换
来源：http://wt.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lm.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ij.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qb.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zn.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qn.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yw.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nt.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cl.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://ya.shxzskj.cn

Py:   s.splitlines()
来源：http://sn.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ez.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://oq.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://ge.szsharing.cn

Java: s.lines().toList()
来源：http://ar.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://tk.asd995.cn

Ruby: s.lines
来源：http://ax.jctech888.com.cn

C#:   s.Split('\n')
来源：http://az.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://bd.jctech888.com.cn

Py:   if not s:
来源：http://ly.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mq.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rs.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://ia.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://az.haigaiapp.cn

Go:   if s == "" {}
来源：http://jb.newstarts.cn

Ruby: if s.empty?
来源：http://no.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vm.9csxet.cn

[E21] 超长截断加省略号
来源：http://oj.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://do.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gu.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iq.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jl.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nw.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://fh.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ur.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cr.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://gw.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hp.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iy.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tm.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ip.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sa.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://pd.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pg.szxytkj.cn

================================================================================
来源：http://qz.bookmarksfly.cn

F. 文件与目录
来源：http://xx.shtwfgs.cn

================================================================================
来源：http://dw.shxzukj.cn

[F01] 读取整个文件
来源：http://ll.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sf.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://rx.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uu.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://af.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qm.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hd.colortex.cn

Ruby: File.read("a.txt")
来源：http://fd.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://pk.muxihuayi.cn

[F02] 逐行读取文件
来源：http://qh.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hd.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ep.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nc.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kz.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dm.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qa.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iy.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://af.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xj.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cg.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dr.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sp.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vs.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gs.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://an.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hy.haigaiapp.cn

[F04] 追加写入文件
来源：http://bt.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qy.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ei.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yy.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nh.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bk.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yo.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yb.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gr.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://kr.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ec.colortex.cn

PHP:  file_exists("a.txt");
来源：http://sb.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://mj.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://aq.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qj.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ly.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://hs.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ki.yuntaijiaju.cn

[F06] 删除文件
来源：http://xn.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://wl.9csxet.cn

PHP:  unlink("a.txt");
来源：http://td.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eh.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dp.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dd.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ju.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://nx.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://lh.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://tm.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ec.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://io.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lv.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qu.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ui.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fr.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://po.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pv.jctech888.com.cn

[F08] 遍历目录
来源：http://wh.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yw.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hj.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://jy.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ps.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wl.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yo.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://wi.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://ee.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://ir.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://yi.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://cw.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://vg.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://rp.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ze.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ap.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://iv.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://co.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ey.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://np.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bj.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qy.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://xr.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ng.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://to.bookmarksfly.cn


<!-- 参考信息 -->