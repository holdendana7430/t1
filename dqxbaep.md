代发 wailian999

Java: new ArrayList<>(list);
来源：http://em.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qz.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://xy.szxytkj.cn

C#:   new List<int>(list);
来源：http://wl.asd995.cn

[D23] reduce 累积计算
来源：http://js.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nc.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gy.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ms.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mu.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qt.panjiajie.cn

Go:   // 手写循环
来源：http://sj.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hv.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aw.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://yh.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ui.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oa.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xw.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ez.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gs.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hh.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nb.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qd.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://qp.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cp.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sz.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rc.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ld.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nn.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yo.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xa.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mo.521024.cn

[D26] 数组转字符串
来源：http://nv.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://hx.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://za.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://pf.jctech888.com.cn

TS:   arr.join(", ")
来源：http://gd.shtwfgs.cn

Java: String.join(", ", list)
来源：http://wn.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://mo.gzmigu.cn

Ruby: arr.join(", ")
来源：http://af.hahajie.cn

C#:   string.Join(", ", list)
来源：http://iv.huixinmuqiang.cn

================================================================================
来源：http://bx.shxzukj.cn

E. 字符串处理
来源：http://xo.521024.cn

================================================================================
来源：http://gx.huanxung.cn

[E01] 拼接字符串
来源：http://br.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://np.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pn.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sb.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ta.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://so.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bz.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mf.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jl.gzmigu.cn

[E02] 重复字符串
来源：http://sp.colortex.cn

Py:   "ab" * 3
来源：http://xb.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://ot.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://yh.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://ys.hnjuh.cn

Java: "ab".repeat(3)
来源：http://zl.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://ms.szsharing.cn

Ruby: "ab" * 3
来源：http://kz.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tn.shxzukj.cn

[E03] 截取子串
来源：http://rc.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vh.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vf.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vc.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://cr.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://su.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ew.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rp.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://um.hahajie.cn

[E04] 查找子串位置
来源：http://zb.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://gz.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://uv.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ty.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://po.bjjhwx.cn

Java: s.indexOf("x")
来源：http://pc.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://ga.chemitech.net.cn

Ruby: s.index("x")
来源：http://ol.szsharing.cn

C#:   s.IndexOf("x")
来源：http://oq.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qa.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pa.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ss.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jb.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lf.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ti.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bm.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jb.panjiajie.cn

[E06] 替换子串
来源：http://yo.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gq.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://sj.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wn.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://cq.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://go.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mm.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yy.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://fx.colortex.cn

[E07] 按分隔符拆分
来源：http://ei.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://it.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uw.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gu.yuexingan06.cn

TS:   s.split(",")
来源：http://sm.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pc.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rt.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://qu.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yr.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://is.szxytkj.cn

Py:   ",".join(items)
来源：http://dv.szxytkj.cn

PHP:  implode(",", $items);
来源：http://hl.szxytkj.cn

JS:   items.join(",")
来源：http://lj.shxzskj.cn

TS:   items.join(",")
来源：http://ge.szxytkj.cn

Java: String.join(",", items)
来源：http://tl.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://ij.newstarts.cn

Ruby: items.join(",")
来源：http://at.521024.cn

C#:   string.Join(",", items)
来源：http://mv.asd995.cn

[E09] 去除所有空白字符
来源：http://mz.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ik.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ab.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://en.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://id.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://hu.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://io.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://md.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cy.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://qp.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pb.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://am.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ih.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://yr.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ke.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://et.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rh.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jn.colortex.cn

[E11] 反转字符串
来源：http://cf.panjiajie.cn

Py:   s[::-1]
来源：http://ng.asd995.cn

PHP:  strrev($s);
来源：http://kh.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://nj.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://sr.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uf.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ma.shxzskj.cn

Ruby: s.reverse
来源：http://zz.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vu.asd995.cn

[E12] 统计某字符出现次数
来源：http://uy.hnjuh.cn

Py:   s.count("a")
来源：http://do.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ro.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://wy.nicolike.cn

TS:   s.split("a").length - 1
来源：http://kx.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bx.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://ez.nicolike.cn

Ruby: s.count("a")
来源：http://la.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://xl.hahajie.cn

[E13] 逐字符遍历
来源：http://rk.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://vn.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ue.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://te.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://td.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://on.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://df.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://en.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qo.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://ow.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lr.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ca.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dp.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ge.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kg.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qc.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ck.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hq.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://aw.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bl.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ah.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gc.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xo.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ep.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uf.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uj.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kf.9csxet.cn

[E16] 数字千分位
来源：http://lx.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://tt.asd995.cn

PHP:  number_format(1234567);
来源：http://el.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zq.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hx.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ux.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lb.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fg.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ee.nszjky.cn

[E17] 首字母大写
来源：http://dl.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ka.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ix.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ts.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ye.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ub.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://re.asd995.cn

Ruby: s.capitalize
来源：http://gq.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ec.nicolike.cn

[E18] 模板占位符替换
来源：http://en.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ps.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hg.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zs.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mx.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dl.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zf.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hr.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ix.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://da.bjjhwx.cn

Py:   s.splitlines()
来源：http://xx.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gd.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://va.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://tv.haigaiapp.cn

Java: s.lines().toList()
来源：http://hh.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://xt.wgjwhj.cn

Ruby: s.lines
来源：http://eo.lnxyls.cn

C#:   s.Split('\n')
来源：http://wr.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://vl.nicolike.cn

Py:   if not s:
来源：http://wp.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pf.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dk.lnxyls.cn

TS:   if (s === "") {}
来源：http://mf.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://gh.colortex.cn

Go:   if s == "" {}
来源：http://st.chemitech.net.cn

Ruby: if s.empty?
来源：http://yl.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hh.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://un.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eh.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mo.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rc.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xm.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xu.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://pk.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ju.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://la.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://jz.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lc.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ce.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wr.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://db.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kh.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vv.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://xs.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aw.9csxet.cn

================================================================================
来源：http://pf.asd995.cn

F. 文件与目录
来源：http://rf.yuntaijiaju.cn

================================================================================
来源：http://uf.asd995.cn

[F01] 读取整个文件
来源：http://zi.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qt.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://ui.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zl.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jo.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sf.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cg.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://jn.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://od.gzmigu.cn

[F02] 逐行读取文件
来源：http://rj.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://az.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xo.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://po.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pw.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ry.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iu.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pu.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://vz.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vv.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dp.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ij.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pp.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qs.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zd.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://gd.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://au.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://pr.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ib.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hd.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tt.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pz.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://et.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qp.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zw.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sr.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://wi.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ev.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ag.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://gh.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://qa.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ka.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sx.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://iz.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ck.szxytkj.cn

[F06] 删除文件
来源：http://gv.hahajie.cn

Py:   os.remove("a.txt")
来源：http://ej.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://qf.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://of.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ex.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gf.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://go.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://eo.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://sx.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://ua.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cz.wgjwhj.cn


<!-- 参考信息 -->