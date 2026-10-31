代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://em.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://sw.nicolike.cn

JS:   arr.join(", ")
来源：http://qo.nicolike.cn

TS:   arr.join(", ")
来源：http://ft.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://tl.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://bh.gzmigu.cn

Ruby: arr.join(", ")
来源：http://wt.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ao.wgjwhj.cn

================================================================================
来源：http://vf.yuexingan06.cn

E. 字符串处理
来源：http://bj.yuntaijiaju.cn

================================================================================
来源：http://ft.gzmigu.cn

[E01] 拼接字符串
来源：http://wh.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ms.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tg.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ef.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tu.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://me.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lf.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ny.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fz.shtwfgs.cn

[E02] 重复字符串
来源：http://sp.huixiangedu.cn

Py:   "ab" * 3
来源：http://lj.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://xp.szsharing.cn

JS:   "ab".repeat(3)
来源：http://dz.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://qp.9csxet.cn

Java: "ab".repeat(3)
来源：http://ts.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://zq.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://qj.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vh.nszjky.cn

[E03] 截取子串
来源：http://qv.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ar.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yr.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kq.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://qj.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://xi.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nv.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pj.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://bu.huanxung.cn

[E04] 查找子串位置
来源：http://yw.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://fb.huanxung.cn

PHP:  strpos($s, "x");
来源：http://zw.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ug.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://hm.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://bn.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://jt.huanxung.cn

Ruby: s.index("x")
来源：http://er.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://bg.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://if.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://se.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dh.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ww.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ll.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ci.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://am.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cn.shxzskj.cn

[E06] 替换子串
来源：http://ty.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wz.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://lq.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ml.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://mp.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zz.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ps.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fo.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://di.shxzukj.cn

[E07] 按分隔符拆分
来源：http://nn.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://co.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lz.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qx.asd995.cn

TS:   s.split(",")
来源：http://ga.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iu.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gv.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://du.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kg.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://va.huixiangedu.cn

Py:   ",".join(items)
来源：http://nv.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://md.521024.cn

JS:   items.join(",")
来源：http://bk.bjjhwx.cn

TS:   items.join(",")
来源：http://ac.shxzukj.cn

Java: String.join(",", items)
来源：http://nq.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://yi.9csxet.cn

Ruby: items.join(",")
来源：http://sv.huanxung.cn

C#:   string.Join(",", items)
来源：http://xu.asd995.cn

[E09] 去除所有空白字符
来源：http://ld.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fl.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rj.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://ai.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ma.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://oo.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gb.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oc.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bo.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://zu.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jk.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cz.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://hw.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ed.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://lm.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kq.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vg.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yl.wgjwhj.cn

[E11] 反转字符串
来源：http://zt.nicolike.cn

Py:   s[::-1]
来源：http://pm.9csxet.cn

PHP:  strrev($s);
来源：http://ai.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://zn.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://wt.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zo.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kj.huixinmuqiang.cn

Ruby: s.reverse
来源：http://zs.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bi.colortex.cn

[E12] 统计某字符出现次数
来源：http://pd.gzmigu.cn

Py:   s.count("a")
来源：http://mg.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://th.asd995.cn

JS:   s.split("a").length - 1
来源：http://yt.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://an.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uw.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://za.shtwfgs.cn

Ruby: s.count("a")
来源：http://hp.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://zw.chemitech.net.cn

[E13] 逐字符遍历
来源：http://dx.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://qo.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lv.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rw.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ia.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dd.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vq.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vm.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://wr.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oe.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tt.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dy.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zp.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tq.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://js.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lz.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ue.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://kn.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oa.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kh.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sk.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://st.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xp.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kw.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xx.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://be.huixiangedu.cn

[E16] 数字千分位
来源：http://fj.hahajie.cn

Py:   f"{1234567:,}"
来源：http://nn.521024.cn

PHP:  number_format(1234567);
来源：http://di.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aw.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bd.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wi.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ov.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ln.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://ax.szxytkj.cn

[E17] 首字母大写
来源：http://xe.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gq.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hc.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dq.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://on.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fy.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iu.szxytkj.cn

Ruby: s.capitalize
来源：http://xi.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zm.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://ar.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://te.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sc.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mj.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eh.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lc.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bs.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qt.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://om.colortex.cn

[E19] 多行文本按行拆分
来源：http://lc.gzmigu.cn

Py:   s.splitlines()
来源：http://xp.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pp.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://wr.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://ka.panjiajie.cn

Java: s.lines().toList()
来源：http://jx.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://zf.huixiangedu.cn

Ruby: s.lines
来源：http://ku.haigaiapp.cn

C#:   s.Split('\n')
来源：http://wg.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://fo.wgjwhj.cn

Py:   if not s:
来源：http://td.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dm.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rz.chemitech.net.cn

TS:   if (s === "") {}
来源：http://we.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://fh.bookmarksfly.cn

Go:   if s == "" {}
来源：http://za.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://rf.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nv.hnjuh.cn

[E21] 超长截断加省略号
来源：http://fv.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xu.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gj.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://il.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dp.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bj.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://za.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ry.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iv.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://cv.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pf.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yl.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sr.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dd.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gg.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rb.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://bh.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://il.chemitech.net.cn

================================================================================
来源：http://fy.9csxet.cn

F. 文件与目录
来源：http://nn.nszjky.cn

================================================================================
来源：http://cc.szxytkj.cn

[F01] 读取整个文件
来源：http://eg.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pw.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://hy.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mc.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://na.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ub.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fl.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://vx.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://da.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://pm.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ko.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ke.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ou.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vd.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pq.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://er.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yh.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cq.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://kv.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ct.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bo.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sm.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ez.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pa.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fa.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://wo.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xr.szxytkj.cn

[F04] 追加写入文件
来源：http://fm.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://on.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wz.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://if.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sf.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://je.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ae.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pa.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://go.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://wb.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wd.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://jk.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://xw.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://lh.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fb.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xg.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://bv.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://mh.shxzskj.cn

[F06] 删除文件
来源：http://xj.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://it.huanxung.cn

PHP:  unlink("a.txt");
来源：http://ed.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iu.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zf.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ut.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://dw.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://dh.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://xl.9csxet.cn

[F07] 创建目录（含多级）
来源：http://xo.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dl.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://og.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sj.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xf.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tp.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lh.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uu.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sq.nszjky.cn

[F08] 遍历目录
来源：http://pc.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yu.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://km.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://fa.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ah.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wr.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kl.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://wf.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://ty.nicolike.cn

[F09] 获取文件大小
来源：http://dq.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://kh.nicolike.cn

PHP:  filesize("a.txt");
来源：http://se.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://eb.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://ga.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ro.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jh.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://ka.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://fm.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://iu.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kz.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://im.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cm.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ku.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xm.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lb.nicolike.cn


<!-- 参考信息 -->