代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ha.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uo.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bx.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dt.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ne.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tw.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vq.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zr.szsharing.cn

[E02] 重复字符串
来源：http://zo.521024.cn

Py:   "ab" * 3
来源：http://bp.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://lr.521024.cn

JS:   "ab".repeat(3)
来源：http://ie.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://hg.shxzskj.cn

Java: "ab".repeat(3)
来源：http://nw.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://yj.bjjhwx.cn

Ruby: "ab" * 3
来源：http://bo.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://af.jianghongdianzi.cn

[E03] 截取子串
来源：http://yw.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qc.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tt.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vg.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://lt.nszjky.cn

Java: s.substring(1, 4)
来源：http://yh.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ao.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fj.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://xz.szxytkj.cn

[E04] 查找子串位置
来源：http://bt.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://jj.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://ae.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ah.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ib.shtwfgs.cn

Java: s.indexOf("x")
来源：http://wo.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://aj.colortex.cn

Ruby: s.index("x")
来源：http://vn.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://mx.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yy.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vo.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uq.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://py.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fp.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bk.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mj.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tb.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yr.chemitech.net.cn

[E06] 替换子串
来源：http://ti.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gg.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://il.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://ww.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bz.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lu.colortex.cn

C#:   s.Replace("a", "b")
来源：http://nw.hnjuh.cn

[E07] 按分隔符拆分
来源：http://fg.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dk.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tw.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kq.shxzskj.cn

TS:   s.split(",")
来源：http://wc.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ak.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bd.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://bb.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nm.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://hc.shxzukj.cn

Py:   ",".join(items)
来源：http://kt.hnjuh.cn

PHP:  implode(",", $items);
来源：http://fj.bookmarksfly.cn

JS:   items.join(",")
来源：http://zf.shtwfgs.cn

TS:   items.join(",")
来源：http://gw.jctech888.com.cn

Java: String.join(",", items)
来源：http://ic.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://fs.gzmigu.cn

Ruby: items.join(",")
来源：http://ko.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://bo.521024.cn

[E09] 去除所有空白字符
来源：http://hq.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qp.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://te.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://fd.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://uc.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ag.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wj.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cz.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dz.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://pa.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cf.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wd.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://jy.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://em.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://zv.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mf.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hi.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ep.chemitech.net.cn

[E11] 反转字符串
来源：http://qy.hahajie.cn

Py:   s[::-1]
来源：http://fi.lnxyls.cn

PHP:  strrev($s);
来源：http://nh.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ct.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://cn.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ua.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zk.gzmigu.cn

Ruby: s.reverse
来源：http://km.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jt.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://su.muxihuayi.cn

Py:   s.count("a")
来源：http://al.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://mt.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://dq.huanxung.cn

TS:   s.split("a").length - 1
来源：http://qu.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tl.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://bl.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://xv.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://hs.jctech888.com.cn

[E13] 逐字符遍历
来源：http://eb.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://ss.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://in.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vf.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bp.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lr.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ac.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bi.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ri.hahajie.cn

[E14] URL 编码与 Base64
来源：http://mz.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gi.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ck.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://el.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xc.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vt.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gr.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rz.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dn.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://jo.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ss.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ky.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dw.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ud.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fw.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ve.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qu.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mz.jianghongdianzi.cn

[E16] 数字千分位
来源：http://fa.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ht.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://hf.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jj.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mv.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mg.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ip.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://px.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://mx.521024.cn

[E17] 首字母大写
来源：http://qm.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cv.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nl.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pt.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sj.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zw.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nf.bjjhwx.cn

Ruby: s.capitalize
来源：http://wx.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ko.hahajie.cn

[E18] 模板占位符替换
来源：http://qi.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mn.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qi.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bt.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qm.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pu.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bs.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eg.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rr.521024.cn

[E19] 多行文本按行拆分
来源：http://fm.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://lg.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mr.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://pu.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://nj.9csxet.cn

Java: s.lines().toList()
来源：http://qg.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://et.panjiajie.cn

Ruby: s.lines
来源：http://hg.hnjuh.cn

C#:   s.Split('\n')
来源：http://kg.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://ap.shtwfgs.cn

Py:   if not s:
来源：http://pi.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hr.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://he.nszjky.cn

TS:   if (s === "") {}
来源：http://qo.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ls.yuexingan06.cn

Go:   if s == "" {}
来源：http://mp.nszjky.cn

Ruby: if s.empty?
来源：http://gn.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://le.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://nv.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://an.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ye.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oq.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qx.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wf.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ll.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ct.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://eh.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sq.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://je.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ji.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ef.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tu.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://my.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://al.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rn.bookmarksfly.cn

================================================================================
来源：http://fq.nszjky.cn

F. 文件与目录
来源：http://es.newstarts.cn

================================================================================
来源：http://wq.gzmigu.cn

[F01] 读取整个文件
来源：http://aa.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tj.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://wn.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zi.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uo.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cd.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vi.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://dg.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://hv.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://yq.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rx.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qs.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xd.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gr.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ix.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uo.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://db.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ld.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://bz.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ul.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gt.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kw.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ix.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cl.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ce.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://tg.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qf.wgjwhj.cn

[F04] 追加写入文件
来源：http://ku.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yn.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sk.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rc.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://un.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zv.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wc.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://et.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ze.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://wm.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xy.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://bu.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://uv.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://cf.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nk.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wz.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://bi.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ej.asd995.cn

[F06] 删除文件
来源：http://dn.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://gp.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ud.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ds.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yv.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sn.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://gh.asd995.cn

Ruby: File.delete("a.txt")
来源：http://ll.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://gc.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://ee.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xg.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nk.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ao.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fe.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hc.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cn.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mr.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ev.chemitech.net.cn

[F08] 遍历目录
来源：http://vt.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ll.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fq.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://jv.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://mw.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gp.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gl.hahajie.cn

Ruby: Dir.children("dir")
来源：http://mw.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://qj.chemitech.net.cn

[F09] 获取文件大小
来源：http://ie.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://fe.521024.cn

PHP:  filesize("a.txt");
来源：http://lw.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://am.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://zq.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qf.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nf.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://mi.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ai.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://dd.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hw.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rq.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xz.nicolike.cn

TS:   path.extname("a.txt")
来源：http://tj.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ag.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yt.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fi.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zb.hnjuh.cn

[F11] 复制与移动文件
来源：http://cl.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rj.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kb.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sx.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xo.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nn.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tc.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lp.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nc.521024.cn

[F12] CSV 读写
来源：http://pi.nicolike.cn


<!-- 参考信息 -->