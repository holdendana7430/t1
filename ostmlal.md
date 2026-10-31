代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iz.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mb.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wu.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wn.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gy.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://su.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yw.9csxet.cn

[D26] 数组转字符串
来源：http://vl.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://xv.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://pp.wgjwhj.cn

JS:   arr.join(", ")
来源：http://nq.panjiajie.cn

TS:   arr.join(", ")
来源：http://vg.wgjwhj.cn

Java: String.join(", ", list)
来源：http://wb.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://ls.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://ko.nicolike.cn

C#:   string.Join(", ", list)
来源：http://xy.shtwfgs.cn

================================================================================
来源：http://oq.521024.cn

E. 字符串处理
来源：http://sn.panjiajie.cn

================================================================================
来源：http://iw.muxihuayi.cn

[E01] 拼接字符串
来源：http://sp.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://da.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gl.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fs.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cq.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ws.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gl.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xe.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dj.nicolike.cn

[E02] 重复字符串
来源：http://tz.shxzskj.cn

Py:   "ab" * 3
来源：http://op.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://bo.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://ht.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://id.szxytkj.cn

Java: "ab".repeat(3)
来源：http://ei.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://eq.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://vv.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ry.colortex.cn

[E03] 截取子串
来源：http://ul.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dg.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://la.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ah.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://gc.newstarts.cn

Java: s.substring(1, 4)
来源：http://le.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://th.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://da.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://sb.muxihuayi.cn

[E04] 查找子串位置
来源：http://wv.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://mf.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://ie.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xi.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://wz.shxzskj.cn

Java: s.indexOf("x")
来源：http://lq.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://sf.hahajie.cn

Ruby: s.index("x")
来源：http://xr.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://sc.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ql.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dk.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fc.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vl.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lc.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://us.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cy.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jk.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yq.shxzskj.cn

[E06] 替换子串
来源：http://ub.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ii.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://tv.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://we.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://wo.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ph.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xp.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://wx.szxytkj.cn

[E07] 按分隔符拆分
来源：http://od.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dg.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wf.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ke.hahajie.cn

TS:   s.split(",")
来源：http://ph.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nc.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://az.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://so.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pf.9csxet.cn

[E08] 数组按分隔符合并
来源：http://wi.huixiangedu.cn

Py:   ",".join(items)
来源：http://ir.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ui.yuexingan06.cn

JS:   items.join(",")
来源：http://jt.chemitech.net.cn

TS:   items.join(",")
来源：http://pr.shxzskj.cn

Java: String.join(",", items)
来源：http://bw.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://tj.haigaiapp.cn

Ruby: items.join(",")
来源：http://mr.huanxung.cn

C#:   string.Join(",", items)
来源：http://lr.huanxung.cn

[E09] 去除所有空白字符
来源：http://yz.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dj.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wb.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://ps.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://qd.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://rt.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ud.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zp.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yt.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://kj.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://co.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mz.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://qi.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://od.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://bj.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zf.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eq.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xl.szxytkj.cn

[E11] 反转字符串
来源：http://bl.bjjhwx.cn

Py:   s[::-1]
来源：http://ck.lnxyls.cn

PHP:  strrev($s);
来源：http://bq.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://qm.521024.cn

TS:   [...s].reverse().join("")
来源：http://uo.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ts.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jy.muxihuayi.cn

Ruby: s.reverse
来源：http://hg.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ys.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://np.jianghongdianzi.cn

Py:   s.count("a")
来源：http://su.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://xt.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://nk.colortex.cn

TS:   s.split("a").length - 1
来源：http://mo.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tj.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://zt.huixiangedu.cn

Ruby: s.count("a")
来源：http://tn.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://uz.wgjwhj.cn

[E13] 逐字符遍历
来源：http://sc.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://if.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qx.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lb.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ke.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ro.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fp.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jk.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jz.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://hh.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bj.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bs.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sb.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ck.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eq.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ih.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hw.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://rw.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://df.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ok.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rd.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nj.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wa.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jx.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tt.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eh.jctech888.com.cn

[E16] 数字千分位
来源：http://rq.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://yz.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ia.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rf.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://py.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zg.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bx.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ov.521024.cn

C#:   1234567.ToString("N0")
来源：http://ka.lnxyls.cn

[E17] 首字母大写
来源：http://hs.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ta.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tg.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xz.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qf.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qi.newstarts.cn

Ruby: s.capitalize
来源：http://yx.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oa.chemitech.net.cn

[E18] 模板占位符替换
来源：http://xl.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iy.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eh.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wi.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nx.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ge.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xy.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ni.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cy.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://tu.gzmigu.cn

Py:   s.splitlines()
来源：http://az.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://em.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://dk.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://vt.9csxet.cn

Java: s.lines().toList()
来源：http://je.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://qa.nszjky.cn

Ruby: s.lines
来源：http://pb.gzmigu.cn

C#:   s.Split('\n')
来源：http://rs.newstarts.cn

[E20] 判断字符串是否为空
来源：http://xg.bookmarksfly.cn

Py:   if not s:
来源：http://wm.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ec.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vj.szxytkj.cn

TS:   if (s === "") {}
来源：http://yh.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://xl.jctech888.com.cn

Go:   if s == "" {}
来源：http://pu.haigaiapp.cn

Ruby: if s.empty?
来源：http://dv.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vo.szxytkj.cn

[E21] 超长截断加省略号
来源：http://zw.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pa.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bc.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qd.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pm.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qg.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://af.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://at.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pb.colortex.cn

[E22] 字节长度与字符长度
来源：http://bd.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://df.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://td.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tg.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yh.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wm.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ik.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://ym.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jh.hnjuh.cn

================================================================================
来源：http://mn.panjiajie.cn

F. 文件与目录
来源：http://fl.panjiajie.cn

================================================================================
来源：http://qk.lnxyls.cn

[F01] 读取整个文件
来源：http://hn.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ig.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ic.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://df.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qh.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ym.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vh.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://dp.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://vj.huixiangedu.cn

[F02] 逐行读取文件
来源：http://rb.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ec.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://if.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xt.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gf.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sh.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jz.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zz.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rn.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://we.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bn.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yn.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wm.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ye.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hu.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eu.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://nw.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yn.haigaiapp.cn

[F04] 追加写入文件
来源：http://nt.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://no.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wu.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oz.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eh.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ls.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ou.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tb.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kf.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://kx.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qj.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://zp.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://ro.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://vw.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cj.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pj.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://cc.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://fr.gzmigu.cn

[F06] 删除文件
来源：http://mo.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://qo.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://bv.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ql.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vy.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fg.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://jl.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://uh.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://ah.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://cp.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kl.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vz.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xp.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ld.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wc.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ez.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vb.shxzukj.cn

[F08] 遍历目录
来源：http://kg.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wd.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kk.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://mh.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ok.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aj.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://by.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://ht.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://im.bookmarksfly.cn

[F09] 获取文件大小
来源：http://sz.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://qu.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://xs.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://gb.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://yf.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tl.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zw.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://ra.huixinmuqiang.cn


<!-- 参考信息 -->