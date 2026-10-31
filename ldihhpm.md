代发 wailian999

[D23] reduce 累积计算
来源：http://bx.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rs.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tj.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://px.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jg.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wu.muxihuayi.cn

Go:   // 手写循环
来源：http://ag.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ii.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fg.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://wt.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kx.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ez.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qk.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dj.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vf.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fb.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yk.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://pd.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oz.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sx.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gx.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cw.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cp.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://od.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ji.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zk.shxzskj.cn

[D26] 数组转字符串
来源：http://zl.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://xw.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://lw.hahajie.cn

JS:   arr.join(", ")
来源：http://sw.jctech888.com.cn

TS:   arr.join(", ")
来源：http://ak.newstarts.cn

Java: String.join(", ", list)
来源：http://er.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://qy.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://ap.hahajie.cn

C#:   string.Join(", ", list)
来源：http://iu.bjjhwx.cn

================================================================================
来源：http://vd.nicolike.cn

E. 字符串处理
来源：http://dq.szxytkj.cn

================================================================================
来源：http://bi.hnjuh.cn

[E01] 拼接字符串
来源：http://zy.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://it.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ub.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wb.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hh.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ng.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yy.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lg.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ul.yuexingan06.cn

[E02] 重复字符串
来源：http://kq.yuexingan06.cn

Py:   "ab" * 3
来源：http://hz.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://xw.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://to.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://mu.9csxet.cn

Java: "ab".repeat(3)
来源：http://im.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://fj.nszjky.cn

Ruby: "ab" * 3
来源：http://ad.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gn.yuntaijiaju.cn

[E03] 截取子串
来源：http://vn.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ho.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gb.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nr.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://ii.nszjky.cn

Java: s.substring(1, 4)
来源：http://yy.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xo.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rm.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://zi.huixiangedu.cn

[E04] 查找子串位置
来源：http://yo.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://sg.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://tl.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kx.szsharing.cn

TS:   s.indexOf("x")
来源：http://lk.hnjuh.cn

Java: s.indexOf("x")
来源：http://jk.521024.cn

Go:   strings.Index(s, "x")
来源：http://cs.newstarts.cn

Ruby: s.index("x")
来源：http://rt.asd995.cn

C#:   s.IndexOf("x")
来源：http://ix.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ci.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vi.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zt.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fw.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tm.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rh.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ld.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ih.hnjuh.cn

[E06] 替换子串
来源：http://ze.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hf.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://jw.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://le.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://dd.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dw.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xs.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uu.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://la.szsharing.cn

[E07] 按分隔符拆分
来源：http://ny.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ot.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mf.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ua.wgjwhj.cn

TS:   s.split(",")
来源：http://oh.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uq.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zx.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://jj.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cf.9csxet.cn

[E08] 数组按分隔符合并
来源：http://it.shxzskj.cn

Py:   ",".join(items)
来源：http://xk.lnxyls.cn

PHP:  implode(",", $items);
来源：http://zh.newstarts.cn

JS:   items.join(",")
来源：http://lh.newstarts.cn

TS:   items.join(",")
来源：http://bv.huixiangedu.cn

Java: String.join(",", items)
来源：http://gb.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://sr.yuexingan06.cn

Ruby: items.join(",")
来源：http://dm.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://kn.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ry.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nc.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yf.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://wo.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://qq.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ae.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yp.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tz.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mv.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://jc.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ne.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tq.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://bg.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://am.521024.cn

Java: String.format("%03d", 7)
来源：http://ei.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ty.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zh.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eg.muxihuayi.cn

[E11] 反转字符串
来源：http://dn.jctech888.com.cn

Py:   s[::-1]
来源：http://sv.huanxung.cn

PHP:  strrev($s);
来源：http://jz.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://gx.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://nn.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qo.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://um.huixiangedu.cn

Ruby: s.reverse
来源：http://ia.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kd.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://dx.haigaiapp.cn

Py:   s.count("a")
来源：http://vd.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://lb.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://qq.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ft.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://it.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://fa.yuexingan06.cn

Ruby: s.count("a")
来源：http://ry.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://go.szsharing.cn

[E13] 逐字符遍历
来源：http://cc.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://mt.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://na.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nl.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mk.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bl.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://of.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wh.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nt.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://yi.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lc.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://le.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://em.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ae.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mx.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kh.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sr.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://re.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://vg.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ae.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://li.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rq.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fc.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://re.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://er.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vu.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wk.chemitech.net.cn

[E16] 数字千分位
来源：http://jd.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://ey.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://yg.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xn.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://we.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yb.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ne.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://st.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://pc.9csxet.cn

[E17] 首字母大写
来源：http://dp.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nf.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ub.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ua.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rz.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dv.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uu.panjiajie.cn

Ruby: s.capitalize
来源：http://sn.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pc.chemitech.net.cn

[E18] 模板占位符替换
来源：http://ag.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ah.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pq.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tr.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sv.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kp.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pv.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qd.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://it.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://ko.asd995.cn

Py:   s.splitlines()
来源：http://dm.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nw.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://ud.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://lm.nszjky.cn

Java: s.lines().toList()
来源：http://xw.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://pr.haigaiapp.cn

Ruby: s.lines
来源：http://zh.hahajie.cn

C#:   s.Split('\n')
来源：http://vp.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://qn.lnxyls.cn

Py:   if not s:
来源：http://am.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kp.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iy.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ds.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://wy.jctech888.com.cn

Go:   if s == "" {}
来源：http://jh.asd995.cn

Ruby: if s.empty?
来源：http://sx.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gm.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://hi.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ny.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ex.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lp.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lp.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ph.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://rq.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ze.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://st.521024.cn

[E22] 字节长度与字符长度
来源：http://js.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://id.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fg.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yk.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qf.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zs.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yq.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://hr.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://my.nicolike.cn

================================================================================
来源：http://jx.panjiajie.cn

F. 文件与目录
来源：http://hc.nszjky.cn

================================================================================
来源：http://jj.newstarts.cn

[F01] 读取整个文件
来源：http://rd.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iw.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://wi.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dv.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hb.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vr.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zz.asd995.cn

Ruby: File.read("a.txt")
来源：http://ys.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://ju.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://oj.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mk.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wz.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qk.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ux.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gq.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oy.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cl.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xe.521024.cn

[F03] 写入文件（覆盖）
来源：http://sh.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ot.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mj.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nt.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vc.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gk.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rj.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://kr.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ej.nszjky.cn

[F04] 追加写入文件
来源：http://vu.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zk.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xs.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lz.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://he.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://di.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sr.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bf.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://hn.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cb.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://pt.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://kz.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://wo.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qm.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fc.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://lz.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://qd.9csxet.cn

[F06] 删除文件
来源：http://qo.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://sr.hahajie.cn

PHP:  unlink("a.txt");
来源：http://rz.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ea.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bu.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tp.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://wu.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://dh.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://xs.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://kl.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fm.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mx.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ac.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://li.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gp.gzmigu.cn


<!-- 参考信息 -->