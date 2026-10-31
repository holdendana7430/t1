代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://gk.haigaiapp.cn

JS:   arr.includes(x)
来源：http://cf.szsharing.cn

TS:   arr.includes(x)
来源：http://sm.szxytkj.cn

Java: list.contains(x)
来源：http://th.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://dg.huanxung.cn

Ruby: arr.include?(x)
来源：http://oq.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://yo.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://vr.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mh.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pj.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fw.jctech888.com.cn

TS:   [...arr];
来源：http://uj.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://he.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wj.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://mk.szsharing.cn

C#:   new List<int>(list);
来源：http://fi.bjjhwx.cn

[D23] reduce 累积计算
来源：http://sz.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mo.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bn.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qv.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ax.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dw.shxzskj.cn

Go:   // 手写循环
来源：http://nu.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qj.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jv.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://aa.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eb.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ej.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://go.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zx.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gu.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gc.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lg.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ah.asd995.cn

[D25] Set 集合去重与交并差
来源：http://tg.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bs.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tm.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://va.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bw.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jq.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iw.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tm.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vp.shtwfgs.cn

[D26] 数组转字符串
来源：http://hx.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://ek.521024.cn

PHP:  implode(", ", $arr);
来源：http://nq.nszjky.cn

JS:   arr.join(", ")
来源：http://bj.muxihuayi.cn

TS:   arr.join(", ")
来源：http://ds.bjjhwx.cn

Java: String.join(", ", list)
来源：http://pf.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ef.521024.cn

Ruby: arr.join(", ")
来源：http://zy.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://ic.wgjwhj.cn

================================================================================
来源：http://nb.521024.cn

E. 字符串处理
来源：http://oj.shxzskj.cn

================================================================================
来源：http://iv.szxytkj.cn

[E01] 拼接字符串
来源：http://rp.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bc.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wk.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://su.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xm.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zz.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qq.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vc.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ts.yuexingan06.cn

[E02] 重复字符串
来源：http://rr.huanxung.cn

Py:   "ab" * 3
来源：http://hd.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://nk.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://tr.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://gu.gzmigu.cn

Java: "ab".repeat(3)
来源：http://bp.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://wi.asd995.cn

Ruby: "ab" * 3
来源：http://gw.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dx.colortex.cn

[E03] 截取子串
来源：http://yl.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vf.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gt.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rm.colortex.cn

TS:   s.slice(1, 4)
来源：http://ha.shxzskj.cn

Java: s.substring(1, 4)
来源：http://lf.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ca.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lv.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://kt.bjjhwx.cn

[E04] 查找子串位置
来源：http://sq.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://cf.szsharing.cn

PHP:  strpos($s, "x");
来源：http://xd.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qc.huanxung.cn

TS:   s.indexOf("x")
来源：http://gp.szxytkj.cn

Java: s.indexOf("x")
来源：http://vz.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://rf.shtwfgs.cn

Ruby: s.index("x")
来源：http://jo.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ee.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lk.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ss.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qm.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://if.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vc.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vf.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hx.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rx.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://du.hahajie.cn

[E06] 替换子串
来源：http://kp.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hk.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://sf.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ey.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://en.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bd.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://he.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://fl.shxzukj.cn

[E07] 按分隔符拆分
来源：http://ld.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qc.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jh.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tp.huanxung.cn

TS:   s.split(",")
来源：http://gl.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gm.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jy.521024.cn

Ruby: s.split(",");  s.split
来源：http://ro.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cx.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://xc.9csxet.cn

Py:   ",".join(items)
来源：http://pg.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://oh.lnxyls.cn

JS:   items.join(",")
来源：http://uh.huixinmuqiang.cn

TS:   items.join(",")
来源：http://cm.lnxyls.cn

Java: String.join(",", items)
来源：http://rb.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://qr.shxzukj.cn

Ruby: items.join(",")
来源：http://sm.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://ra.nicolike.cn

