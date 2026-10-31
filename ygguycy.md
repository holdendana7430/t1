代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eb.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hs.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://rn.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qu.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://he.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kc.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rh.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fr.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hs.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://we.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mn.huixiangedu.cn

[D26] 数组转字符串
来源：http://vu.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://uk.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://fu.bjjhwx.cn

JS:   arr.join(", ")
来源：http://fx.9csxet.cn

TS:   arr.join(", ")
来源：http://xs.muxihuayi.cn

Java: String.join(", ", list)
来源：http://nm.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://be.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://dd.huanxung.cn

C#:   string.Join(", ", list)
来源：http://lo.yuntaijiaju.cn

================================================================================
来源：http://ao.huanxung.cn

E. 字符串处理
来源：http://po.huanxung.cn

================================================================================
来源：http://ju.panjiajie.cn

[E01] 拼接字符串
来源：http://uf.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qx.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pi.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vr.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kp.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nn.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ur.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mu.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gy.muxihuayi.cn

[E02] 重复字符串
来源：http://yq.shxzukj.cn

Py:   "ab" * 3
来源：http://do.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://oe.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://dl.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://rd.hahajie.cn

Java: "ab".repeat(3)
来源：http://km.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://bv.jctech888.com.cn

Ruby: "ab" * 3
来源：http://tp.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ct.newstarts.cn

[E03] 截取子串
来源：http://gc.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nk.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oi.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uq.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://cb.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://zv.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ch.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://do.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://fd.szxytkj.cn

[E04] 查找子串位置
来源：http://gt.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://nv.nszjky.cn

PHP:  strpos($s, "x");
来源：http://sq.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sm.szxytkj.cn

TS:   s.indexOf("x")
来源：http://oy.lnxyls.cn

Java: s.indexOf("x")
来源：http://gr.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://kd.bjjhwx.cn

Ruby: s.index("x")
来源：http://cm.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://qu.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://za.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ra.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jn.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://st.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vl.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cb.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ub.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ij.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oi.shxzskj.cn

[E06] 替换子串
来源：http://xd.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://av.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://wv.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ij.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://tg.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bz.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://br.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wp.asd995.cn

C#:   s.Replace("a", "b")
来源：http://jw.hahajie.cn

[E07] 按分隔符拆分
来源：http://ug.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rj.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pc.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://er.yuntaijiaju.cn

TS:   s.split(",")
来源：http://gy.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fj.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kx.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://op.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sv.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://bh.hahajie.cn

Py:   ",".join(items)
来源：http://ad.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://vy.nicolike.cn

JS:   items.join(",")
来源：http://nm.hnjuh.cn

TS:   items.join(",")
来源：http://wx.nszjky.cn

Java: String.join(",", items)
来源：http://gs.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://wx.shtwfgs.cn

Ruby: items.join(",")
来源：http://tp.9csxet.cn

C#:   string.Join(",", items)
来源：http://oc.nszjky.cn

[E09] 去除所有空白字符
来源：http://if.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qz.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://de.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://pd.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://zr.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://iy.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ox.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kh.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yo.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://jq.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nu.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cw.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://jg.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ni.hahajie.cn

Java: String.format("%03d", 7)
来源：http://en.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sh.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ix.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fn.shxzskj.cn

[E11] 反转字符串
来源：http://xc.huanxung.cn

Py:   s[::-1]
来源：http://sn.lnxyls.cn

PHP:  strrev($s);
来源：http://ys.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://ih.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://gc.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jv.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qz.nicolike.cn

Ruby: s.reverse
来源：http://uj.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vg.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://oj.nszjky.cn

Py:   s.count("a")
来源：http://gj.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://ry.asd995.cn

JS:   s.split("a").length - 1
来源：http://px.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://rl.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://po.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://ue.yuexingan06.cn

Ruby: s.count("a")
来源：http://pd.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://ir.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://tu.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://dm.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aj.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pd.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cy.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jd.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yy.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xj.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vh.colortex.cn

[E14] URL 编码与 Base64
来源：http://zo.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xz.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jf.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hy.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eh.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vj.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ft.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tu.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rp.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://xe.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cm.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mh.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bw.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fv.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ji.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zz.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uh.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fo.haigaiapp.cn

[E16] 数字千分位
来源：http://xy.asd995.cn

Py:   f"{1234567:,}"
来源：http://jd.szxytkj.cn

PHP:  number_format(1234567);
来源：http://gm.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sp.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zv.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ak.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wo.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xq.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://lk.521024.cn

[E17] 首字母大写
来源：http://dc.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sp.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mf.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tg.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qg.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lo.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xt.newstarts.cn

Ruby: s.capitalize
来源：http://yk.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yl.shxzukj.cn

[E18] 模板占位符替换
来源：http://ne.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://su.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ye.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xd.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uh.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fs.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fo.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qx.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bn.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://zt.yuexingan06.cn

Py:   s.splitlines()
来源：http://vs.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wh.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://xw.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://yu.panjiajie.cn

Java: s.lines().toList()
来源：http://gd.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://jo.bjjhwx.cn

Ruby: s.lines
来源：http://qr.chemitech.net.cn

C#:   s.Split('\n')
来源：http://hn.asd995.cn

[E20] 判断字符串是否为空
来源：http://gi.chemitech.net.cn

Py:   if not s:
来源：http://in.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://od.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tw.521024.cn

TS:   if (s === "") {}
来源：http://dw.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://fb.haigaiapp.cn

Go:   if s == "" {}
来源：http://pk.hnjuh.cn

Ruby: if s.empty?
来源：http://pz.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://na.nszjky.cn

[E21] 超长截断加省略号
来源：http://ls.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://up.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tc.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oi.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sc.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lb.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://cn.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zb.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://li.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ah.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gj.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jn.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ek.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dx.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://du.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lv.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://wf.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cs.huixinmuqiang.cn

================================================================================
来源：http://ba.newstarts.cn

F. 文件与目录
来源：http://rj.lnxyls.cn

================================================================================
来源：http://qe.colortex.cn

[F01] 读取整个文件
来源：http://gi.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aq.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://so.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vw.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gb.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ag.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dj.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://xm.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://bi.shxzukj.cn

[F02] 逐行读取文件
来源：http://qh.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dq.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fd.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lw.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ko.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ik.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nu.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ed.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pa.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://mf.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rx.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wv.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lx.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vs.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://is.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://km.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ke.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gs.asd995.cn

[F04] 追加写入文件
来源：http://yl.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rt.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hs.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kb.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zv.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bi.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wa.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bu.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ui.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://af.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://af.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://ul.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://ju.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://zc.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yb.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://le.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://sl.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://yd.gzmigu.cn

[F06] 删除文件
来源：http://lc.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://uo.asd995.cn

PHP:  unlink("a.txt");
来源：http://je.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ti.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aj.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fk.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://cd.asd995.cn

Ruby: File.delete("a.txt")
来源：http://uc.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ym.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://tq.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jd.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uj.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gf.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://si.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qr.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gl.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xz.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nk.szsharing.cn

[F08] 遍历目录
来源：http://az.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oe.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cn.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://wa.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://zq.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ia.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dd.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://cf.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://op.bookmarksfly.cn

[F09] 获取文件大小
来源：http://tm.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://ow.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://fq.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://or.nszjky.cn


<!-- 参考信息 -->