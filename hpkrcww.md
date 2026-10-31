代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jf.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ow.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://op.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nr.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://td.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://su.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://az.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hw.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kn.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fb.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lh.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cy.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kd.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yk.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://td.9csxet.cn

[D26] 数组转字符串
来源：http://qf.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://ld.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://sh.hahajie.cn

JS:   arr.join(", ")
来源：http://fy.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ab.shxzukj.cn

Java: String.join(", ", list)
来源：http://ry.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://bs.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://pj.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://wa.muxihuayi.cn

================================================================================
来源：http://qk.gzmigu.cn

E. 字符串处理
来源：http://vv.bjjhwx.cn

================================================================================
来源：http://ho.bjjhwx.cn

[E01] 拼接字符串
来源：http://mx.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vd.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vv.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wv.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cq.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bu.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yu.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mn.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oq.panjiajie.cn

[E02] 重复字符串
来源：http://jd.szxytkj.cn

Py:   "ab" * 3
来源：http://hq.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://lp.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ei.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://in.huanxung.cn

Java: "ab".repeat(3)
来源：http://rl.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://qr.haigaiapp.cn

Ruby: "ab" * 3
来源：http://me.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uk.newstarts.cn

[E03] 截取子串
来源：http://om.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qh.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kg.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wu.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://ng.szsharing.cn

Java: s.substring(1, 4)
来源：http://rb.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cp.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rq.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://zs.panjiajie.cn

[E04] 查找子串位置
来源：http://sq.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://an.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://fp.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ux.nicolike.cn

TS:   s.indexOf("x")
来源：http://lx.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://pf.colortex.cn

Go:   strings.Index(s, "x")
来源：http://wt.huanxung.cn

Ruby: s.index("x")
来源：http://uj.newstarts.cn

C#:   s.IndexOf("x")
来源：http://mo.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rj.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rk.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://de.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rr.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wx.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hv.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nq.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ol.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ia.asd995.cn

[E06] 替换子串
来源：http://rk.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eq.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://se.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aa.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://ns.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fk.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rf.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nq.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://zy.nicolike.cn

[E07] 按分隔符拆分
来源：http://qx.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dl.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nk.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://co.nicolike.cn

TS:   s.split(",")
来源：http://dl.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bv.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mp.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://kt.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://am.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ec.521024.cn

Py:   ",".join(items)
来源：http://qj.asd995.cn

PHP:  implode(",", $items);
来源：http://qb.shtwfgs.cn

JS:   items.join(",")
来源：http://hr.huanxung.cn

TS:   items.join(",")
来源：http://bs.szxytkj.cn

Java: String.join(",", items)
来源：http://td.521024.cn

Go:   strings.Join(items, ",")
来源：http://yd.szxytkj.cn

Ruby: items.join(",")
来源：http://dn.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://ro.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://ln.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gr.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rx.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://qz.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://rn.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://xj.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bt.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dd.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zd.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://rk.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bj.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ax.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://fx.521024.cn

TS:   "7".padStart(3, "0")
来源：http://nb.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://el.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mv.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uv.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rl.muxihuayi.cn

[E11] 反转字符串
来源：http://op.huixiangedu.cn

Py:   s[::-1]
来源：http://qq.haigaiapp.cn

PHP:  strrev($s);
来源：http://ta.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://by.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://gg.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ir.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jg.newstarts.cn

Ruby: s.reverse
来源：http://xz.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cn.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://sg.gzmigu.cn

Py:   s.count("a")
来源：http://gh.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://rf.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://sj.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://dw.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jy.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://qf.wgjwhj.cn

Ruby: s.count("a")
来源：http://vs.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://li.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://mm.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://nw.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pr.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tb.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ay.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hs.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qd.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ll.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nr.newstarts.cn

[E14] URL 编码与 Base64
来源：http://vd.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ih.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aa.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kj.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tg.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wb.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ao.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wl.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ar.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://ei.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gy.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ma.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vs.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oe.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://od.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mz.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tk.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ia.szxytkj.cn

[E16] 数字千分位
来源：http://eh.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://mv.szsharing.cn

PHP:  number_format(1234567);
来源：http://xs.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vw.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nd.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fx.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vl.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eb.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://qs.asd995.cn

[E17] 首字母大写
来源：http://pg.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zc.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ve.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jm.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cl.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cx.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fb.hnjuh.cn

Ruby: s.capitalize
来源：http://wl.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ae.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://vu.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pb.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jf.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fn.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uz.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ay.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sl.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ig.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hr.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ma.colortex.cn

Py:   s.splitlines()
来源：http://qv.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gx.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://mx.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://qn.wgjwhj.cn

Java: s.lines().toList()
来源：http://uo.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://wp.huixinmuqiang.cn

Ruby: s.lines
来源：http://il.szsharing.cn

C#:   s.Split('\n')
来源：http://hr.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://tl.9csxet.cn

Py:   if not s:
来源：http://jc.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ov.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pg.nicolike.cn

TS:   if (s === "") {}
来源：http://wr.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ig.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://pv.lnxyls.cn

Ruby: if s.empty?
来源：http://ou.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wo.nicolike.cn

[E21] 超长截断加省略号
来源：http://ca.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yr.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://my.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ny.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xd.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://it.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ie.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nm.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ez.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ry.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nt.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wh.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lo.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://da.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oh.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://zg.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jl.bookmarksfly.cn

================================================================================
来源：http://cx.bjjhwx.cn

F. 文件与目录
来源：http://fq.szxytkj.cn

================================================================================
来源：http://wd.yuexingan06.cn

[F01] 读取整个文件
来源：http://el.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tr.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://ws.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hs.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jk.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wc.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qc.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ts.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://yw.9csxet.cn

[F02] 逐行读取文件
来源：http://xi.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kb.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gc.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ge.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xa.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gr.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://no.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xu.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lm.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://bc.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qy.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oh.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vv.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lq.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fc.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://op.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://fp.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bw.nicolike.cn

[F04] 追加写入文件
来源：http://kv.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aq.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kn.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sk.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qf.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ry.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gv.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cd.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eg.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://cl.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yj.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://va.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ce.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://gh.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bu.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xi.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://fc.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://zz.huixiangedu.cn

[F06] 删除文件
来源：http://hn.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://jg.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://nm.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zr.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://om.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rb.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://mb.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://jb.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://fi.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://qr.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mh.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kh.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vh.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rj.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xy.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zt.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qe.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.521024.cn

[F08] 遍历目录
来源：http://vo.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fb.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ls.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://jj.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://qv.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ed.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yd.colortex.cn

Ruby: Dir.children("dir")
来源：http://fh.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://el.hnjuh.cn


<!-- 参考信息 -->