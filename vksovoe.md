代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rg.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pf.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ap.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mh.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xu.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qa.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mh.shxzukj.cn

[D26] 数组转字符串
来源：http://pb.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://ok.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://bi.gzmigu.cn

JS:   arr.join(", ")
来源：http://an.521024.cn

TS:   arr.join(", ")
来源：http://nn.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hp.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://dm.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://iw.9csxet.cn

C#:   string.Join(", ", list)
来源：http://hz.9csxet.cn

================================================================================
来源：http://im.chemitech.net.cn

E. 字符串处理
来源：http://df.nszjky.cn

================================================================================
来源：http://cj.lnxyls.cn

[E01] 拼接字符串
来源：http://ko.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kh.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dg.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pu.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ox.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bn.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aq.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yf.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hc.szsharing.cn

[E02] 重复字符串
来源：http://rq.521024.cn

Py:   "ab" * 3
来源：http://nf.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://hv.newstarts.cn

JS:   "ab".repeat(3)
来源：http://dk.nicolike.cn

TS:   "ab".repeat(3)
来源：http://ia.colortex.cn

Java: "ab".repeat(3)
来源：http://sk.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://pg.hnjuh.cn

Ruby: "ab" * 3
来源：http://et.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vd.bookmarksfly.cn

[E03] 截取子串
来源：http://wr.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yn.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fw.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vk.huanxung.cn

TS:   s.slice(1, 4)
来源：http://yw.hahajie.cn

Java: s.substring(1, 4)
来源：http://xz.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ev.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ff.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://kb.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ya.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://dt.colortex.cn

PHP:  strpos($s, "x");
来源：http://vr.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jw.hnjuh.cn

TS:   s.indexOf("x")
来源：http://oc.szxytkj.cn

Java: s.indexOf("x")
来源：http://et.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://oy.yuexingan06.cn

Ruby: s.index("x")
来源：http://cb.huanxung.cn

C#:   s.IndexOf("x")
来源：http://kk.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ny.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jm.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://to.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rw.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gy.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lv.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dm.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ya.huanxung.cn

[E06] 替换子串
来源：http://fp.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kd.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://sy.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cp.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://oy.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ga.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eq.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ds.colortex.cn

C#:   s.Replace("a", "b")
来源：http://iw.szsharing.cn

[E07] 按分隔符拆分
来源：http://vv.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mp.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tp.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ql.521024.cn

TS:   s.split(",")
来源：http://nt.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cu.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jz.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://cz.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kz.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://zv.jctech888.com.cn

Py:   ",".join(items)
来源：http://ps.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://ev.521024.cn

JS:   items.join(",")
来源：http://rl.nszjky.cn

TS:   items.join(",")
来源：http://du.hnjuh.cn

Java: String.join(",", items)
来源：http://ko.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://op.nszjky.cn

Ruby: items.join(",")
来源：http://me.shxzskj.cn

C#:   string.Join(",", items)
来源：http://xa.szsharing.cn

[E09] 去除所有空白字符
来源：http://wt.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wo.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://of.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://id.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ly.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://gd.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sc.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xk.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aa.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://yj.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cz.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wn.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://ss.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://gb.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://bz.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ft.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dn.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sk.shxzukj.cn

[E11] 反转字符串
来源：http://vj.huixiangedu.cn

Py:   s[::-1]
来源：http://ej.shxzskj.cn

PHP:  strrev($s);
来源：http://sc.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://zc.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://qf.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nc.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ch.gzmigu.cn

Ruby: s.reverse
来源：http://uu.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xt.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://ja.huixinmuqiang.cn

Py:   s.count("a")
来源：http://zy.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://rj.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://xa.521024.cn

TS:   s.split("a").length - 1
来源：http://mq.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fa.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://fl.lnxyls.cn

Ruby: s.count("a")
来源：http://mz.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://rb.bjjhwx.cn

[E13] 逐字符遍历
来源：http://zo.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://pm.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bx.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lx.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ln.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cv.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ji.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ny.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xs.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://di.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pw.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zo.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zy.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xx.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eu.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xb.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jx.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://sd.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gn.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ce.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qe.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ks.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ay.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wt.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ij.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cv.521024.cn

[E16] 数字千分位
来源：http://xs.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://ba.521024.cn

PHP:  number_format(1234567);
来源：http://mh.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yh.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zc.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dt.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hs.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ex.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://ob.nszjky.cn

[E17] 首字母大写
来源：http://ta.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nf.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mq.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jh.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yf.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mb.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bp.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ip.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jn.szxytkj.cn

[E18] 模板占位符替换
来源：http://rl.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://du.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sk.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bs.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nk.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://me.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ma.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qm.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ho.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://zu.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://gs.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ep.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://oq.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://qz.huixiangedu.cn

Java: s.lines().toList()
来源：http://tq.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://bi.yuexingan06.cn

Ruby: s.lines
来源：http://hj.9csxet.cn

C#:   s.Split('\n')
来源：http://fm.9csxet.cn

[E20] 判断字符串是否为空
来源：http://xp.huixiangedu.cn

Py:   if not s:
来源：http://tk.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oo.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xj.muxihuayi.cn

TS:   if (s === "") {}
来源：http://bk.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://qs.huixiangedu.cn

Go:   if s == "" {}
来源：http://gc.wgjwhj.cn

Ruby: if s.empty?
来源：http://fp.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mh.huanxung.cn

[E21] 超长截断加省略号
来源：http://rk.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rf.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nm.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zl.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ac.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sv.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://pj.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kt.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bi.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://yf.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dc.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pb.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sa.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nl.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zi.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mc.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://mu.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wg.colortex.cn

================================================================================
来源：http://zq.shxzukj.cn

F. 文件与目录
来源：http://cw.521024.cn

================================================================================
来源：http://mb.newstarts.cn

[F01] 读取整个文件
来源：http://zi.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ho.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://ci.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qc.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sm.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xn.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sv.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://et.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://le.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://hh.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iy.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eq.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bu.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lz.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ar.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ez.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ci.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://xl.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ue.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://th.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vr.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dx.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pn.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bi.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ei.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sr.9csxet.cn

[F04] 追加写入文件
来源：http://fk.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ed.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kl.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://us.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wp.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wd.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wl.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://el.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mr.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://ds.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gm.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://gh.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://rk.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://as.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://of.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xz.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://yo.asd995.cn

C#:   File.Exists("a.txt")
来源：http://pd.huanxung.cn

[F06] 删除文件
来源：http://lv.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://mx.nicolike.cn

PHP:  unlink("a.txt");
来源：http://ed.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jy.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ck.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vh.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://be.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://tt.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://bb.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://lb.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ci.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tf.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ai.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kl.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://db.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fm.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eu.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hd.hahajie.cn

[F08] 遍历目录
来源：http://hn.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ud.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lk.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://eq.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://qv.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uv.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jh.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://dd.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://pl.shtwfgs.cn

[F09] 获取文件大小
来源：http://xs.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://ij.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://vi.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://bg.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://so.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vn.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yc.newstarts.cn

Ruby: File.size("a.txt")
来源：http://xz.bjjhwx.cn


<!-- 参考信息 -->