[E09] 去除所有空白字符
来源：http://vo.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bi.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ef.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://cp.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://en.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ov.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fl.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vu.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ng.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://yo.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qn.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://be.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ix.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://wa.hahajie.cn

Java: String.format("%03d", 7)
来源：http://ky.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://km.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vd.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pw.jianghongdianzi.cn

[E11] 反转字符串
来源：http://dr.muxihuayi.cn

Py:   s[::-1]
来源：http://lp.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://oa.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://bu.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://qf.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ei.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rz.jianghongdianzi.cn

Ruby: s.reverse
来源：http://xw.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zi.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://or.shxzskj.cn

Py:   s.count("a")
来源：http://mu.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://ry.9csxet.cn

JS:   s.split("a").length - 1
来源：http://wg.hahajie.cn

TS:   s.split("a").length - 1
来源：http://xx.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dz.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://gi.wgjwhj.cn

Ruby: s.count("a")
来源：http://yf.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://yo.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ed.colortex.cn

Py:   for ch in s: print(ch)
来源：http://go.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sh.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zi.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pg.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dx.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nw.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ib.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xc.nicolike.cn

[E14] URL 编码与 Base64
来源：http://wi.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yt.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bs.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dx.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fi.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gr.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iw.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qm.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://md.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://wp.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yd.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://di.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kj.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ed.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xp.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eh.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wt.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vn.yuexingan06.cn

[E16] 数字千分位
来源：http://gn.asd995.cn

Py:   f"{1234567:,}"
来源：http://lo.shxzskj.cn

PHP:  number_format(1234567);
来源：http://nb.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qh.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fo.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rw.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jx.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lt.asd995.cn

C#:   1234567.ToString("N0")
来源：http://jg.gzmigu.cn

[E17] 首字母大写
来源：http://kd.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wr.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ng.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cf.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hp.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://au.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ys.colortex.cn

Ruby: s.capitalize
来源：http://me.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nz.hnjuh.cn

[E18] 模板占位符替换
来源：http://fj.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ov.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ud.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jj.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sq.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ew.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ne.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://on.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hf.newstarts.cn

[E19] 多行文本按行拆分
来源：http://cn.hahajie.cn

Py:   s.splitlines()
来源：http://vu.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mk.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://an.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://rl.shxzukj.cn

Java: s.lines().toList()
来源：http://ok.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://sq.panjiajie.cn

Ruby: s.lines
来源：http://dv.haigaiapp.cn

C#:   s.Split('\n')
来源：http://qj.nszjky.cn

[E20] 判断字符串是否为空
来源：http://tx.jctech888.com.cn

Py:   if not s:
来源：http://bk.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tx.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://on.colortex.cn

TS:   if (s === "") {}
来源：http://uu.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ax.chemitech.net.cn

Go:   if s == "" {}
来源：http://qn.szsharing.cn

Ruby: if s.empty?
来源：http://tm.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mx.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://dw.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wt.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jo.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nm.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hw.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hj.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://jc.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://km.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ra.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://hj.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eq.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sg.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ng.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zv.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kx.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ad.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://ef.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zr.muxihuayi.cn

================================================================================
来源：http://kb.jctech888.com.cn

F. 文件与目录
来源：http://wz.szsharing.cn

================================================================================
来源：http://qd.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://zt.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qr.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://bc.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vb.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fa.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vj.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://od.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://dv.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://pn.yuexingan06.cn

[F02] 逐行读取文件
来源：http://wv.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rg.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ew.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://am.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gt.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wg.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hs.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gf.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://uy.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bs.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sf.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tz.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dw.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ss.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kk.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://xu.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aq.shtwfgs.cn

[F04] 追加写入文件
来源：http://gu.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wz.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bn.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dq.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://py.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ck.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bv.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://we.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://or.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ko.colortex.cn

PHP:  file_exists("a.txt");
来源：http://cp.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://fz.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://am.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://to.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hy.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://yo.nicolike.cn


<!-- 参考信息 -->