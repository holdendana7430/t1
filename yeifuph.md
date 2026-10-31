代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mr.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lo.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pc.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zf.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xk.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ye.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mh.asd995.cn

[D26] 数组转字符串
来源：http://sd.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://ht.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://sq.szsharing.cn

JS:   arr.join(", ")
来源：http://fa.hnjuh.cn

TS:   arr.join(", ")
来源：http://ef.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://az.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://tj.panjiajie.cn

Ruby: arr.join(", ")
来源：http://oq.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://ju.jctech888.com.cn

================================================================================
来源：http://sn.shtwfgs.cn

E. 字符串处理
来源：http://mi.asd995.cn

================================================================================
来源：http://gz.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://se.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qd.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ss.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nr.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://db.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zj.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pu.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ri.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kd.muxihuayi.cn

[E02] 重复字符串
来源：http://qo.hnjuh.cn

Py:   "ab" * 3
来源：http://qd.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://jb.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ix.9csxet.cn

TS:   "ab".repeat(3)
来源：http://ti.newstarts.cn

Java: "ab".repeat(3)
来源：http://rz.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://zx.9csxet.cn

Ruby: "ab" * 3
来源：http://wa.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ia.colortex.cn

[E03] 截取子串
来源：http://wu.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wp.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lf.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://je.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://mq.nicolike.cn

Java: s.substring(1, 4)
来源：http://ao.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mh.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vh.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://mo.muxihuayi.cn

[E04] 查找子串位置
来源：http://cv.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://hl.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://gk.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lv.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://wg.hnjuh.cn

Java: s.indexOf("x")
来源：http://dp.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://gd.newstarts.cn

Ruby: s.index("x")
来源：http://ss.newstarts.cn

C#:   s.IndexOf("x")
来源：http://nm.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ju.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vi.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qd.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ia.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ps.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qb.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pf.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mo.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yf.colortex.cn

[E06] 替换子串
来源：http://dq.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sk.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://bk.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://xy.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bq.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lh.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://tx.shxzukj.cn

[E07] 按分隔符拆分
来源：http://fn.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ec.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hu.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://re.szxytkj.cn

TS:   s.split(",")
来源：http://wi.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yq.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uu.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://pa.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ff.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://dj.yuexingan06.cn

Py:   ",".join(items)
来源：http://ma.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://el.gzmigu.cn

JS:   items.join(",")
来源：http://cm.huanxung.cn

TS:   items.join(",")
来源：http://wo.nicolike.cn

Java: String.join(",", items)
来源：http://tp.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://yg.bjjhwx.cn

Ruby: items.join(",")
来源：http://ic.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://wd.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://tq.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://me.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bn.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://mm.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://rt.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://go.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uc.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vi.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kd.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://bh.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oo.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ei.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://nk.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://gt.newstarts.cn

Java: String.format("%03d", 7)
来源：http://ct.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ou.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ux.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pi.asd995.cn

[E11] 反转字符串
来源：http://jy.nszjky.cn

Py:   s[::-1]
来源：http://pl.huixiangedu.cn

PHP:  strrev($s);
来源：http://qy.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://ac.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://lp.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fk.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bx.gzmigu.cn

Ruby: s.reverse
来源：http://yf.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gs.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://xb.chemitech.net.cn

Py:   s.count("a")
来源：http://aa.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://sc.szsharing.cn

JS:   s.split("a").length - 1
来源：http://eb.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ho.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sx.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://rz.huanxung.cn

Ruby: s.count("a")
来源：http://yv.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://qc.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://pn.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://tc.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yj.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hy.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://of.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://md.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lp.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ma.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mf.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://me.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ys.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jm.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ef.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zg.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hr.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gn.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kk.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pq.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://ib.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ac.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xs.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oj.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kz.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://si.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://su.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lz.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rt.9csxet.cn

[E16] 数字千分位
来源：http://fq.9csxet.cn

Py:   f"{1234567:,}"
来源：http://wi.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://dv.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ge.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vd.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ia.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pb.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ow.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://ga.nicolike.cn

[E17] 首字母大写
来源：http://wu.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aa.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eq.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rk.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vz.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fg.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xu.bjjhwx.cn

Ruby: s.capitalize
来源：http://xq.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pn.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://aj.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cm.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mw.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://op.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ko.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rw.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wc.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jd.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ut.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://tr.lnxyls.cn

Py:   s.splitlines()
来源：http://ny.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cp.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://cm.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ko.szxytkj.cn

Java: s.lines().toList()
来源：http://oa.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://qd.bookmarksfly.cn

Ruby: s.lines
来源：http://np.lnxyls.cn

C#:   s.Split('\n')
来源：http://vx.nicolike.cn

[E20] 判断字符串是否为空
来源：http://ld.gzmigu.cn

Py:   if not s:
来源：http://ub.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dz.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yy.shxzukj.cn

TS:   if (s === "") {}
来源：http://ui.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://np.szsharing.cn

Go:   if s == "" {}
来源：http://ew.newstarts.cn

Ruby: if s.empty?
来源：http://jk.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ce.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://kf.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tt.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yv.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kk.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nj.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ut.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://qb.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wb.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tz.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://xm.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://na.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pi.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wh.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bs.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ws.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tx.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://yj.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tj.hnjuh.cn

================================================================================
来源：http://nj.chemitech.net.cn

F. 文件与目录
来源：http://ff.hnjuh.cn

================================================================================
来源：http://cy.shtwfgs.cn

[F01] 读取整个文件
来源：http://rd.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://su.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://ny.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ge.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kl.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ab.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qz.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://zf.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ay.9csxet.cn

[F02] 逐行读取文件
来源：http://kh.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://we.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eq.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ap.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hr.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://he.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fn.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fe.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uw.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://bt.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vx.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ci.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yk.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://za.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xl.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ec.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ah.bjjhwx.cn

[F04] 追加写入文件
来源：http://ce.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yf.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xj.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ol.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lp.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ha.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vm.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lo.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ly.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ea.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://io.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://si.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://gg.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://wt.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ks.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hi.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://fx.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ai.huanxung.cn

[F06] 删除文件
来源：http://jq.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://om.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://lt.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dc.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fz.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oc.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://bb.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://dn.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://mp.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://kg.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ni.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dm.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vv.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ev.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gt.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jx.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nz.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bo.szsharing.cn

[F08] 遍历目录
来源：http://iq.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cp.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mn.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://sk.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://rk.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wo.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iq.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ly.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://vc.nszjky.cn

[F09] 获取文件大小
来源：http://vq.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://gy.huanxung.cn

PHP:  filesize("a.txt");
来源：http://jf.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ns.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://cw.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hv.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rj.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://zw.panjiajie.cn


<!-- 参考信息 -->