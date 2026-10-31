代发 wailian999

Java: new ArrayList<>(list);
来源：http://kh.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ph.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://fu.szsharing.cn

C#:   new List<int>(list);
来源：http://yr.bjjhwx.cn

[D23] reduce 累积计算
来源：http://cu.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pa.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yu.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kc.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yn.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gy.hnjuh.cn

Go:   // 手写循环
来源：http://ve.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cy.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ph.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ng.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xw.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jd.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bt.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ix.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yn.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eb.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xs.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cc.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://vn.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pr.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sy.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oe.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://br.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vp.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qz.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dm.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bf.521024.cn

[D26] 数组转字符串
来源：http://rj.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://am.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://au.nicolike.cn

JS:   arr.join(", ")
来源：http://vc.shxzskj.cn

TS:   arr.join(", ")
来源：http://op.lnxyls.cn

Java: String.join(", ", list)
来源：http://od.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://kc.521024.cn

Ruby: arr.join(", ")
来源：http://kx.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://iv.nicolike.cn

================================================================================
来源：http://yw.jctech888.com.cn

E. 字符串处理
来源：http://hd.panjiajie.cn

================================================================================
来源：http://xx.lnxyls.cn

[E01] 拼接字符串
来源：http://yb.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qc.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ot.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lu.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uf.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zu.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://we.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kd.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ce.nicolike.cn

[E02] 重复字符串
来源：http://wq.yuexingan06.cn

Py:   "ab" * 3
来源：http://kp.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://yv.9csxet.cn

JS:   "ab".repeat(3)
来源：http://ei.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ct.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ff.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://yl.haigaiapp.cn

Ruby: "ab" * 3
来源：http://lw.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lb.szsharing.cn

[E03] 截取子串
来源：http://fz.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zj.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hw.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ye.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://aw.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://dn.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://br.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mx.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://cm.newstarts.cn

[E04] 查找子串位置
来源：http://dk.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://ub.nicolike.cn

PHP:  strpos($s, "x");
来源：http://ct.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pj.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://ch.shtwfgs.cn

Java: s.indexOf("x")
来源：http://jx.asd995.cn

Go:   strings.Index(s, "x")
来源：http://az.521024.cn

Ruby: s.index("x")
来源：http://jv.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ob.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wb.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://du.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vk.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qs.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jv.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qt.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wk.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hk.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kz.huixinmuqiang.cn

[E06] 替换子串
来源：http://no.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zb.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://ux.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qt.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://ab.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uq.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nn.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qy.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://rd.szsharing.cn

[E07] 按分隔符拆分
来源：http://rp.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fg.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zx.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ps.colortex.cn

TS:   s.split(",")
来源：http://om.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qh.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ze.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://sj.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fc.nicolike.cn

[E08] 数组按分隔符合并
来源：http://pi.huanxung.cn

Py:   ",".join(items)
来源：http://so.gzmigu.cn

PHP:  implode(",", $items);
来源：http://lo.jianghongdianzi.cn

JS:   items.join(",")
来源：http://jj.bjjhwx.cn

TS:   items.join(",")
来源：http://wy.shxzskj.cn

Java: String.join(",", items)
来源：http://ep.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://fb.bookmarksfly.cn

Ruby: items.join(",")
来源：http://rw.asd995.cn

C#:   string.Join(",", items)
来源：http://aa.colortex.cn

[E09] 去除所有空白字符
来源：http://hc.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cl.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hd.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://eb.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://vk.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://wx.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ey.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://py.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ep.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://dp.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kk.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vg.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://md.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://hx.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://jp.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pk.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hl.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oc.bookmarksfly.cn

[E11] 反转字符串
来源：http://xq.jianghongdianzi.cn

Py:   s[::-1]
来源：http://nq.jctech888.com.cn

PHP:  strrev($s);
来源：http://qg.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://pp.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://cy.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bn.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ww.bookmarksfly.cn

Ruby: s.reverse
来源：http://dd.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ki.huanxung.cn

[E12] 统计某字符出现次数
来源：http://qo.nszjky.cn

Py:   s.count("a")
来源：http://yi.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://sx.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://si.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://af.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://qn.lnxyls.cn

Ruby: s.count("a")
来源：http://yr.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://df.shxzukj.cn

[E13] 逐字符遍历
来源：http://ej.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://hg.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bg.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mt.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://de.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gi.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mu.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xy.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ur.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ka.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ke.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://px.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uo.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zj.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sr.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sf.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vb.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zb.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://im.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hm.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dl.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ai.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fx.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xh.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://li.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qn.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://py.jianghongdianzi.cn

[E16] 数字千分位
来源：http://oj.huanxung.cn

Py:   f"{1234567:,}"
来源：http://mq.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://bp.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ve.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://on.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rp.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zk.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ol.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://hs.yuexingan06.cn

[E17] 首字母大写
来源：http://st.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bq.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://by.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xf.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vm.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ps.shxzukj.cn

Ruby: s.capitalize
来源：http://cc.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ih.lnxyls.cn

[E18] 模板占位符替换
来源：http://pt.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jk.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://np.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sr.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rr.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yf.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iu.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tx.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.9csxet.cn

[E19] 多行文本按行拆分
来源：http://cn.lnxyls.cn

Py:   s.splitlines()
来源：http://wm.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lf.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://ow.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://od.yuexingan06.cn

Java: s.lines().toList()
来源：http://xn.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://ku.shxzukj.cn

Ruby: s.lines
来源：http://jc.huanxung.cn

C#:   s.Split('\n')
来源：http://td.nszjky.cn

[E20] 判断字符串是否为空
来源：http://gl.521024.cn

Py:   if not s:
来源：http://jy.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hq.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rz.jctech888.com.cn

TS:   if (s === "") {}
来源：http://tp.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://mn.szsharing.cn

Go:   if s == "" {}
来源：http://ss.yuexingan06.cn

Ruby: if s.empty?
来源：http://tq.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dy.szsharing.cn

[E21] 超长截断加省略号
来源：http://af.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rt.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pf.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://re.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://th.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://xr.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kw.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fs.asd995.cn

[E22] 字节长度与字符长度
来源：http://ms.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sn.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bn.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ji.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rh.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mg.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dx.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://wj.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cp.yuexingan06.cn

================================================================================
来源：http://tr.huanxung.cn

F. 文件与目录
来源：http://fu.asd995.cn

================================================================================
来源：http://xj.chemitech.net.cn

[F01] 读取整个文件
来源：http://vg.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://em.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://er.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ci.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pd.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pc.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rj.521024.cn

Ruby: File.read("a.txt")
来源：http://mq.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://lz.chemitech.net.cn

[F02] 逐行读取文件
来源：http://ok.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fe.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sz.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bm.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://el.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xh.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yi.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yv.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bq.521024.cn

[F03] 写入文件（覆盖）
来源：http://zq.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ps.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iu.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lg.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://is.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://px.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sb.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://gj.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ap.szxytkj.cn

[F04] 追加写入文件
来源：http://cl.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cv.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mv.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jl.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mv.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ay.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vc.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ww.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kb.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://iw.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wj.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://pm.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://mt.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://gq.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ke.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cv.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://uy.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://pf.huanxung.cn

[F06] 删除文件
来源：http://vc.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://ca.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://aj.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://za.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oc.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mv.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://sp.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://yx.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://dm.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://ml.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qk.szsharing.cn


<!-- 参考信息 -->