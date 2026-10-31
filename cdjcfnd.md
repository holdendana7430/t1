代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://eu.colortex.cn

JS:   arr.includes(x)
来源：http://kq.nszjky.cn

TS:   arr.includes(x)
来源：http://bq.huanxung.cn

Java: list.contains(x)
来源：http://rq.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://jo.hahajie.cn

Ruby: arr.include?(x)
来源：http://cu.szxytkj.cn

C#:   list.Contains(x)
来源：http://pj.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://mc.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gk.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://om.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ya.newstarts.cn

TS:   [...arr];
来源：http://bn.newstarts.cn

Java: new ArrayList<>(list);
来源：http://li.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pa.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ly.haigaiapp.cn

C#:   new List<int>(list);
来源：http://kq.muxihuayi.cn

[D23] reduce 累积计算
来源：http://zq.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ka.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ku.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jb.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tc.asd995.cn

Go:   // 手写循环
来源：http://gp.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ly.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kp.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://ya.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hy.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cx.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ti.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ca.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ok.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kt.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vg.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yt.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://ck.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wx.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ui.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ij.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bx.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tk.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nd.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://et.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ih.szxytkj.cn

[D26] 数组转字符串
来源：http://di.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://ew.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://yg.huixiangedu.cn

JS:   arr.join(", ")
来源：http://bz.yuexingan06.cn

TS:   arr.join(", ")
来源：http://oc.huanxung.cn

Java: String.join(", ", list)
来源：http://en.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://cm.9csxet.cn

Ruby: arr.join(", ")
来源：http://vk.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://bz.lnxyls.cn

================================================================================
来源：http://fl.gzmigu.cn

E. 字符串处理
来源：http://ej.muxihuayi.cn

================================================================================
来源：http://jy.newstarts.cn

[E01] 拼接字符串
来源：http://rk.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://za.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xt.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kv.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oo.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cr.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xm.yuexingan06.cn

[E02] 重复字符串
来源：http://sy.huixiangedu.cn

Py:   "ab" * 3
来源：http://bb.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://fg.huanxung.cn

JS:   "ab".repeat(3)
来源：http://nc.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://et.lnxyls.cn

Java: "ab".repeat(3)
来源：http://vh.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://yw.lnxyls.cn

Ruby: "ab" * 3
来源：http://hk.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yw.nicolike.cn

[E03] 截取子串
来源：http://bo.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://or.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jk.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kg.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://xh.huanxung.cn

Java: s.substring(1, 4)
来源：http://mr.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dm.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mt.521024.cn

C#:   s.Substring(1, 3)
来源：http://tx.panjiajie.cn

[E04] 查找子串位置
来源：http://pn.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://bv.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://un.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vs.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ha.panjiajie.cn

Java: s.indexOf("x")
来源：http://uv.asd995.cn

Go:   strings.Index(s, "x")
来源：http://ac.chemitech.net.cn

Ruby: s.index("x")
来源：http://le.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://wp.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lb.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xa.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ju.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yc.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://at.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qc.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://so.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ex.jianghongdianzi.cn

[E06] 替换子串
来源：http://pk.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xp.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://gi.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://si.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://aq.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wr.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wy.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://az.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://bb.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://zp.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qv.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yw.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aj.chemitech.net.cn

TS:   s.split(",")
来源：http://fm.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://py.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://as.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://ry.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cf.newstarts.cn

[E08] 数组按分隔符合并
来源：http://rk.nicolike.cn

Py:   ",".join(items)
来源：http://qp.gzmigu.cn

PHP:  implode(",", $items);
来源：http://qx.shtwfgs.cn

JS:   items.join(",")
来源：http://lq.chemitech.net.cn

TS:   items.join(",")
来源：http://yl.bookmarksfly.cn

Java: String.join(",", items)
来源：http://gz.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://xo.lnxyls.cn

Ruby: items.join(",")
来源：http://fj.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://fj.shxzukj.cn

[E09] 去除所有空白字符
来源：http://yl.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uv.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ft.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://ex.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://yl.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://uc.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ld.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cm.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qt.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://gd.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vj.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yp.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://ro.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://jo.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://rh.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vs.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zf.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wk.colortex.cn

[E11] 反转字符串
来源：http://rq.szxytkj.cn

Py:   s[::-1]
来源：http://qu.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://in.521024.cn

JS:   [...s].reverse().join("")
来源：http://wz.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://ec.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://td.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qz.521024.cn

Ruby: s.reverse
来源：http://rt.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oz.hahajie.cn

[E12] 统计某字符出现次数
来源：http://eu.9csxet.cn

Py:   s.count("a")
来源：http://vf.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://bq.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://nh.nicolike.cn

TS:   s.split("a").length - 1
来源：http://ft.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ap.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://vn.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://cj.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://qk.muxihuayi.cn

[E13] 逐字符遍历
来源：http://au.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://cr.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kc.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zs.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sx.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hv.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ul.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sc.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xs.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://qh.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pu.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bm.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ix.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qt.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eq.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nz.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nw.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bg.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://hc.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ko.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kp.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bn.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cy.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wt.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oo.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hk.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mr.chemitech.net.cn

[E16] 数字千分位
来源：http://em.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ql.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://oe.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iu.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cj.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gz.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sg.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kh.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://zz.chemitech.net.cn

[E17] 首字母大写
来源：http://kr.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rj.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://on.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cg.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fz.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bk.bjjhwx.cn

Ruby: s.capitalize
来源：http://dr.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cj.newstarts.cn

[E18] 模板占位符替换
来源：http://ik.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xh.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pv.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dg.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vi.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dv.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hs.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ys.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://va.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://cs.nicolike.cn

Py:   s.splitlines()
来源：http://ow.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yt.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://hm.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ie.szsharing.cn

Java: s.lines().toList()
来源：http://bi.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://be.shxzskj.cn

Ruby: s.lines
来源：http://sv.shxzukj.cn

C#:   s.Split('\n')
来源：http://fj.521024.cn

[E20] 判断字符串是否为空
来源：http://wd.nszjky.cn

Py:   if not s:
来源：http://bh.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mr.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zw.9csxet.cn

TS:   if (s === "") {}
来源：http://ha.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://lw.nicolike.cn

Go:   if s == "" {}
来源：http://rh.9csxet.cn

Ruby: if s.empty?
来源：http://mi.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wf.nszjky.cn

[E21] 超长截断加省略号
来源：http://zg.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eu.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uo.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mc.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vu.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://id.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jc.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://st.521024.cn

[E22] 字节长度与字符长度
来源：http://pe.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aw.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jg.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hg.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rp.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://id.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://id.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://mc.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ji.jctech888.com.cn

================================================================================
来源：http://ez.muxihuayi.cn

F. 文件与目录
来源：http://dt.szsharing.cn

================================================================================
来源：http://yp.shxzukj.cn

[F01] 读取整个文件
来源：http://hw.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zl.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://uz.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cp.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vy.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fx.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iy.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://wz.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://of.9csxet.cn

[F02] 逐行读取文件
来源：http://ia.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ka.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ns.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jf.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aa.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cw.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cf.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cz.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ag.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://ig.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lt.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ao.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://co.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bk.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zh.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://to.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ls.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eu.jctech888.com.cn

[F04] 追加写入文件
来源：http://xp.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zg.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dt.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xv.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dp.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eo.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xg.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://on.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://zc.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kd.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://qq.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://xv.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://cg.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uv.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://em.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://nm.shxzukj.cn


<!-- 参考信息 -->