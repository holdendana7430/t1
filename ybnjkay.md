代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bc.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rw.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gt.hnjuh.cn

[D26] 数组转字符串
来源：http://gy.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://yg.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://vj.szxytkj.cn

JS:   arr.join(", ")
来源：http://mt.hnjuh.cn

TS:   arr.join(", ")
来源：http://rd.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://nw.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://jn.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://ha.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://ha.shxzukj.cn

================================================================================
来源：http://rf.hahajie.cn

E. 字符串处理
来源：http://wf.bookmarksfly.cn

================================================================================
来源：http://tl.bookmarksfly.cn

[E01] 拼接字符串
来源：http://rf.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mx.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hd.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://co.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rq.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uk.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ac.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wg.yuexingan06.cn

[E02] 重复字符串
来源：http://qz.nicolike.cn

Py:   "ab" * 3
来源：http://zz.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://cg.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://lm.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ga.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://sr.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://wz.lnxyls.cn

Ruby: "ab" * 3
来源：http://yp.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ka.bookmarksfly.cn

[E03] 截取子串
来源：http://wo.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wf.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bg.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xu.colortex.cn

TS:   s.slice(1, 4)
来源：http://kd.hahajie.cn

Java: s.substring(1, 4)
来源：http://pa.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uz.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pw.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://vj.huanxung.cn

[E04] 查找子串位置
来源：http://cg.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://yh.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://kv.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xy.huanxung.cn

TS:   s.indexOf("x")
来源：http://cu.hahajie.cn

Java: s.indexOf("x")
来源：http://mb.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://rg.chemitech.net.cn

Ruby: s.index("x")
来源：http://gs.521024.cn

C#:   s.IndexOf("x")
来源：http://yk.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dh.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://af.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mt.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wr.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gh.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://om.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://py.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uy.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yy.nicolike.cn

[E06] 替换子串
来源：http://yk.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jk.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://tr.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tk.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://jk.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fq.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jt.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://zx.huanxung.cn

[E07] 按分隔符拆分
来源：http://aq.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tq.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xu.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://by.szsharing.cn

TS:   s.split(",")
来源：http://vw.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qw.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://so.asd995.cn

Ruby: s.split(",");  s.split
来源：http://hu.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pd.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://zb.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://jc.szxytkj.cn

PHP:  implode(",", $items);
来源：http://oh.shxzskj.cn

JS:   items.join(",")
来源：http://xr.gzmigu.cn

TS:   items.join(",")
来源：http://cu.hahajie.cn

Java: String.join(",", items)
来源：http://cr.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://kq.huixiangedu.cn

Ruby: items.join(",")
来源：http://kl.nszjky.cn

C#:   string.Join(",", items)
来源：http://ca.nicolike.cn

[E09] 去除所有空白字符
来源：http://xv.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uj.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sb.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://tt.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://cz.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://fd.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uo.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qo.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ti.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://ck.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mu.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pl.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://ua.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://jc.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://fm.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kb.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jh.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fn.jianghongdianzi.cn

[E11] 反转字符串
来源：http://zo.muxihuayi.cn

Py:   s[::-1]
来源：http://jj.nicolike.cn

PHP:  strrev($s);
来源：http://kh.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://af.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://ig.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iu.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yk.szxytkj.cn

Ruby: s.reverse
来源：http://vb.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pa.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://lh.huixinmuqiang.cn

Py:   s.count("a")
来源：http://sn.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://kh.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://uo.nszjky.cn

TS:   s.split("a").length - 1
来源：http://ab.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jy.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://er.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://zz.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://au.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://es.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://br.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vq.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dk.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lo.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gp.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ag.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sj.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zx.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://ea.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://br.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uq.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sr.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nh.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ui.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vj.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qk.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ak.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://zh.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gv.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zz.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vl.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ky.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ly.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ef.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sa.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://js.szxytkj.cn

[E16] 数字千分位
来源：http://cv.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://pj.hnjuh.cn

PHP:  number_format(1234567);
来源：http://el.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://po.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pr.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lt.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qf.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eg.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://dm.colortex.cn

[E17] 首字母大写
来源：http://gb.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tq.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://it.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oh.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bt.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nn.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wh.shtwfgs.cn

Ruby: s.capitalize
来源：http://id.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rl.colortex.cn

[E18] 模板占位符替换
来源：http://qn.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ty.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ul.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yg.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pb.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hq.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fz.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ez.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cz.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ab.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ee.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tr.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://xr.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://cv.muxihuayi.cn

Java: s.lines().toList()
来源：http://ms.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://dd.muxihuayi.cn

Ruby: s.lines
来源：http://bd.chemitech.net.cn

C#:   s.Split('\n')
来源：http://go.9csxet.cn

[E20] 判断字符串是否为空
来源：http://mt.wgjwhj.cn

Py:   if not s:
来源：http://cb.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qy.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vm.shxzskj.cn

TS:   if (s === "") {}
来源：http://wk.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ur.gzmigu.cn

Go:   if s == "" {}
来源：http://pa.muxihuayi.cn

Ruby: if s.empty?
来源：http://hf.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zh.shxzskj.cn

[E21] 超长截断加省略号
来源：http://ga.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://us.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qc.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fd.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lg.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xf.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://up.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vh.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bf.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://wl.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ln.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://po.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kj.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ey.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kk.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sr.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://et.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tx.nicolike.cn

================================================================================
来源：http://dn.newstarts.cn

F. 文件与目录
来源：http://ur.bookmarksfly.cn

================================================================================
来源：http://ue.shxzukj.cn

[F01] 读取整个文件
来源：http://pu.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nk.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://cz.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://to.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hg.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xj.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wn.newstarts.cn

Ruby: File.read("a.txt")
来源：http://tz.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://to.huixiangedu.cn

[F02] 逐行读取文件
来源：http://rr.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ld.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nf.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ja.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://te.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vb.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jw.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pc.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://su.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://dn.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sg.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ag.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zi.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ca.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://en.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bi.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://tk.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ir.wgjwhj.cn

[F04] 追加写入文件
来源：http://mx.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ty.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rj.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://we.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://in.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nq.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://el.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ng.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qj.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://qe.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ud.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://be.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://ut.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://hg.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xm.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mw.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://he.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://gx.521024.cn

[F06] 删除文件
来源：http://ne.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://jp.huanxung.cn

PHP:  unlink("a.txt");
来源：http://xe.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rh.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xr.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://go.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://bg.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ab.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://hb.hahajie.cn

[F07] 创建目录（含多级）
来源：http://yx.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sv.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bv.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gk.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pc.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mf.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ac.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gc.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qv.gzmigu.cn

[F08] 遍历目录
来源：http://vb.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qg.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jj.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://uq.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://qc.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ne.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pu.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://nu.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://nb.chemitech.net.cn

[F09] 获取文件大小
来源：http://dv.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://fw.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://tf.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://qb.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://qe.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://va.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://is.szsharing.cn

Ruby: File.size("a.txt")
来源：http://rh.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://yn.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://wh.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qo.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hn.szxytkj.cn


<!-- 参考信息 -->