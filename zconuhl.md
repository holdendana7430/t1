代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://si.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://xq.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ec.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iq.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ws.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kj.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iz.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kc.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kr.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cl.521024.cn

[D25] Set 集合去重与交并差
来源：http://vi.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ly.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pm.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xn.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ql.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lm.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wl.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wc.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ls.hnjuh.cn

[D26] 数组转字符串
来源：http://lz.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://mz.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://pt.chemitech.net.cn

JS:   arr.join(", ")
来源：http://od.colortex.cn

TS:   arr.join(", ")
来源：http://zf.huanxung.cn

Java: String.join(", ", list)
来源：http://cs.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://bk.szxytkj.cn

Ruby: arr.join(", ")
来源：http://dq.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://te.hahajie.cn

================================================================================
来源：http://zo.521024.cn

E. 字符串处理
来源：http://ic.shxzukj.cn

================================================================================
来源：http://zn.nszjky.cn

[E01] 拼接字符串
来源：http://xt.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cw.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://af.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zr.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aq.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zn.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ti.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://he.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bw.hnjuh.cn

[E02] 重复字符串
来源：http://gn.hnjuh.cn

Py:   "ab" * 3
来源：http://ms.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://ic.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://pe.9csxet.cn

TS:   "ab".repeat(3)
来源：http://sx.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://gi.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://bu.shxzukj.cn

Ruby: "ab" * 3
来源：http://ev.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uq.huanxung.cn

[E03] 截取子串
来源：http://pq.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iq.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dd.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zq.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://zt.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://xz.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yg.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kp.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://zy.gzmigu.cn

[E04] 查找子串位置
来源：http://op.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://kv.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://ft.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cp.colortex.cn

TS:   s.indexOf("x")
来源：http://wn.wgjwhj.cn

Java: s.indexOf("x")
来源：http://sm.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://om.shxzskj.cn

Ruby: s.index("x")
来源：http://pg.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://xk.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rd.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hc.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mm.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wa.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tw.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://in.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://so.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sw.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://el.huixiangedu.cn

[E06] 替换子串
来源：http://pq.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gf.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://eg.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kh.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://se.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cx.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xk.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ru.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://wq.gzmigu.cn

[E07] 按分隔符拆分
来源：http://tl.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rd.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yk.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ea.gzmigu.cn

TS:   s.split(",")
来源：http://xd.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ha.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ov.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://yn.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vs.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ey.bookmarksfly.cn

Py:   ",".join(items)
来源：http://pe.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ua.szsharing.cn

JS:   items.join(",")
来源：http://dx.wgjwhj.cn

TS:   items.join(",")
来源：http://iw.nicolike.cn

Java: String.join(",", items)
来源：http://vi.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://kc.bjjhwx.cn

Ruby: items.join(",")
来源：http://ux.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ld.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://xr.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xt.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://do.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://hn.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://qx.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ji.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ud.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ng.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yt.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://sg.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://za.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://mq.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://qf.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://hl.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sa.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wt.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qj.bjjhwx.cn

[E11] 反转字符串
来源：http://bo.hnjuh.cn

Py:   s[::-1]
来源：http://zf.nicolike.cn

PHP:  strrev($s);
来源：http://py.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://hq.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://yy.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sr.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qf.yuntaijiaju.cn

Ruby: s.reverse
来源：http://gj.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xm.szsharing.cn

[E12] 统计某字符出现次数
来源：http://hn.shxzukj.cn

Py:   s.count("a")
来源：http://au.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://ek.newstarts.cn

JS:   s.split("a").length - 1
来源：http://uf.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://rw.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://li.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://iy.colortex.cn

Ruby: s.count("a")
来源：http://nb.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://ac.9csxet.cn

[E13] 逐字符遍历
来源：http://li.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://lh.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jf.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ex.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pn.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ej.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://li.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tc.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vb.nszjky.cn

[E14] URL 编码与 Base64
来源：http://dh.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xp.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://br.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lt.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wx.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xr.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fy.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wa.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xi.521024.cn

[E15] HTML 转义 / 反转义
来源：http://hi.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rz.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pm.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eh.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oa.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ko.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://al.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pl.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ol.gzmigu.cn

[E16] 数字千分位
来源：http://re.521024.cn

Py:   f"{1234567:,}"
来源：http://kt.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ww.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eh.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uj.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wd.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://de.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sk.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://vf.nicolike.cn

[E17] 首字母大写
来源：http://ks.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wd.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cl.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ay.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cd.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tc.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jx.szsharing.cn

Ruby: s.capitalize
来源：http://zb.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://if.shxzukj.cn

[E18] 模板占位符替换
来源：http://sz.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yt.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://os.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kv.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vt.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xw.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nj.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ib.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vg.9csxet.cn

[E19] 多行文本按行拆分
来源：http://aj.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://wm.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wk.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://mz.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://fw.lnxyls.cn

Java: s.lines().toList()
来源：http://qw.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://rx.jctech888.com.cn

Ruby: s.lines
来源：http://mp.huanxung.cn

C#:   s.Split('\n')
来源：http://da.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://qy.521024.cn

Py:   if not s:
来源：http://ze.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mf.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://rb.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://pn.gzmigu.cn

Go:   if s == "" {}
来源：http://nt.newstarts.cn

Ruby: if s.empty?
来源：http://in.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jv.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ca.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bc.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ox.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://os.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fy.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ri.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://tf.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vw.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wq.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://zy.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hg.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fu.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qm.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xz.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://il.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qx.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://gl.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pw.chemitech.net.cn

================================================================================
来源：http://wf.bjjhwx.cn

F. 文件与目录
来源：http://xp.chemitech.net.cn

================================================================================
来源：http://pz.9csxet.cn

[F01] 读取整个文件
来源：http://xo.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wl.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://re.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vy.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fv.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pq.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://su.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://kq.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://tz.panjiajie.cn

[F02] 逐行读取文件
来源：http://de.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kd.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cw.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rc.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ov.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bj.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bt.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rw.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ze.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://qu.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vt.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cf.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pt.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tk.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bv.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://di.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://tm.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qb.521024.cn

[F04] 追加写入文件
来源：http://gj.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dk.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gb.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bu.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jx.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pg.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uk.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ru.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qd.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://sz.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qu.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://cg.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://af.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://mm.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mm.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wz.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://vq.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://pd.huanxung.cn

[F06] 删除文件
来源：http://un.521024.cn

Py:   os.remove("a.txt")
来源：http://ie.9csxet.cn

PHP:  unlink("a.txt");
来源：http://dg.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pu.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yr.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jr.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://ge.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://tw.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://xi.hahajie.cn

[F07] 创建目录（含多级）
来源：http://iu.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ra.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nt.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ig.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nm.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://as.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dd.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zx.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fe.jianghongdianzi.cn

[F08] 遍历目录
来源：http://wf.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://au.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ll.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://ov.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://um.huixiangedu.cn


<!-- 参考信息 -->