代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://kn.hahajie.cn

Ruby: arr.include?(x)
来源：http://zr.nszjky.cn

C#:   list.Contains(x)
来源：http://bb.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ye.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ii.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zv.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dz.asd995.cn

TS:   [...arr];
来源：http://rv.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://fd.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cg.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://ra.yuexingan06.cn

C#:   new List<int>(list);
来源：http://pi.hahajie.cn

[D23] reduce 累积计算
来源：http://vm.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://un.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fo.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rn.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zv.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ye.bjjhwx.cn

Go:   // 手写循环
来源：http://pa.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yv.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ww.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ie.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sb.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yc.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zj.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vb.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hx.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oy.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dw.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pm.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://mw.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zh.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yb.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mh.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hy.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ah.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yo.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gk.panjiajie.cn

[D26] 数组转字符串
来源：http://ex.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://np.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://ez.huixiangedu.cn

JS:   arr.join(", ")
来源：http://ce.521024.cn

TS:   arr.join(", ")
来源：http://qk.jctech888.com.cn

Java: String.join(", ", list)
来源：http://lm.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://ec.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://iv.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://uc.hahajie.cn

================================================================================
来源：http://fc.shtwfgs.cn

E. 字符串处理
来源：http://lz.szxytkj.cn

================================================================================
来源：http://pd.yuexingan06.cn

[E01] 拼接字符串
来源：http://nv.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lr.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jn.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qr.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kl.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wj.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ll.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sg.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tq.haigaiapp.cn

[E02] 重复字符串
来源：http://sh.bjjhwx.cn

Py:   "ab" * 3
来源：http://ey.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://xg.huanxung.cn

JS:   "ab".repeat(3)
来源：http://bc.9csxet.cn

TS:   "ab".repeat(3)
来源：http://uj.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://zp.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://rp.asd995.cn

Ruby: "ab" * 3
来源：http://tw.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fy.9csxet.cn

[E03] 截取子串
来源：http://rx.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zl.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hq.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tj.asd995.cn

TS:   s.slice(1, 4)
来源：http://rr.nszjky.cn

Java: s.substring(1, 4)
来源：http://eh.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hp.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dc.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://rn.gzmigu.cn

[E04] 查找子串位置
来源：http://la.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://zw.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://kt.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tr.shxzukj.cn

TS:   s.indexOf("x")
来源：http://fm.521024.cn

Java: s.indexOf("x")
来源：http://hp.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://ld.9csxet.cn

Ruby: s.index("x")
来源：http://qr.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://ni.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jn.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wn.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vo.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pp.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://we.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nz.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dm.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ew.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rj.haigaiapp.cn

[E06] 替换子串
来源：http://ka.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cn.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://dq.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xs.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://ra.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ed.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gq.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kh.colortex.cn

C#:   s.Replace("a", "b")
来源：http://ay.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://yv.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uh.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kh.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ou.shxzskj.cn

TS:   s.split(",")
来源：http://si.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cs.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://tr.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ay.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://pq.shxzskj.cn

Py:   ",".join(items)
来源：http://pn.hahajie.cn

PHP:  implode(",", $items);
来源：http://ch.bjjhwx.cn

JS:   items.join(",")
来源：http://fm.yuexingan06.cn

TS:   items.join(",")
来源：http://zw.shtwfgs.cn

Java: String.join(",", items)
来源：http://xv.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://pq.shxzskj.cn

Ruby: items.join(",")
来源：http://go.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://rw.huanxung.cn

[E09] 去除所有空白字符
来源：http://dp.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jk.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sv.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ol.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://qy.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ty.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vh.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ct.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gh.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://vn.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oo.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tg.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://oj.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://xj.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://hc.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bg.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pd.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aw.newstarts.cn

[E11] 反转字符串
来源：http://hx.lnxyls.cn

Py:   s[::-1]
来源：http://mn.newstarts.cn

PHP:  strrev($s);
来源：http://im.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://hv.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://ze.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gl.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gl.nszjky.cn

Ruby: s.reverse
来源：http://js.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uy.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://lq.shxzukj.cn

Py:   s.count("a")
来源：http://sp.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://dd.521024.cn

JS:   s.split("a").length - 1
来源：http://nl.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://ol.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xc.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ix.nicolike.cn

Ruby: s.count("a")
来源：http://vz.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://vq.huanxung.cn

[E13] 逐字符遍历
来源：http://ow.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://xb.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jp.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vk.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kc.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fb.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zs.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ox.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ju.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://ku.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ef.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bh.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yj.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lr.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hs.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ug.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qf.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dz.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://qv.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bs.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kj.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fd.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kb.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ss.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vn.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://an.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ho.hnjuh.cn

[E16] 数字千分位
来源：http://cx.hahajie.cn

Py:   f"{1234567:,}"
来源：http://qv.shxzukj.cn

PHP:  number_format(1234567);
来源：http://ve.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vt.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://am.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pn.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pi.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vp.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://vt.szxytkj.cn

[E17] 首字母大写
来源：http://xn.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mn.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://by.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pr.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ud.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gx.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ee.newstarts.cn

Ruby: s.capitalize
来源：http://kv.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gi.shtwfgs.cn

[E18] 模板占位符替换
来源：http://lr.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vd.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ri.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xc.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pc.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lt.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://co.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://na.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://me.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://cl.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://jo.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rm.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://as.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://hj.bjjhwx.cn

Java: s.lines().toList()
来源：http://in.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://px.shxzukj.cn

Ruby: s.lines
来源：http://zr.521024.cn

C#:   s.Split('\n')
来源：http://wg.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ux.huanxung.cn

Py:   if not s:
来源：http://so.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vn.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://an.hnjuh.cn

TS:   if (s === "") {}
来源：http://pd.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://to.colortex.cn

Go:   if s == "" {}
来源：http://ut.huixiangedu.cn

Ruby: if s.empty?
来源：http://iv.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qd.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://qz.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rs.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ba.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dk.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hx.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uk.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://xk.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sf.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bw.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://dx.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ma.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://df.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sl.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://br.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rp.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uh.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://no.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mw.shxzskj.cn

================================================================================
来源：http://hz.shtwfgs.cn

F. 文件与目录
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://ip.nszjky.cn

[F01] 读取整个文件
来源：http://xp.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vj.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://uy.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yg.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oo.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zv.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gm.9csxet.cn

Ruby: File.read("a.txt")
来源：http://up.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://oy.chemitech.net.cn

[F02] 逐行读取文件
来源：http://he.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vf.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wr.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bj.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iy.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://au.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nt.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xt.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jg.colortex.cn

[F03] 写入文件（覆盖）
来源：http://nq.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qz.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ez.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gf.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kz.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yo.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iz.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://wr.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://op.colortex.cn

[F04] 追加写入文件
来源：http://bb.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dq.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tc.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gi.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yp.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ol.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oc.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ld.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tu.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://kr.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tf.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://ga.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://oy.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://wm.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qw.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mh.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://wn.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://ft.colortex.cn

[F06] 删除文件
来源：http://nm.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://uh.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://gn.9csxet.cn


<!-- 参考信息 -->