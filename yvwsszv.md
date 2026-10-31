代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bx.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ko.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zr.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mu.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tb.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://il.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pl.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://is.hahajie.cn

[E02] 重复字符串
来源：http://uo.haigaiapp.cn

Py:   "ab" * 3
来源：http://bp.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://bm.szsharing.cn

JS:   "ab".repeat(3)
来源：http://kv.huanxung.cn

TS:   "ab".repeat(3)
来源：http://nd.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ql.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://pe.jctech888.com.cn

Ruby: "ab" * 3
来源：http://xg.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mh.panjiajie.cn

[E03] 截取子串
来源：http://df.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zq.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qx.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bi.521024.cn

TS:   s.slice(1, 4)
来源：http://jo.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://hd.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sc.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nk.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://go.szsharing.cn

[E04] 查找子串位置
来源：http://vv.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://bj.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://py.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eh.newstarts.cn

TS:   s.indexOf("x")
来源：http://dj.bjjhwx.cn

Java: s.indexOf("x")
来源：http://qp.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://ag.yuexingan06.cn

Ruby: s.index("x")
来源：http://je.huanxung.cn

C#:   s.IndexOf("x")
来源：http://at.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lv.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bc.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dp.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cn.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bk.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yh.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tb.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ez.huixinmuqiang.cn

[E06] 替换子串
来源：http://km.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://op.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://qh.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://do.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://gh.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://we.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kf.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uz.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://xt.521024.cn

[E07] 按分隔符拆分
来源：http://qg.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yi.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fx.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fj.gzmigu.cn

TS:   s.split(",")
来源：http://ce.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dr.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pc.521024.cn

Ruby: s.split(",");  s.split
来源：http://be.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wq.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://yb.huixiangedu.cn

Py:   ",".join(items)
来源：http://ba.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ep.newstarts.cn

JS:   items.join(",")
来源：http://zf.asd995.cn

TS:   items.join(",")
来源：http://re.nicolike.cn

Java: String.join(",", items)
来源：http://lc.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://dp.haigaiapp.cn

Ruby: items.join(",")
来源：http://eh.panjiajie.cn

C#:   string.Join(",", items)
来源：http://my.asd995.cn

[E09] 去除所有空白字符
来源：http://jp.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sk.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ew.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://eg.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://bz.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://ur.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://np.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sq.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://nx.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ig.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mh.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ny.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://fr.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://cz.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fe.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ep.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wh.shxzukj.cn

[E11] 反转字符串
来源：http://hr.9csxet.cn

Py:   s[::-1]
来源：http://yj.nicolike.cn

PHP:  strrev($s);
来源：http://vx.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://ov.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://cd.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sn.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qs.shxzukj.cn

Ruby: s.reverse
来源：http://np.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jv.newstarts.cn

[E12] 统计某字符出现次数
来源：http://yw.shtwfgs.cn

Py:   s.count("a")
来源：http://kw.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://kd.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://nk.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ys.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mm.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://bt.muxihuayi.cn

Ruby: s.count("a")
来源：http://bh.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://iu.nszjky.cn

[E13] 逐字符遍历
来源：http://qa.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://jx.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xx.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ay.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qa.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ce.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://db.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lr.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fn.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://xo.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xy.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zk.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fa.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iu.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wt.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rk.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oj.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://mw.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uc.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iq.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xg.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nq.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gu.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rv.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mw.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ri.chemitech.net.cn

[E16] 数字千分位
来源：http://os.huanxung.cn

Py:   f"{1234567:,}"
来源：http://gr.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://eo.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://al.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lu.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://js.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ld.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vk.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://gy.yuexingan06.cn

[E17] 首字母大写
来源：http://ix.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bm.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gz.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tc.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sa.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mn.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ks.yuexingan06.cn

Ruby: s.capitalize
来源：http://rm.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lq.asd995.cn

[E18] 模板占位符替换
来源：http://tz.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://la.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kj.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qs.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sr.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://da.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cx.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yd.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jv.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://qj.chemitech.net.cn

Py:   s.splitlines()
来源：http://dg.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kk.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://tx.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://od.lnxyls.cn

Java: s.lines().toList()
来源：http://ij.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://jh.szxytkj.cn

Ruby: s.lines
来源：http://na.newstarts.cn

C#:   s.Split('\n')
来源：http://ag.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://hr.chemitech.net.cn

Py:   if not s:
来源：http://ua.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://os.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kv.bjjhwx.cn

TS:   if (s === "") {}
来源：http://ax.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://df.huanxung.cn

Go:   if s == "" {}
来源：http://iz.haigaiapp.cn

Ruby: if s.empty?
来源：http://te.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fr.hahajie.cn

[E21] 超长截断加省略号
来源：http://ay.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zc.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gy.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fn.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sw.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jk.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://zp.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gc.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fg.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://wu.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bf.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zq.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yd.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jp.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://po.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://el.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://mf.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zq.hahajie.cn

================================================================================
来源：http://pe.panjiajie.cn

F. 文件与目录
来源：http://cn.huanxung.cn

================================================================================
来源：http://wl.haigaiapp.cn

[F01] 读取整个文件
来源：http://kt.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ls.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://ny.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ou.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tt.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aw.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vu.nszjky.cn

Ruby: File.read("a.txt")
来源：http://ef.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://an.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://jo.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mf.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ed.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zv.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uf.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fh.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zn.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://br.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://da.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://on.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qj.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ra.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rp.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lb.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lk.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://nm.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://am.colortex.cn

[F04] 追加写入文件
来源：http://vc.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ag.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ci.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yf.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pf.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tx.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ki.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ql.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://pq.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ib.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ye.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://az.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ym.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nj.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ax.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://wh.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://bj.yuntaijiaju.cn

[F06] 删除文件
来源：http://ph.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://di.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://kp.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xd.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qz.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ol.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://ea.521024.cn

Ruby: File.delete("a.txt")
来源：http://sv.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://kq.521024.cn

[F07] 创建目录（含多级）
来源：http://lm.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qf.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://en.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kg.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oi.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ev.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tj.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oo.bjjhwx.cn

[F08] 遍历目录
来源：http://so.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dz.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dt.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://mo.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://wr.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yn.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ud.nszjky.cn

Ruby: Dir.children("dir")
来源：http://mc.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://mn.bjjhwx.cn

[F09] 获取文件大小
来源：http://zj.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ao.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://fu.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://xl.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://fb.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://km.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://of.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://bx.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://pk.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://wy.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lh.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fn.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dk.9csxet.cn

TS:   path.extname("a.txt")
来源：http://nc.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mx.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fd.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dq.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://em.szsharing.cn

[F11] 复制与移动文件
来源：http://cy.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yw.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://te.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rt.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xx.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ua.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sq.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kj.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vr.huixinmuqiang.cn

[F12] CSV 读写
来源：http://fx.szsharing.cn


<!-- 参考信息 -->