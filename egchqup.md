代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://be.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://xz.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://gd.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://fl.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cn.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dm.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vf.bjjhwx.cn

TS:   [...arr];
来源：http://zy.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://cn.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cp.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://ug.hahajie.cn

C#:   new List<int>(list);
来源：http://ma.jctech888.com.cn

[D23] reduce 累积计算
来源：http://td.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ct.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mx.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ju.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iu.shxzskj.cn

Go:   // 手写循环
来源：http://ls.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hg.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zx.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://rh.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ws.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://em.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ot.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hi.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jj.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zs.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ug.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mt.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://rz.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mx.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://se.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zq.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://es.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xu.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xf.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aa.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://um.asd995.cn

[D26] 数组转字符串
来源：http://kv.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://qx.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://xo.nicolike.cn

JS:   arr.join(", ")
来源：http://la.hahajie.cn

TS:   arr.join(", ")
来源：http://lp.bjjhwx.cn

Java: String.join(", ", list)
来源：http://ua.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://po.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://we.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://lv.colortex.cn

================================================================================
来源：http://yf.shxzskj.cn

E. 字符串处理
来源：http://kx.bookmarksfly.cn

================================================================================
来源：http://xq.nszjky.cn

[E01] 拼接字符串
来源：http://sx.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ce.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zc.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aq.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uc.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fv.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tq.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pv.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://em.jianghongdianzi.cn

[E02] 重复字符串
来源：http://mn.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://yi.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://na.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://pz.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://xj.newstarts.cn

Java: "ab".repeat(3)
来源：http://ka.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ql.lnxyls.cn

Ruby: "ab" * 3
来源：http://pu.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jk.huanxung.cn

[E03] 截取子串
来源：http://fx.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sd.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bp.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vn.521024.cn

TS:   s.slice(1, 4)
来源：http://al.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://sj.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ra.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jq.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://dg.haigaiapp.cn

[E04] 查找子串位置
来源：http://ta.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ya.nszjky.cn

PHP:  strpos($s, "x");
来源：http://tp.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nz.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ek.asd995.cn

Java: s.indexOf("x")
来源：http://zv.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://pt.yuexingan06.cn

Ruby: s.index("x")
来源：http://ea.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://je.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ip.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gx.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pu.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://th.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jw.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nj.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jh.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zq.shxzukj.cn

[E06] 替换子串
来源：http://gx.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://un.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://lu.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vl.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://rc.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sv.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tg.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rh.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://cq.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://ga.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sw.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://si.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ly.colortex.cn

TS:   s.split(",")
来源：http://ht.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fd.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lc.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://sq.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://an.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ih.hnjuh.cn

Py:   ",".join(items)
来源：http://ch.newstarts.cn

PHP:  implode(",", $items);
来源：http://th.shxzskj.cn

JS:   items.join(",")
来源：http://hl.hnjuh.cn

TS:   items.join(",")
来源：http://vu.szxytkj.cn

Java: String.join(",", items)
来源：http://ze.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://pk.bjjhwx.cn

Ruby: items.join(",")
来源：http://jh.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://qh.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ma.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zh.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bl.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://sc.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://or.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://va.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oi.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lx.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ef.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://gp.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ev.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wa.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://sp.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://wi.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://mg.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vd.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ko.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sa.huixiangedu.cn

[E11] 反转字符串
来源：http://xi.nszjky.cn

Py:   s[::-1]
来源：http://if.szxytkj.cn

PHP:  strrev($s);
来源：http://po.colortex.cn

JS:   [...s].reverse().join("")
来源：http://ni.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://pl.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jx.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tr.yuntaijiaju.cn

Ruby: s.reverse
来源：http://ud.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gb.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://pm.shxzskj.cn

Py:   s.count("a")
来源：http://db.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://vv.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ni.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://gu.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wu.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://lc.colortex.cn

Ruby: s.count("a")
来源：http://vd.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://si.panjiajie.cn

[E13] 逐字符遍历
来源：http://zh.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://yj.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nq.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nk.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hg.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hw.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://um.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dx.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tx.newstarts.cn

[E14] URL 编码与 Base64
来源：http://rx.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fy.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lp.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xd.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://em.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ay.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kv.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://re.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zn.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://hy.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fa.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bd.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kg.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://he.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xz.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wu.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ae.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yd.wgjwhj.cn

[E16] 数字千分位
来源：http://nm.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://zi.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://cd.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ap.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://si.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ad.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kr.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ct.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://uv.yuexingan06.cn

[E17] 首字母大写
来源：http://sv.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pf.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hg.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rc.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lq.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dn.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.shtwfgs.cn

Ruby: s.capitalize
来源：http://jx.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://to.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://yr.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://op.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uz.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yw.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gk.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://od.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pz.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xd.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://be.521024.cn

[E19] 多行文本按行拆分
来源：http://gp.lnxyls.cn

Py:   s.splitlines()
来源：http://vb.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jc.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://yb.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://df.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://xk.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://my.521024.cn

Ruby: s.lines
来源：http://lo.asd995.cn

C#:   s.Split('\n')
来源：http://gj.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://ps.yuntaijiaju.cn

Py:   if not s:
来源：http://lz.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xd.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uc.gzmigu.cn

TS:   if (s === "") {}
来源：http://tm.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://pg.panjiajie.cn

Go:   if s == "" {}
来源：http://mv.szxytkj.cn

Ruby: if s.empty?
来源：http://yg.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://do.nicolike.cn

[E21] 超长截断加省略号
来源：http://sp.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://az.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ms.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oy.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hh.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pw.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://jv.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ct.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ma.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://io.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fm.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jx.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ho.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://go.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oj.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://hz.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ge.bjjhwx.cn

================================================================================
来源：http://ke.haigaiapp.cn

F. 文件与目录
来源：http://kj.haigaiapp.cn

================================================================================
来源：http://za.shtwfgs.cn

[F01] 读取整个文件
来源：http://ki.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lt.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://ng.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zt.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zp.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oh.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rt.huanxung.cn

Ruby: File.read("a.txt")
来源：http://re.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://rj.gzmigu.cn

[F02] 逐行读取文件
来源：http://ah.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hf.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fc.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sl.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://li.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hb.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mr.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iz.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tj.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://yp.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gj.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sk.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ta.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lh.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ry.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://ra.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://he.colortex.cn

[F04] 追加写入文件
来源：http://ty.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pd.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rc.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gg.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://on.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rq.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hw.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iu.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ac.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://si.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rk.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://im.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://kx.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://hj.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zl.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ab.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://jg.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://yg.huixinmuqiang.cn

[F06] 删除文件
来源：http://pu.huanxung.cn

Py:   os.remove("a.txt")
来源：http://cn.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://mh.bookmarksfly.cn


<!-- 参考信息 -->