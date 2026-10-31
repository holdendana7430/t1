代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gl.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sn.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yl.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xy.hahajie.cn

[E02] 重复字符串
来源：http://qs.521024.cn

Py:   "ab" * 3
来源：http://eh.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://dw.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://sn.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://qw.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ll.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://et.asd995.cn

Ruby: "ab" * 3
来源：http://xl.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nu.nicolike.cn

[E03] 截取子串
来源：http://gq.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uu.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zg.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ka.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://wl.nszjky.cn

Java: s.substring(1, 4)
来源：http://vh.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zw.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bn.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://yo.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://jf.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://wu.nszjky.cn

PHP:  strpos($s, "x");
来源：http://lg.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wi.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://xw.nszjky.cn

Java: s.indexOf("x")
来源：http://cj.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://pf.9csxet.cn

Ruby: s.index("x")
来源：http://oi.szsharing.cn

C#:   s.IndexOf("x")
来源：http://mc.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gt.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dx.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mc.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pb.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jg.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ag.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pp.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rp.huixiangedu.cn

[E06] 替换子串
来源：http://fy.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wi.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://xi.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vb.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ai.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gq.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bl.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xv.colortex.cn

C#:   s.Replace("a", "b")
来源：http://uv.huanxung.cn

[E07] 按分隔符拆分
来源：http://jd.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mi.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yw.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bp.huixiangedu.cn

TS:   s.split(",")
来源：http://ue.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bi.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hh.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://si.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tk.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://rk.jctech888.com.cn

Py:   ",".join(items)
来源：http://ww.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://wc.nicolike.cn

JS:   items.join(",")
来源：http://yt.gzmigu.cn

TS:   items.join(",")
来源：http://lg.wgjwhj.cn

Java: String.join(",", items)
来源：http://ji.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://wn.huixiangedu.cn

Ruby: items.join(",")
来源：http://xn.panjiajie.cn

C#:   string.Join(",", items)
来源：http://cz.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://mq.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mm.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ig.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://jb.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ql.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://lo.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ph.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ei.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ci.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://xt.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rw.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nr.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://zf.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://er.newstarts.cn

Java: String.format("%03d", 7)
来源：http://pm.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dv.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ia.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://su.szxytkj.cn

[E11] 反转字符串
来源：http://lj.haigaiapp.cn

Py:   s[::-1]
来源：http://zc.gzmigu.cn

PHP:  strrev($s);
来源：http://kj.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://hv.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://fx.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pm.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pe.nszjky.cn

Ruby: s.reverse
来源：http://ek.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://re.nszjky.cn

[E12] 统计某字符出现次数
来源：http://ms.bookmarksfly.cn

Py:   s.count("a")
来源：http://yt.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ci.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://md.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://nu.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sv.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://sy.lnxyls.cn

Ruby: s.count("a")
来源：http://gb.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://ll.panjiajie.cn

[E13] 逐字符遍历
来源：http://bg.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://wq.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ne.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pt.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fp.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ai.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ff.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rk.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://an.nszjky.cn

[E14] URL 编码与 Base64
来源：http://hw.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pb.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ak.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hl.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zc.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pk.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ws.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qk.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ak.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://kp.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yk.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mj.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wt.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vz.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bw.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rq.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yn.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cl.newstarts.cn

[E16] 数字千分位
来源：http://dr.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://vb.9csxet.cn

PHP:  number_format(1234567);
来源：http://mb.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ht.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wv.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vq.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bx.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zv.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ru.jctech888.com.cn

[E17] 首字母大写
来源：http://jq.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dn.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zs.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qp.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pv.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ok.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bn.shtwfgs.cn

Ruby: s.capitalize
来源：http://so.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dr.szsharing.cn

[E18] 模板占位符替换
来源：http://jn.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gj.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mn.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qg.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eb.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ud.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zh.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gj.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vf.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://up.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://kw.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qu.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://qu.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://gb.bookmarksfly.cn

Java: s.lines().toList()
来源：http://kn.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://jn.shtwfgs.cn

Ruby: s.lines
来源：http://gd.szxytkj.cn

C#:   s.Split('\n')
来源：http://dd.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://lk.huixinmuqiang.cn

Py:   if not s:
来源：http://wy.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sa.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uj.hnjuh.cn

TS:   if (s === "") {}
来源：http://aa.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://ga.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://fr.nicolike.cn

Ruby: if s.empty?
来源：http://vl.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iq.colortex.cn

[E21] 超长截断加省略号
来源：http://bq.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vu.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sm.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ei.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ch.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://fu.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nn.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ym.hahajie.cn

[E22] 字节长度与字符长度
来源：http://bk.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gh.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://do.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fi.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://da.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wf.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://zx.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vc.chemitech.net.cn

================================================================================
来源：http://vf.lnxyls.cn

F. 文件与目录
来源：http://vi.szxytkj.cn

================================================================================
来源：http://mk.wgjwhj.cn

[F01] 读取整个文件
来源：http://oi.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jg.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yi.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vg.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ca.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rl.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sy.szsharing.cn

Ruby: File.read("a.txt")
来源：http://lt.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://zg.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://bb.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pl.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aq.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ij.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wo.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lx.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ii.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mu.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kb.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://tb.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mi.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nm.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xn.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gh.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zk.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ff.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://wv.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ar.colortex.cn

[F04] 追加写入文件
来源：http://ia.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vr.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nr.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qo.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lt.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ws.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oo.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qw.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aq.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://xt.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://il.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://jd.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://kj.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ha.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cd.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zn.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://ss.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://db.jctech888.com.cn

[F06] 删除文件
来源：http://dj.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://lt.colortex.cn

PHP:  unlink("a.txt");
来源：http://al.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pz.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aj.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yr.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://oq.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://xf.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://uz.521024.cn

[F07] 创建目录（含多级）
来源：http://md.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rv.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bb.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wf.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yi.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ga.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cg.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wm.shtwfgs.cn

[F08] 遍历目录
来源：http://dh.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tt.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nk.521024.cn

JS:   fs.readdirSync("dir")
来源：http://vj.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://iy.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://db.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tr.asd995.cn

Ruby: Dir.children("dir")
来源：http://kj.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://vi.nicolike.cn

[F09] 获取文件大小
来源：http://rx.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://eb.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://bc.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://ly.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://bw.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xr.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wr.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://kx.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://pp.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dh.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lk.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xd.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pk.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://qh.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://em.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://er.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sa.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ud.lnxyls.cn

[F11] 复制与移动文件
来源：http://uq.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ll.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://em.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ou.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cp.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://en.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ou.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bv.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ax.muxihuayi.cn

[F12] CSV 读写
来源：http://gk.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hw.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://si.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sg.yuntaijiaju.cn

TS:   // 同上
来源：http://ag.newstarts.cn


<!-- 参考信息 -->