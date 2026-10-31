代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://eq.wgjwhj.cn

JS:   arr.includes(x)
来源：http://xh.huanxung.cn

TS:   arr.includes(x)
来源：http://jh.huixinmuqiang.cn

Java: list.contains(x)
来源：http://im.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://qt.shxzukj.cn

Ruby: arr.include?(x)
来源：http://cx.huanxung.cn

C#:   list.Contains(x)
来源：http://mz.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://ia.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gs.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bk.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sd.gzmigu.cn

TS:   [...arr];
来源：http://qj.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://jw.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hf.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://nv.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://qo.hnjuh.cn

[D23] reduce 累积计算
来源：http://hl.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ay.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mw.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://um.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ps.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ha.jianghongdianzi.cn

Go:   // 手写循环
来源：http://zv.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hn.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wq.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://or.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tq.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ma.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jw.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ie.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xt.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aa.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kp.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mr.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://xh.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cp.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ja.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bl.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wg.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wi.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pc.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ba.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rn.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://wa.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ot.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://xz.yuexingan06.cn

JS:   arr.join(", ")
来源：http://qe.nicolike.cn

TS:   arr.join(", ")
来源：http://fy.9csxet.cn

Java: String.join(", ", list)
来源：http://dw.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://nq.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://ca.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://ai.wgjwhj.cn

================================================================================
来源：http://aw.gzmigu.cn

E. 字符串处理
来源：http://nk.hnjuh.cn

================================================================================
来源：http://fo.wgjwhj.cn

[E01] 拼接字符串
来源：http://bm.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iq.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uu.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hk.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lu.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tr.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yp.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dl.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bx.jianghongdianzi.cn

[E02] 重复字符串
来源：http://fz.szxytkj.cn

Py:   "ab" * 3
来源：http://od.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://zi.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://ly.szsharing.cn

TS:   "ab".repeat(3)
来源：http://tg.9csxet.cn

Java: "ab".repeat(3)
来源：http://zc.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://vg.haigaiapp.cn

Ruby: "ab" * 3
来源：http://gj.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ha.huanxung.cn

[E03] 截取子串
来源：http://wu.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vq.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://om.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ez.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://tg.nicolike.cn

Java: s.substring(1, 4)
来源：http://vh.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wq.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ub.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://wa.nszjky.cn

[E04] 查找子串位置
来源：http://ob.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://qf.nszjky.cn

PHP:  strpos($s, "x");
来源：http://ad.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dn.szsharing.cn

TS:   s.indexOf("x")
来源：http://mt.huixiangedu.cn

Java: s.indexOf("x")
来源：http://qz.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://iv.jctech888.com.cn

Ruby: s.index("x")
来源：http://mb.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://kn.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xs.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fy.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yn.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bi.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fs.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zp.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zq.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jt.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dm.muxihuayi.cn

[E06] 替换子串
来源：http://bi.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bg.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://yq.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fx.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://su.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ey.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://up.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pu.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://mz.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://si.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vg.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xd.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zn.szxytkj.cn

TS:   s.split(",")
来源：http://ra.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ck.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kk.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://ur.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bb.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://io.huixiangedu.cn

Py:   ",".join(items)
来源：http://gy.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://gm.wgjwhj.cn

JS:   items.join(",")
来源：http://bl.shxzukj.cn

TS:   items.join(",")
来源：http://sy.jctech888.com.cn

Java: String.join(",", items)
来源：http://qs.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://jz.chemitech.net.cn

Ruby: items.join(",")
来源：http://aw.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://ox.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://nb.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sx.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ab.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://av.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://on.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://pj.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jq.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sj.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://na.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://ux.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fm.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wb.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://fj.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://mw.huanxung.cn

Java: String.format("%03d", 7)
来源：http://jx.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iu.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pz.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rq.asd995.cn

[E11] 反转字符串
来源：http://gs.9csxet.cn

Py:   s[::-1]
来源：http://vh.panjiajie.cn

PHP:  strrev($s);
来源：http://sq.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://mw.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://sq.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tz.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aj.bjjhwx.cn

Ruby: s.reverse
来源：http://ak.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dp.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://py.hnjuh.cn

Py:   s.count("a")
来源：http://rp.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://eb.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://dq.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://xs.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cr.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://ar.hahajie.cn

Ruby: s.count("a")
来源：http://tj.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://cb.colortex.cn

[E13] 逐字符遍历
来源：http://gr.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://do.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fs.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vx.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yv.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ck.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yg.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cb.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cf.huanxung.cn

[E14] URL 编码与 Base64
来源：http://xu.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vf.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rz.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bd.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dh.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wg.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bi.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yl.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://px.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://tx.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qi.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zh.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lz.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nz.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sq.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jt.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qw.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://it.nszjky.cn

[E16] 数字千分位
来源：http://jv.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://sd.huanxung.cn

PHP:  number_format(1234567);
来源：http://xc.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pg.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mi.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pb.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://es.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://on.asd995.cn

C#:   1234567.ToString("N0")
来源：http://oa.521024.cn

[E17] 首字母大写
来源：http://us.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ii.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ho.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ax.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nw.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cn.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gw.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://yl.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gt.jctech888.com.cn

[E18] 模板占位符替换
来源：http://sq.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fe.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jt.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://io.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://om.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ti.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cj.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oh.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mw.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://xa.huanxung.cn

Py:   s.splitlines()
来源：http://vf.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gz.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://pb.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://gs.nicolike.cn

Java: s.lines().toList()
来源：http://bk.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://wi.wgjwhj.cn

Ruby: s.lines
来源：http://xz.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ng.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://us.muxihuayi.cn

Py:   if not s:
来源：http://wl.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qm.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://br.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://fd.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ue.hnjuh.cn

Go:   if s == "" {}
来源：http://py.shtwfgs.cn

Ruby: if s.empty?
来源：http://gb.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ex.shxzskj.cn

[E21] 超长截断加省略号
来源：http://sb.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sa.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mr.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bk.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ui.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://se.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qo.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qc.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://br.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cf.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://em.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cc.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://li.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mn.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://th.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://eh.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ef.yuexingan06.cn

================================================================================
来源：http://fm.newstarts.cn

F. 文件与目录
来源：http://tq.haigaiapp.cn

================================================================================
来源：http://ca.nicolike.cn

[F01] 读取整个文件
来源：http://pk.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rc.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ar.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jx.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ds.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://si.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hm.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://ua.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://jx.lnxyls.cn

[F02] 逐行读取文件
来源：http://ws.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ot.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fr.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wo.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kc.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zz.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ms.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wu.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sb.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://xi.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://db.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ia.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xi.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bp.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nz.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aa.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://tu.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tw.gzmigu.cn

[F04] 追加写入文件
来源：http://nn.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ox.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cb.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iv.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jv.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://em.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pv.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bi.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://kb.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gm.asd995.cn

PHP:  file_exists("a.txt");
来源：http://rk.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://zn.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://pr.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fs.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zu.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://fy.yuexingan06.cn


<!-- 参考信息 -->