代发 wailian999

[D23] reduce 累积计算
来源：http://wv.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mx.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ez.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iv.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://au.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zx.huanxung.cn

Go:   // 手写循环
来源：http://gx.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lg.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xk.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://od.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vz.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bk.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dj.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fy.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zw.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fb.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qy.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ta.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://pu.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sc.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cz.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kx.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pm.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://px.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sq.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vf.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ly.hnjuh.cn

[D26] 数组转字符串
来源：http://mv.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://dz.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://dh.colortex.cn

JS:   arr.join(", ")
来源：http://iy.szxytkj.cn

TS:   arr.join(", ")
来源：http://zg.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://zi.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://ac.huanxung.cn

Ruby: arr.join(", ")
来源：http://xj.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://yb.shxzukj.cn

================================================================================
来源：http://ul.huixinmuqiang.cn

E. 字符串处理
来源：http://hz.szsharing.cn

================================================================================
来源：http://qb.szxytkj.cn

[E01] 拼接字符串
来源：http://tt.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vv.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ha.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://td.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bs.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tj.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dk.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pq.colortex.cn

[E02] 重复字符串
来源：http://le.huanxung.cn

Py:   "ab" * 3
来源：http://hn.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://xf.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://vp.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://di.shxzukj.cn

Java: "ab".repeat(3)
来源：http://fi.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://rn.9csxet.cn

Ruby: "ab" * 3
来源：http://kp.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hp.gzmigu.cn

[E03] 截取子串
来源：http://il.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://px.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lm.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ie.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://iv.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://ie.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ce.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cp.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://pg.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://gg.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://kw.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://lr.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://re.panjiajie.cn

TS:   s.indexOf("x")
来源：http://fc.9csxet.cn

Java: s.indexOf("x")
来源：http://mx.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://bf.gzmigu.cn

Ruby: s.index("x")
来源：http://qm.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://db.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ry.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nd.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yy.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hv.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mb.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hu.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://to.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zt.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://co.chemitech.net.cn

[E06] 替换子串
来源：http://jw.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cp.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://af.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ue.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://yd.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yu.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pk.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sh.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://qz.shxzskj.cn

[E07] 按分隔符拆分
来源：http://xi.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pm.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iw.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://le.gzmigu.cn

TS:   s.split(",")
来源：http://ev.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hr.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://os.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://gr.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yv.asd995.cn

[E08] 数组按分隔符合并
来源：http://xg.bjjhwx.cn

Py:   ",".join(items)
来源：http://lt.lnxyls.cn

PHP:  implode(",", $items);
来源：http://mu.chemitech.net.cn

JS:   items.join(",")
来源：http://ci.gzmigu.cn

TS:   items.join(",")
来源：http://el.asd995.cn

Java: String.join(",", items)
来源：http://nk.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://yk.shxzskj.cn

Ruby: items.join(",")
来源：http://vq.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://oe.szsharing.cn

[E09] 去除所有空白字符
来源：http://bu.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ev.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ip.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://xr.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://rz.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://ar.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bs.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://op.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sb.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://sb.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uh.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nk.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://qd.521024.cn

TS:   "7".padStart(3, "0")
来源：http://mt.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://wx.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sp.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://op.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tq.wgjwhj.cn

[E11] 反转字符串
来源：http://pc.muxihuayi.cn

Py:   s[::-1]
来源：http://xg.nicolike.cn

PHP:  strrev($s);
来源：http://ss.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://kn.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://sa.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wi.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qy.huixinmuqiang.cn

Ruby: s.reverse
来源：http://io.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rv.9csxet.cn

[E12] 统计某字符出现次数
来源：http://vz.panjiajie.cn

Py:   s.count("a")
来源：http://xb.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://vm.asd995.cn

JS:   s.split("a").length - 1
来源：http://wy.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://xf.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nr.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://tn.haigaiapp.cn

Ruby: s.count("a")
来源：http://du.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://fz.shxzskj.cn

[E13] 逐字符遍历
来源：http://ow.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://ya.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nn.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bm.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oh.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ri.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bi.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mj.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ga.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://rq.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qt.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pb.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gw.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xh.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lk.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yl.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vz.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qu.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://eo.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sw.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vj.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xu.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dl.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ht.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wp.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rz.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qs.521024.cn

[E16] 数字千分位
来源：http://ab.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://ao.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://qu.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ty.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ed.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ht.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://au.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://os.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://il.hahajie.cn

[E17] 首字母大写
来源：http://jl.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://in.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uc.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fl.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yx.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bd.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pj.nicolike.cn

Ruby: s.capitalize
来源：http://jc.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jx.szxytkj.cn

[E18] 模板占位符替换
来源：http://eq.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cu.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gy.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ny.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fx.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ei.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qj.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ut.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gi.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ck.yuexingan06.cn

Py:   s.splitlines()
来源：http://ip.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yn.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://kj.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://tc.colortex.cn

Java: s.lines().toList()
来源：http://lk.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://dt.newstarts.cn

Ruby: s.lines
来源：http://na.huixiangedu.cn

C#:   s.Split('\n')
来源：http://rn.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://uk.muxihuayi.cn

Py:   if not s:
来源：http://gc.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vj.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nh.szxytkj.cn

TS:   if (s === "") {}
来源：http://lm.521024.cn

Java: if (s.isEmpty()) {}
来源：http://xa.jctech888.com.cn

Go:   if s == "" {}
来源：http://uw.muxihuayi.cn

Ruby: if s.empty?
来源：http://wh.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ez.shxzskj.cn

[E21] 超长截断加省略号
来源：http://lq.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ys.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tg.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zs.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://za.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rv.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ra.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wi.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ic.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://ud.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tw.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hv.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dt.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://al.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gh.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gb.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://rv.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yv.hnjuh.cn

================================================================================
来源：http://ai.gzmigu.cn

F. 文件与目录
来源：http://lg.hahajie.cn

================================================================================
来源：http://cd.nicolike.cn

[F01] 读取整个文件
来源：http://ub.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sh.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ug.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xb.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ui.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fs.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pa.huanxung.cn

Ruby: File.read("a.txt")
来源：http://ur.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://pt.gzmigu.cn

[F02] 逐行读取文件
来源：http://xy.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ux.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://go.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vp.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kd.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zi.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gk.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fw.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ho.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://ae.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yx.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xy.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mr.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qi.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dh.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bc.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ui.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sf.hahajie.cn

[F04] 追加写入文件
来源：http://th.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sq.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tm.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xz.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lt.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rs.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eo.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jl.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qa.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://wd.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://so.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://ch.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://er.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ti.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dv.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ba.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://us.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://zs.hnjuh.cn

[F06] 删除文件
来源：http://hg.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://yl.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://eo.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tn.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ol.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vd.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://vv.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://nl.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://qh.asd995.cn

[F07] 创建目录（含多级）
来源：http://ms.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fx.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tm.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://my.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ds.panjiajie.cn


<!-- 参考信息 -->