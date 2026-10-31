代发 wailian999

[D23] reduce 累积计算
来源：http://iw.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jp.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hh.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ef.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ya.wgjwhj.cn

Go:   // 手写循环
来源：http://fb.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://at.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zl.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://tb.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pp.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vs.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vy.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yq.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zu.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sf.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sp.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://xq.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zm.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ds.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cn.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zd.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iw.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rb.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gp.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pg.colortex.cn

[D26] 数组转字符串
来源：http://tb.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://zr.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://wk.huixiangedu.cn

JS:   arr.join(", ")
来源：http://of.newstarts.cn

TS:   arr.join(", ")
来源：http://tl.jctech888.com.cn

Java: String.join(", ", list)
来源：http://lm.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://zs.521024.cn

Ruby: arr.join(", ")
来源：http://fz.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://fz.shxzukj.cn

================================================================================
来源：http://tu.shxzukj.cn

E. 字符串处理
来源：http://ki.panjiajie.cn

================================================================================
来源：http://nq.chemitech.net.cn

[E01] 拼接字符串
来源：http://le.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pu.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dy.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lu.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lg.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yp.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ra.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://br.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rq.bookmarksfly.cn

[E02] 重复字符串
来源：http://mr.panjiajie.cn

Py:   "ab" * 3
来源：http://nj.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://pq.hahajie.cn

JS:   "ab".repeat(3)
来源：http://nz.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://kw.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://kg.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://ne.gzmigu.cn

Ruby: "ab" * 3
来源：http://kj.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lo.gzmigu.cn

[E03] 截取子串
来源：http://qw.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://do.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hf.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zy.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://qj.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ta.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ab.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ux.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://wk.wgjwhj.cn

[E04] 查找子串位置
来源：http://bd.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ml.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://ow.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qa.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://lm.haigaiapp.cn

Java: s.indexOf("x")
来源：http://ip.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://kb.chemitech.net.cn

Ruby: s.index("x")
来源：http://nl.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://eb.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oe.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kn.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nf.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xx.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://he.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ud.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bj.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fc.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ud.newstarts.cn

[E06] 替换子串
来源：http://ve.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ln.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://fh.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ey.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://ke.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ru.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fm.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://et.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://ji.shxzskj.cn

[E07] 按分隔符拆分
来源：http://an.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ku.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rk.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bn.muxihuayi.cn

TS:   s.split(",")
来源：http://os.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xn.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gu.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://zs.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bb.colortex.cn

[E08] 数组按分隔符合并
来源：http://fm.nicolike.cn

Py:   ",".join(items)
来源：http://cx.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://hv.hnjuh.cn

JS:   items.join(",")
来源：http://tj.yuntaijiaju.cn

TS:   items.join(",")
来源：http://sn.chemitech.net.cn

Java: String.join(",", items)
来源：http://dk.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://fx.huixiangedu.cn

Ruby: items.join(",")
来源：http://iv.asd995.cn

C#:   string.Join(",", items)
来源：http://vy.lnxyls.cn

[E09] 去除所有空白字符
来源：http://oc.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zj.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pv.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://yb.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://fw.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://wj.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://po.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ku.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://to.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://zu.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://op.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gc.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://vd.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ky.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://al.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ps.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yq.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tv.asd995.cn

[E11] 反转字符串
来源：http://cs.shtwfgs.cn

Py:   s[::-1]
来源：http://ue.jctech888.com.cn

PHP:  strrev($s);
来源：http://qi.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://sl.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://yy.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ny.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sa.nicolike.cn

Ruby: s.reverse
来源：http://hv.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ub.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://gc.muxihuayi.cn

Py:   s.count("a")
来源：http://np.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://eh.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://du.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://rl.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fv.521024.cn

Go:   strings.Count(s, "a")
来源：http://gh.hnjuh.cn

Ruby: s.count("a")
来源：http://id.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://ft.gzmigu.cn

[E13] 逐字符遍历
来源：http://ht.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://yi.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zs.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lk.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tg.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ko.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gs.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ty.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rj.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://mw.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hj.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tc.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qc.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aq.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kf.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uc.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uw.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nv.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://sl.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ts.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://br.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wt.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bj.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ja.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sr.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lt.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ba.gzmigu.cn

[E16] 数字千分位
来源：http://bs.szsharing.cn

Py:   f"{1234567:,}"
来源：http://so.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://fq.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://da.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ps.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jw.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rm.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rk.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://hb.jianghongdianzi.cn

[E17] 首字母大写
来源：http://fm.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zs.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oq.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uo.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qv.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dw.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uk.wgjwhj.cn

Ruby: s.capitalize
来源：http://eb.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://un.hnjuh.cn

[E18] 模板占位符替换
来源：http://sk.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ke.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bt.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vo.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vo.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kc.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ys.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ej.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://to.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://is.hahajie.cn

Py:   s.splitlines()
来源：http://xl.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ih.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://pu.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://vr.panjiajie.cn

Java: s.lines().toList()
来源：http://zp.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://ds.huixiangedu.cn

Ruby: s.lines
来源：http://ir.yuexingan06.cn

C#:   s.Split('\n')
来源：http://lu.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://ny.shtwfgs.cn

Py:   if not s:
来源：http://pt.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wk.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wl.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://qu.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://no.shxzukj.cn

Go:   if s == "" {}
来源：http://zg.shxzukj.cn

Ruby: if s.empty?
来源：http://hc.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bv.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://qm.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nd.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://on.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://se.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://my.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uj.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://vw.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fz.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fn.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://pm.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jb.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mc.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vq.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yg.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yu.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vu.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://hu.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tp.shxzukj.cn

================================================================================
来源：http://ft.shxzukj.cn

F. 文件与目录
来源：http://ln.asd995.cn

================================================================================
来源：http://ey.szxytkj.cn

[F01] 读取整个文件
来源：http://it.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gn.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://as.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vh.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gx.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://so.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ck.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ww.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://yt.bjjhwx.cn

[F02] 逐行读取文件
来源：http://cy.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zn.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://an.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fn.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cr.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tw.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cg.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fl.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ec.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://hb.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vl.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xj.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ub.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fi.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nq.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cs.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://gi.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ag.9csxet.cn

[F04] 追加写入文件
来源：http://hg.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qb.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pw.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cv.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xm.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bz.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vc.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://te.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://an.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ig.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://zd.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://oj.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://os.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ei.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hn.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://yh.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://xc.hahajie.cn

[F06] 删除文件
来源：http://mt.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://oe.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://nt.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fk.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mj.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zs.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://lu.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://av.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ht.asd995.cn

[F07] 创建目录（含多级）
来源：http://lw.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mc.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qp.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bi.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://up.jianghongdianzi.cn


<!-- 参考信息 -->