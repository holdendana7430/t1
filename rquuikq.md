代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://ml.lnxyls.cn

Ruby: arr.include?(x)
来源：http://uq.lnxyls.cn

C#:   list.Contains(x)
来源：http://vi.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://cx.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gh.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xo.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://um.lnxyls.cn

TS:   [...arr];
来源：http://ch.hahajie.cn

Java: new ArrayList<>(list);
来源：http://ao.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xq.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://rd.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ml.panjiajie.cn

[D23] reduce 累积计算
来源：http://fn.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ej.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://om.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ic.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://li.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vk.szxytkj.cn

Go:   // 手写循环
来源：http://zi.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mf.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sz.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://lf.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vj.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://my.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dp.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ai.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://up.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zw.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hk.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vl.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://xx.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cb.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mg.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://la.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vn.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ks.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xi.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ux.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://no.haigaiapp.cn

[D26] 数组转字符串
来源：http://xc.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://dz.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://hk.newstarts.cn

JS:   arr.join(", ")
来源：http://az.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://is.bjjhwx.cn

Java: String.join(", ", list)
来源：http://to.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://lp.hnjuh.cn

Ruby: arr.join(", ")
来源：http://wf.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://pb.huixiangedu.cn

================================================================================
来源：http://my.lnxyls.cn

E. 字符串处理
来源：http://ri.asd995.cn

================================================================================
来源：http://fm.huixiangedu.cn

[E01] 拼接字符串
来源：http://ka.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qi.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wz.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fz.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pr.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mo.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tr.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sp.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mt.bookmarksfly.cn

[E02] 重复字符串
来源：http://yf.chemitech.net.cn

Py:   "ab" * 3
来源：http://nz.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://ie.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://oj.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://pu.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://jd.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://oi.newstarts.cn

Ruby: "ab" * 3
来源：http://gp.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cm.asd995.cn

[E03] 截取子串
来源：http://lf.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gl.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qo.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bk.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://wd.nszjky.cn

Java: s.substring(1, 4)
来源：http://fo.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mv.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ug.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://fi.hahajie.cn

[E04] 查找子串位置
来源：http://io.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://my.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://kv.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ui.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ze.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ca.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://hf.panjiajie.cn

Ruby: s.index("x")
来源：http://dg.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://hk.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://th.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://it.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mc.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://je.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mq.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mu.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ll.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ne.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pi.hahajie.cn

[E06] 替换子串
来源：http://vy.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jf.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://jz.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ja.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://ot.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aj.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uo.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oi.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://kg.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://qh.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kt.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://to.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://br.jctech888.com.cn

TS:   s.split(",")
来源：http://ux.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ju.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yk.521024.cn

Ruby: s.split(",");  s.split
来源：http://fv.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wr.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://xt.huanxung.cn

Py:   ",".join(items)
来源：http://so.hahajie.cn

PHP:  implode(",", $items);
来源：http://uh.9csxet.cn

JS:   items.join(",")
来源：http://yz.jianghongdianzi.cn

TS:   items.join(",")
来源：http://cj.colortex.cn

Java: String.join(",", items)
来源：http://rp.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://vm.yuexingan06.cn

Ruby: items.join(",")
来源：http://vj.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://vq.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://zt.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zo.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://up.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://ar.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://em.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://jx.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gp.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aa.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ze.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://yw.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qt.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hl.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://ja.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://pl.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://bp.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ir.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iz.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fp.nicolike.cn

[E11] 反转字符串
来源：http://ch.hahajie.cn

Py:   s[::-1]
来源：http://qb.hnjuh.cn

PHP:  strrev($s);
来源：http://ss.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://su.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://ab.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gg.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fe.nszjky.cn

Ruby: s.reverse
来源：http://wo.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://he.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://zo.chemitech.net.cn

Py:   s.count("a")
来源：http://qu.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://yo.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://sl.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://tm.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jr.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://kd.521024.cn

Ruby: s.count("a")
来源：http://bb.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://tg.huanxung.cn

[E13] 逐字符遍历
来源：http://my.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://mo.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ah.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pr.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mh.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xn.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pl.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kk.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wt.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://yh.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sq.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dj.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://db.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ut.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pd.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qx.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qa.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oq.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://ta.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hm.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qa.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yr.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wx.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qb.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vd.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nf.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://el.asd995.cn

[E16] 数字千分位
来源：http://wh.huanxung.cn

Py:   f"{1234567:,}"
来源：http://mw.shxzukj.cn

PHP:  number_format(1234567);
来源：http://sk.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qv.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zk.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vm.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yq.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ww.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://sb.9csxet.cn

[E17] 首字母大写
来源：http://dt.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ql.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qn.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://id.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://so.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sy.muxihuayi.cn

Ruby: s.capitalize
来源：http://tr.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yl.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://mw.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ux.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dh.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://md.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bd.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gz.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://em.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nu.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jr.nicolike.cn

[E19] 多行文本按行拆分
来源：http://ou.szxytkj.cn

Py:   s.splitlines()
来源：http://mf.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cq.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://cy.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://na.gzmigu.cn

Java: s.lines().toList()
来源：http://xk.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://ro.muxihuayi.cn

Ruby: s.lines
来源：http://pd.panjiajie.cn

C#:   s.Split('\n')
来源：http://gv.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://nj.szsharing.cn

Py:   if not s:
来源：http://to.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ts.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qw.haigaiapp.cn

TS:   if (s === "") {}
来源：http://an.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://sc.asd995.cn

Go:   if s == "" {}
来源：http://wa.yuexingan06.cn

Ruby: if s.empty?
来源：http://ca.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://ac.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mg.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xf.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lw.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pu.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://zs.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vb.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fy.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://qu.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ev.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rw.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fl.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mm.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ai.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://qf.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://es.szxytkj.cn

================================================================================
来源：http://yw.chemitech.net.cn

F. 文件与目录
来源：http://br.hnjuh.cn

================================================================================
来源：http://tg.gzmigu.cn

[F01] 读取整个文件
来源：http://av.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ck.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://up.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kv.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kv.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jb.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dh.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://no.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://rs.haigaiapp.cn

[F02] 逐行读取文件
来源：http://wj.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cu.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kl.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://me.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gl.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xz.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ei.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pe.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ry.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://vo.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ae.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kl.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wd.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vb.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rg.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uo.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://mz.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hp.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://hv.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pd.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pu.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cl.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://al.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yc.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uc.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ao.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://eg.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ja.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://wl.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://cd.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://tq.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fb.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qu.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://ga.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://ya.hnjuh.cn

[F06] 删除文件
来源：http://uo.szsharing.cn

Py:   os.remove("a.txt")
来源：http://lo.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://hw.nicolike.cn


<!-- 参考信息 -->