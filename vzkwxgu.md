代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lx.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fu.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://by.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eh.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bp.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://he.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://aw.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ea.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bl.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aw.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aj.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pe.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ky.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hf.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://op.panjiajie.cn

[D26] 数组转字符串
来源：http://yj.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ae.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://hb.colortex.cn

JS:   arr.join(", ")
来源：http://oq.szsharing.cn

TS:   arr.join(", ")
来源：http://at.9csxet.cn

Java: String.join(", ", list)
来源：http://wd.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://hn.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://ts.9csxet.cn

C#:   string.Join(", ", list)
来源：http://gt.nicolike.cn

================================================================================
来源：http://mn.lnxyls.cn

E. 字符串处理
来源：http://uh.yuexingan06.cn

================================================================================
来源：http://hl.szsharing.cn

[E01] 拼接字符串
来源：http://qa.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ty.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ko.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bg.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vj.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bq.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xk.huanxung.cn

[E02] 重复字符串
来源：http://el.shxzukj.cn

Py:   "ab" * 3
来源：http://py.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://my.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://xz.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://mn.9csxet.cn

Java: "ab".repeat(3)
来源：http://zd.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://nc.shtwfgs.cn

Ruby: "ab" * 3
来源：http://yg.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ac.hnjuh.cn

[E03] 截取子串
来源：http://jp.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ld.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uo.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nu.asd995.cn

TS:   s.slice(1, 4)
来源：http://eh.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://kd.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://co.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ej.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://qt.wgjwhj.cn

[E04] 查找子串位置
来源：http://me.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://vt.colortex.cn

PHP:  strpos($s, "x");
来源：http://yr.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ry.9csxet.cn

TS:   s.indexOf("x")
来源：http://dq.szxytkj.cn

Java: s.indexOf("x")
来源：http://ce.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://gl.nszjky.cn

Ruby: s.index("x")
来源：http://hj.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://jy.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xy.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fd.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sb.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zn.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jg.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zz.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://se.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yl.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bm.shxzskj.cn

[E06] 替换子串
来源：http://hj.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tl.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://tl.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zv.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://ll.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nj.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sy.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zr.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://mu.colortex.cn

[E07] 按分隔符拆分
来源：http://xc.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kc.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gn.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lf.hnjuh.cn

TS:   s.split(",")
来源：http://iu.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://id.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yw.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://ey.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://to.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://if.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://al.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://hu.lnxyls.cn

JS:   items.join(",")
来源：http://xg.bjjhwx.cn

TS:   items.join(",")
来源：http://zt.lnxyls.cn

Java: String.join(",", items)
来源：http://my.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://rf.shtwfgs.cn

Ruby: items.join(",")
来源：http://lr.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://vp.asd995.cn

[E09] 去除所有空白字符
来源：http://sx.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qq.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://of.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://xg.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://bd.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://sf.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://do.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://on.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xm.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://pp.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wv.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ry.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://nt.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://sr.hahajie.cn

Java: String.format("%03d", 7)
来源：http://aw.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xl.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qz.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mt.shxzskj.cn

[E11] 反转字符串
来源：http://qt.panjiajie.cn

Py:   s[::-1]
来源：http://ed.haigaiapp.cn

PHP:  strrev($s);
来源：http://jl.521024.cn

JS:   [...s].reverse().join("")
来源：http://nu.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://xe.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://au.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yj.shtwfgs.cn

Ruby: s.reverse
来源：http://mq.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kp.521024.cn

[E12] 统计某字符出现次数
来源：http://zn.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ni.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ch.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ld.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://si.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hx.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://hj.szxytkj.cn

Ruby: s.count("a")
来源：http://sa.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://cf.huanxung.cn

[E13] 逐字符遍历
来源：http://oo.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://jo.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yu.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wq.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ac.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cp.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fo.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ab.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sd.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://bs.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fq.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yw.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ni.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nf.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ea.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ak.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tl.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ti.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://jo.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://um.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mp.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nz.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zf.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mj.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gy.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iz.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://by.521024.cn

[E16] 数字千分位
来源：http://yh.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://cf.shxzukj.cn

PHP:  number_format(1234567);
来源：http://gv.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lp.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fj.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://us.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jh.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dn.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://mv.chemitech.net.cn

[E17] 首字母大写
来源：http://ma.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dx.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rg.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yc.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xk.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tu.huixiangedu.cn

Ruby: s.capitalize
来源：http://jx.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ey.shxzskj.cn

[E18] 模板占位符替换
来源：http://ue.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://md.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zw.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ed.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vf.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rz.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ve.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ky.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lx.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://zy.huanxung.cn

Py:   s.splitlines()
来源：http://zl.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bc.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://en.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://jj.lnxyls.cn

Java: s.lines().toList()
来源：http://qo.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://jn.hnjuh.cn

Ruby: s.lines
来源：http://qx.asd995.cn

C#:   s.Split('\n')
来源：http://yr.szsharing.cn

[E20] 判断字符串是否为空
来源：http://zd.newstarts.cn

Py:   if not s:
来源：http://lz.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gt.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://je.jctech888.com.cn

TS:   if (s === "") {}
来源：http://cr.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://tk.shxzskj.cn

Go:   if s == "" {}
来源：http://xs.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://lu.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vy.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://ws.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xz.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qh.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tz.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hm.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ni.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://nw.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jd.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ak.huanxung.cn

[E22] 字节长度与字符长度
来源：http://kd.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://da.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ss.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gg.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pz.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ny.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sw.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://hw.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lf.jctech888.com.cn

================================================================================
来源：http://jz.chemitech.net.cn

F. 文件与目录
来源：http://pv.shxzukj.cn

================================================================================
来源：http://yu.haigaiapp.cn

[F01] 读取整个文件
来源：http://gy.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kn.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://re.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jz.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://la.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rz.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wl.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ca.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ue.wgjwhj.cn

[F02] 逐行读取文件
来源：http://hq.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uw.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hw.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dw.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fv.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bt.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jf.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lz.colortex.cn

[F03] 写入文件（覆盖）
来源：http://fo.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ms.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yq.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cy.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://di.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://co.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ll.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://iq.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://en.shxzukj.cn

[F04] 追加写入文件
来源：http://la.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xx.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tj.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://el.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gy.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://me.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wb.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dq.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ki.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://yb.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vu.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://is.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://ww.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ni.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hv.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kz.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ni.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://ai.shxzskj.cn

[F06] 删除文件
来源：http://ww.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://le.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://fp.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iw.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rq.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bg.asd995.cn

Go:   os.Remove("a.txt")
来源：http://mb.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ml.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://ha.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://tg.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qc.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pi.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ci.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tm.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fr.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nw.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ck.wgjwhj.cn

[F08] 遍历目录
来源：http://cn.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://es.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://st.521024.cn

JS:   fs.readdirSync("dir")
来源：http://nd.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://oh.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jk.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zs.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ck.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://el.hnjuh.cn


<!-- 参考信息 -->