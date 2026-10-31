代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://pk.huanxung.cn

Ruby: arr.include?(x)
来源：http://vc.colortex.cn

C#:   list.Contains(x)
来源：http://kl.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://xr.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hy.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cf.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eb.shxzskj.cn

TS:   [...arr];
来源：http://ja.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://dt.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yv.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://ob.lnxyls.cn

C#:   new List<int>(list);
来源：http://sy.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://ot.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ol.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cv.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yc.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oj.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yl.hnjuh.cn

Go:   // 手写循环
来源：http://ey.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dd.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nn.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://wr.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gh.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qp.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sr.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fd.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gv.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jp.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fk.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://iv.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://py.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gg.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uh.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gp.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lp.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zc.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://he.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ue.wgjwhj.cn

[D26] 数组转字符串
来源：http://tq.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://eb.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://av.asd995.cn

JS:   arr.join(", ")
来源：http://hw.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://pj.szsharing.cn

Java: String.join(", ", list)
来源：http://bk.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://kc.asd995.cn

Ruby: arr.join(", ")
来源：http://fm.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://wh.lnxyls.cn

================================================================================
来源：http://bo.jianghongdianzi.cn

E. 字符串处理
来源：http://dy.bookmarksfly.cn

================================================================================
来源：http://wu.shtwfgs.cn

[E01] 拼接字符串
来源：http://pu.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://id.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cg.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cl.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xy.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gw.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tm.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lw.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bj.szxytkj.cn

[E02] 重复字符串
来源：http://km.9csxet.cn

Py:   "ab" * 3
来源：http://ca.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://rb.hahajie.cn

JS:   "ab".repeat(3)
来源：http://ue.szsharing.cn

TS:   "ab".repeat(3)
来源：http://dx.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://jk.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://hz.haigaiapp.cn

Ruby: "ab" * 3
来源：http://fn.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ki.muxihuayi.cn

[E03] 截取子串
来源：http://ny.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cg.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xq.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://db.nicolike.cn

TS:   s.slice(1, 4)
来源：http://of.hahajie.cn

Java: s.substring(1, 4)
来源：http://ns.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zg.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dl.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://nt.wgjwhj.cn

[E04] 查找子串位置
来源：http://mo.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://ti.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://mz.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://az.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://nf.shtwfgs.cn

Java: s.indexOf("x")
来源：http://my.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://gs.bjjhwx.cn

Ruby: s.index("x")
来源：http://iu.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://lu.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ld.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pc.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://to.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uk.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vm.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zg.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vk.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ay.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jv.hnjuh.cn

[E06] 替换子串
来源：http://ki.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vn.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://gl.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mv.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://bc.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kh.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qf.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wx.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://rn.521024.cn

[E07] 按分隔符拆分
来源：http://px.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hh.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qq.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gv.521024.cn

TS:   s.split(",")
来源：http://ss.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xz.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qo.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://sm.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://se.asd995.cn

[E08] 数组按分隔符合并
来源：http://ei.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ol.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://cv.jctech888.com.cn

JS:   items.join(",")
来源：http://gg.asd995.cn

TS:   items.join(",")
来源：http://iz.521024.cn

Java: String.join(",", items)
来源：http://qf.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://xr.shxzskj.cn

Ruby: items.join(",")
来源：http://zt.hahajie.cn

C#:   string.Join(",", items)
来源：http://ks.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://ka.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fs.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ad.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://rt.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ar.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://cn.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ov.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zw.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ht.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://uj.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rm.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lo.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ys.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://rz.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://jt.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mo.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ms.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vp.521024.cn

[E11] 反转字符串
来源：http://mo.chemitech.net.cn

Py:   s[::-1]
来源：http://cl.bookmarksfly.cn

PHP:  strrev($s);
来源：http://om.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://st.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://rk.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ow.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jk.szxytkj.cn

Ruby: s.reverse
来源：http://xi.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jk.huanxung.cn

[E12] 统计某字符出现次数
来源：http://ov.yuexingan06.cn

Py:   s.count("a")
来源：http://xq.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://cm.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://tq.szsharing.cn

TS:   s.split("a").length - 1
来源：http://bq.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mo.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://wr.chemitech.net.cn

Ruby: s.count("a")
来源：http://ra.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://hi.yuexingan06.cn

[E13] 逐字符遍历
来源：http://nf.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://gn.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ny.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lk.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ax.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oi.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dz.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vu.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sa.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://yz.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oa.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rj.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://km.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kc.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wg.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zo.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xs.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wr.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://uy.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gs.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vd.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kp.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fw.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ol.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mr.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bj.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yl.muxihuayi.cn

[E16] 数字千分位
来源：http://xb.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://dj.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://kc.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://le.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vr.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bi.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xs.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ow.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://oq.nicolike.cn

[E17] 首字母大写
来源：http://vk.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hl.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ye.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tb.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fc.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ba.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cx.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ol.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://io.shxzukj.cn

[E18] 模板占位符替换
来源：http://at.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iq.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fo.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://of.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vm.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qg.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mo.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ru.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.huanxung.cn

[E19] 多行文本按行拆分
来源：http://ai.shxzskj.cn

Py:   s.splitlines()
来源：http://hf.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xt.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://oq.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://dd.huixiangedu.cn

Java: s.lines().toList()
来源：http://ei.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://aq.shxzskj.cn

Ruby: s.lines
来源：http://hc.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://qi.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://mu.huanxung.cn

Py:   if not s:
来源：http://hj.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pv.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wb.lnxyls.cn

TS:   if (s === "") {}
来源：http://my.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ht.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://ls.521024.cn

Ruby: if s.empty?
来源：http://dq.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mk.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ub.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://if.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hm.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vv.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nr.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://tm.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bs.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ls.newstarts.cn

[E22] 字节长度与字符长度
来源：http://gv.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kj.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://re.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oz.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ov.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xc.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qy.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://uu.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://op.nszjky.cn

================================================================================
来源：http://zd.huixinmuqiang.cn

F. 文件与目录
来源：http://jl.jianghongdianzi.cn

================================================================================
来源：http://ny.gzmigu.cn

[F01] 读取整个文件
来源：http://br.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jl.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://xg.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dp.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sl.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gk.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jy.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://be.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://al.newstarts.cn

[F02] 逐行读取文件
来源：http://mp.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pj.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vm.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aa.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aq.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ik.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ml.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mx.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://om.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://cv.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lk.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yn.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vn.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jg.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oa.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zy.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://lt.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yr.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://kb.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ht.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uf.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hy.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vt.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xu.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://at.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tt.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://eo.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uy.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://rp.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://in.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ks.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hd.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ld.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://fg.521024.cn

C#:   File.Exists("a.txt")
来源：http://bx.shxzskj.cn

[F06] 删除文件
来源：http://mf.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://gu.hahajie.cn

PHP:  unlink("a.txt");
来源：http://lo.szsharing.cn


<!-- 参考信息 -->